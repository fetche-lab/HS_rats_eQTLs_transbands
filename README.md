# HS Rat Adipose–Liver Trans-eQTL Hotspot Report

Interactive, self-contained progress report for the LD-based cis/trans eQTL classification, trans-band discovery, candidate driver validation, and pangenome follow-up in Heterogeneous Stock rat adipose and liver tissues.

The main report is fully self-contained: all CSS, JavaScript, and data arrays live inside `index.html`, so it works offline when opened in a browser.

## Repository layout

| Path | Purpose |
|------|---------|
| `index.html` | **Main interactive report** (open this in a browser) |
| `assets/` | Static figures embedded in the report (hotspot bar plots, PC1 enrichment, etc.) |
| `supplementary/` | Downloadable gene lists + interactive tables for literature follow-up |
| `transband_manhattan_adipose.html` | Interactive genome-wide Manhattan plot — adipose |
| `transband_manhattan_liver.html` | Interactive genome-wide Manhattan plot — liver |
| `locuszoom_adipose_chr5_68-70.html` | Interactive LocusZoom-style view of the top adipose band |
| `locuszoom_liver_chr4_177-179.html` | Interactive LocusZoom-style view of the top liver band |
| `peirce_cis_trans_ld_adipose.png` | Static Peirce-style cis/trans LD overview — adipose |
| `peirce_cis_trans_ld_liver.png` | Static Peirce-style cis/trans LD overview — liver |
| `band_term_heatmap.png` | Band × term heatmap |
| `upset_top_bands.png` | UpSet plot of target-gene overlap |
| `enrichment_gokegg/` | GO/KEGG summary figures |
| `progress_report_0826_v5.pdf` | PDF version of the earlier progress report |
| `index_previous_report.html` | Previous version of the HTML report (kept for reference) |
| `plotly.min.js` | Local Plotly library used by the interactive Manhattan/LocusZoom pages |
| `.nojekyll` | Disables Jekyll processing on GitHub Pages |

## Main report contents

- **Abstract** — study summary
- **Overview** — headline numbers and the two strongest hotspots
- **Objectives** — five connected analysis goals with expandable detail cards
- **Cis / Trans** — LD-based classification and the self-hit leakage check
- **Adipose** — confirmed trans-bands and deep dive into `Chr5:68–72 Mb`
- **Liver** — confirmed trans-bands and deep dive into `Chr4:176–184 Mb`
- **Drivers** — candidate driver genes with literature links (GeneCards / PubMed)
- **Enrichment** — GO/KEGG over-representation results and power considerations
- **Pangenome** — proposed next steps for pangenome / structural-variant fine-mapping
- **Gallery** — links to the interactive Manhattan and LocusZoom plots
- **Supplementary** — download gene lists for the top bands
- **Methods** — validation chain and references

## Supplementary gene lists

The top adipose (`Chr5:68–72 Mb`, 73 genes) and liver (`Chr4:176–184 Mb`, 55 genes) target-gene lists are available as:

- CSV files in `supplementary/`
- An interactive, sortable HTML table at `supplementary/supplementary_gene_lists.html`

Each row gives the gene symbol, description, peak −logP, effect size, peak location, and gene location, plus direct GeneCards and PubMed links for literature review.
