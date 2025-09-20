[README_DEPLOY.txt](https://github.com/user-attachments/files/22448681/README_DEPLOY.txt)
Deployable Atlanta Dashboard Bundle

Files:
- index.html
- data/atlanta_growth_template.csv
- embed_snippet.html
- netlify.toml (optional)

How to deploy

A) GitHub Pages
1. New public repo (e.g., atlanta-dashboard).
2. Upload these files to the repo root.
3. Settings → Pages → Branch: main, Folder: /root.
4. Your URL will look like https://USERNAME.github.io/atlanta-dashboard/

B) Netlify
1. app.netlify.com → New site from drag-and-drop.
2. Drop this folder. Done. You’ll get a netlify.app URL.

C) Vercel
1. Create a new project and import your repo or use CLI.
2. Deploy; you’ll get a vercel.app URL.

Embed in Webflow/Relume
Use this iframe code in a Webflow Embed element:
<iframe 
  src="YOUR_HOSTED_URL/index.html" 
  width="100%" 
  height="820" 
  style="border:none;"
  loading="lazy" 
  referrerpolicy="no-referrer-when-downgrade"
  allowfullscreen>
</iframe>

Notes
- Plotly loads from a CDN. For fully offline use, vendor plotly-latest.min.js locally.
- To update data, regenerate or wire the page to fetch CSV and redraw.
