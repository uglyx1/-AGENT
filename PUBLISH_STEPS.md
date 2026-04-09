# Publish Steps (Docs-Only Repo)

Run these commands from the `public_release` directory:

```powershell
cd public_release
git init
git checkout -b main
git add .
git commit -m "docs: public showcase for commerce ops agent"
git remote add origin <YOUR_GITHUB_REPO_URL>
git push -u origin main
```

Recommended:

- create a new empty GitHub repository first
- do **not** push the parent project root
- keep this repo docs-only
