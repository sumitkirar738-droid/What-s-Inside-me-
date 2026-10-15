VERCEL DEPLOY FIX

The 404 page usually means Vercel did not find a default entry page at the deployed root.
This folder contains:
- index.html: your letter site (renamed from the standalone HTML file)
- vercel.json: minimal static-site configuration

Deploy steps:
1. Extract this ZIP.
2. In Vercel, open your project -> Settings -> Build and Development Settings.
3. For a plain HTML site, set Framework Preset to Other, and leave Build Command empty.
4. Set Output Directory to . (a single dot), and make sure Root Directory points to the folder containing index.html.
5. Commit/upload index.html and vercel.json to the project root, then redeploy.
If deploying from Git, ensure these files are committed in the connected repository's root (or set Root Directory to their folder).
