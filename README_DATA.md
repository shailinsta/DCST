# Data directory (datasets not redistributed)

Place the following files here (or update paths in `DCST_complete_pipeline.ipynb`):

| File | Source | Role |
|------|--------|------|
| `clinical.tsv` | [GDC TCGA-PAAD](https://portal.gdc.cancer.gov/projects/TCGA-PAAD) | Primary real clinical cohort (N≈92 evaluable) |
| `GSE32676_series_matrix.txt` | [GEO GSE32676](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE32676) | Supplementary expression (N=32) |
| `PDC_study_clinical_*.csv` | CPTAC / PDC (Cao et al., *Cell* 2021) | Supplementary clinical (N=166) |

The in-silico multi-omics cohort (N=800) is **generated inside the notebook** and does not require external files.

Do not commit controlled-access or large raw omics files to this public repository.
