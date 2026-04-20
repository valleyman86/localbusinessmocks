# GitHub Pages Setup (One-Time)

Use this once, then we can publish every new mock site quickly.

## 1. Create A New GitHub Repo

Suggested repo name: `local-business-mock-sites`

- Create it as **Public** (easiest for Pages + sharing demo links).
- Do not initialize with a README (this folder already has one).

## 2. Initialize Git Locally

Run from this folder:

```bash
git init
git branch -M main
git add .
git commit -m "Initial starter setup"
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/local-business-mock-sites.git
git push -u origin main
```

If `origin` already exists, update it:

```bash
git remote set-url origin https://github.com/<YOUR_GITHUB_USERNAME>/local-business-mock-sites.git
```

## 3. Turn On GitHub Pages

In GitHub:

1. Open repo `Settings`.
2. Open `Pages`.
3. Under `Build and deployment`, set:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
4. Save.

Your live URL will be:

`https://<YOUR_GITHUB_USERNAME>.github.io/local-business-mock-sites/`

## 4. Let Me Push For You (From This Environment)

To allow pushes from this machine/session:

1. Authenticate GitHub CLI:

```bash
gh auth login
```

2. Choose:
   - GitHub.com
   - HTTPS
   - Authenticate in browser
3. Confirm with:

```bash
gh auth status
```

Once that is done, I can run normal `git add`, `git commit`, and `git push` for you here.

## 5. Ongoing Publish Flow

For each update:

```bash
git add .
git commit -m "Update mock site"
git push
```

GitHub Pages usually updates in about 1-2 minutes.
