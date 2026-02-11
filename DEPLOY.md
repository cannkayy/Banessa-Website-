# Deploy to Vercel with GitHub

## 1. Create a repo on GitHub

- Go to [github.com/new](https://github.com/new).
- Name it (e.g. `banessa-valentine` or `banessa-website`).
- **Do not** add a README, .gitignore, or license (this project already has them).
- Click **Create repository**.

## 2. Push this project to GitHub

In Terminal, from this folder:

```bash
cd "/Users/cannonhurst/Documents/Banessa Website"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your GitHub username and the repo name you chose.

## 3. Connect the repo to Vercel

- Go to [vercel.com](https://vercel.com) and sign in (use “Continue with GitHub” if you like).
- Click **Add New…** → **Project**.
- Under **Import Git Repository**, select your repo and click **Import**.
- Leave **Build Command** and **Output Directory** empty (it’s a static site).
- Click **Deploy**.

Vercel will build and give you a URL like `https://your-project.vercel.app`.

## 4. Updating the site later

After you change the site:

```bash
git add .
git commit -m "Update message"
git push
```

Vercel will automatically redeploy when you push to `main`.
