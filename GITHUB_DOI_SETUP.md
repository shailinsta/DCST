# GitHub Repository and DOI Setup — DCST

Follow these steps to publish the repository and obtain a DOI (Zenodo or equivalent).  
(Adapted from project release practice; replace placeholders with your GitHub username.)

## Part 1 — Create the GitHub repository

1. Go to https://github.com/new  
2. **Repository name:** `DCST`  
3. **Description:** `Dynamic Causal Spatiotemporal Digital Twins for PDAC Treatment-Response Prediction`  
4. Visibility: **Public** (required for most DOI services)  
5. **Do not** add a README, license, or `.gitignore` on GitHub (this folder already has them).  
6. Click **Create repository**.

## Part 2 — Upload this folder

Final structure on GitHub should be:

```
DCST/
├── DCST_complete_pipeline.ipynb
├── README.md
├── requirements.txt
├── CITATION.cff
├── zenodo.json
├── .gitignore
├── GITHUB_DOI_SETUP.md
├── figures/
│   ├── fig1_dcst_architecture.jpeg
│   ├── fig2_hgt_block.png
│   ├── fig3_training_val_auc.png
│   ├── fig4_ensemble_val_auc.png
│   ├── fig5_bootstrap_auc.png
│   ├── fig6_roc_pr_curves.png
│   ├── fig7_foldwise_cv_auc.png
│   ├── fig8_permutation_importance.png
│   ├── fig9_causal_planner.png
│   └── fig10_dp_fedavg.png
├── results/
│   └── partC_summary.json
└── data/
    └── README_DATA.md
```

**Do not** upload raw `clinical.tsv`, GEO matrix, or CPTAC CSVs.  
**Do not** include passwords, API keys, or private Drive links.

Commit message example: `Initial DCST project release v1.0.0`

## Part 3 — Pre-DOI checklist

- [ ] README.md opens correctly  
- [ ] `DCST_complete_pipeline.ipynb` is in the repository root  
- [ ] `requirements.txt`, `CITATION.cff`, `zenodo.json` present  
- [ ] All 10 figures present under `figures/`  
- [ ] `results/partC_summary.json` present  
- [ ] No private data or credentials  
- [ ] Update `YOUR_USERNAME` in README.md and CITATION.cff  

## Part 4 — Create a GitHub Release

1. Repository → **Releases** → **Create a new release**  
2. Tag: `v1.0.0`  
3. Title: `DCST v1.0.0`  
4. Description:  
   `Initial public release of DCST (Dynamic Causal Spatiotemporal Digital Twins for PDAC), including the Colab-ready notebook, figures, and summary results.`  
5. Publish release.

## Part 5 — Obtain a DOI (Zenodo)

1. Log in to [Zenodo](https://zenodo.org/) with the same GitHub account.  
2. Enable GitHub integration; select the `DCST` repository.  
3. Create a release on GitHub (or trigger from Zenodo).  
4. Zenodo assigns a **DOI** (e.g. `10.5281/zenodo.xxxxxxxx`).  
5. Paste the DOI into:
   - Manuscript Data Availability / Software Availability  
   - `README.md` citation block  
   - `CITATION.cff` (`identifiers` section if desired)

## Part 6 — Update the manuscript

After the DOI is live, replace the placeholder in the main paper and Supplementary Materials:

> URL to be provided upon acceptance  

with:

> https://doi.org/10.5281/zenodo.xxxxxxxx  
> (or the GitHub release URL)

## Google Colab note

Users can open the notebook directly from GitHub in Colab:

`https://colab.research.google.com/github/YOUR_USERNAME/DCST/blob/main/DCST_complete_pipeline.ipynb`
