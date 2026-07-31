# HS Rats Adipose–Liver eQTL Trans-Bands Report

Interactive progress report for the LD-based trans-eQTL band analysis and GO/KEGG enrichment in HS rat adipose and liver tissues.

## View the report online

Once this repository is published with GitHub Pages, the report is available at:

```text
https://YOUR_USERNAME.github.io/HS_rats_eQTLs_transbands/
```

The page contains:
- an LD-based Peirce-style cis–trans overview
- trans-band Manhattan plots
- LocusZoom-style priority band views
- an UpSet plot of target-gene overlap
- a band × term heatmap
- GO/KEGG enrichment summary plots

The interactive Manhattan and LocusZoom plots are zoomable/pannable and work offline because the Plotly library is included in the repository.

## Downloadable bundle

`HS_rats_eQTLs_transbands.zip` in this folder contains the same files for offline use or local sharing.

## How to publish on GitHub Pages

### 1. Create a GitHub repository

Create a new repository named `HS_rats_eQTLs_transbands` (or any name you prefer) on GitHub.

### 2. Push this folder to GitHub

From this directory, run:

```bash
git remote add origin https://github.com/YOUR_USERNAME/HS_rats_eQTLs_transbands.git
git branch -M main
git push -u origin main
```

Use a GitHub **Personal Access Token** when prompted for the password.

### 3. Enable GitHub Pages

- On the repository page, go to **Settings → Pages**.
- Under **Build and deployment → Source**, select **Deploy from a branch**.
- Choose the **main** branch and the **/ (root)** folder.
- Click **Save**.

After about one minute, the report will be live at:

```text
https://YOUR_USERNAME.github.io/HS_rats_eQTLs_transbands/
```

## Files included

| File / folder | Purpose |
|---------------|---------|
| `index.html` | Main report (open this in a browser) |
| `progress_report_style.css` | Report styling |
| `plotly.min.js` | Local Plotly library for offline interactive plots |
| `*.png` | Static figures |
| `*.html` (other than `index.html`) | Interactive Manhattan and LocusZoom plots |
| `enrichment_gokegg/` | GO/KEGG summary figures |
| `progress_report_0826_v5.pdf` | PDF version of the report |
| `.nojekyll` | Disables Jekyll processing on GitHub Pages |
| `HS_rats_eQTLs_transbands.zip` | Zipped copy of the whole bundle |

## Updating the report

Replace any figures or the HTML/CSS files and push the changes. GitHub Pages will update automatically within a few minutes.
