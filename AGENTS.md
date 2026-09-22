# Notes for agents

- Static single-file site: `index.html` (~12MB, all images embedded as base64). No build step, no dependencies besides Google Fonts via CDN.
- Do not minify or reformat `index.html`.
- Local preview: `docker compose -f docker-compose.base44.yml up -d` → http://localhost:3000. nginx runs its workers as root because the repo root directory is mode 700 (otherwise nginx returns 403).
- Deployment target: GitHub Pages from `main` branch, root folder `/`.
- Verify: `curl -s -o /dev/null -w "%{http_code}" localhost:3000/` should return 200 with ~12MB body.
