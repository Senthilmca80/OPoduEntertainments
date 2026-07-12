# OPoduEntertainments — Deploy Instructions

This repo contains a static site with `index.html`.

Deployment options:

1) Netlify (recommended quick deploy)

- Drag & drop: Go to https://app.netlify.com/drop and drop the project folder.
- CLI deploy (interactive login required):

```bash
npm i -g netlify-cli
netlify login
netlify deploy --prod --dir=.
```

2) Vercel

- CLI deploy (interactive login):

```bash
npm i -g vercel
vercel login
vercel --prod
```

3) GitHub Pages (CI-based)

- Create a GitHub repo and push this project to the `main` branch.
- In GitHub → Settings → Pages, set Source to `main` branch and `/ (root)`.

Local test

```bash
# from the project folder
python3 -m http.server 8000
# open http://localhost:8000
```

Files added to help deploy: `netlify.toml` and `vercel.json`.

If you want, I can run the CLI deploy for you — tell me which provider and I'll run the commands (you'll need to complete interactive login).
