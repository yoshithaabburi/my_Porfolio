Production checklist

- Build command: `npm run build`
- Preview static client: `npx serve dist/client`
- Production server: `node dist/server/server.js` (or use Dockerfile)

Vercel

- Project root: `abburi_portfolio` (if configured per repo)
- Build Command: `npm run build`
- Output Directory: `dist/client`
- Environment variables: set any keys (OPENAI_API_KEY, etc.) in Vercel dashboard

Docker

- Build: `docker build -t abburi-portfolio .`
- Run: `docker run -p 3000:3000 abburi-portfolio`

CI

- There's a GitHub Actions workflow in `.github/workflows/ci.yml` that runs lint and build on push/PR to `main`.
