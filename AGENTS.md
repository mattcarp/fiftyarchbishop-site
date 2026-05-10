# Deployment

This site is served by **GitHub Pages** from the `main` branch root.

## Deploying

1. Ensure `main` is clean and up to date with `origin/main`.
2. Update the deploy timestamp in `index.html`:
   - Find the `<span class="deploy-stamp">` element at the bottom of the `<body>`.
   - Replace its contents with the current UTC time, e.g. `2026-05-10 13:46 UTC`.
3. Commit and push to `origin/main`:
   ```
   git add index.html assets/
   git commit -m "Deploy: update timestamp and content"
   git push origin main
   ```
4. GitHub Pages will rebuild within a minute or two. Verify at https://50archbishop.com.
