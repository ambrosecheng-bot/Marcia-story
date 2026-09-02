# Notes for agents

- The whole site is a single self-contained `index.html` (~12 MB, portrait image embedded as base64). No build step, no dependencies, no secrets.
- Served in dev by nginx (`docker-compose.base44.yml`) with the repo bind-mounted read-only at `/usr/share/nginx/html`, published on host port 3000.
- Quirk: the sandbox repo directory is mode 0700 root-only, so nginx *worker* processes must also run as root. The compose command rewrites the `user` directive in `nginx.conf` before starting; running only the container as `user: root` is not enough (workers still drop to `nginx` and get 403).
- Verify: `curl -s -o /dev/null -w '%{http_code}' http://localhost:3000/` → 200.
- Editing `index.html` is picked up on the next page load (static file, no restart needed); use a forced preview reload.
