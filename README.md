# DCST: Dynamic Causal Spatiotemporal Digital Twins for Individualized Treatment-Response Prediction in Pancreatic Ductal Adenocarcinoma
# Shailendra Mishra, Megha Rathi, Himani Agarwal, and Saumya Mishr
# Pancreatic ductal adenocarcinoma (PDAC) exhibits extreme inter-patient heterogeneity in treatment response and five-year survival below 13%. Existing computational approaches either discard multi-relational temporal dynamics or lack formal uncertainty-aware causal reasoning under privacy constraints. We introduce Dynamic Causal SpatioTwin (DCST), a systems-level architecture that models each patient as a multi-scale spatiotemporal dynamical system. DCST unifies four components: (i) a multi-scale residual Heterogeneous Graph Transformer with cross-scale attention and temporal GRU, (ii) a hierarchical Bayesian digital twin with temporal dependence realized by stochastic variational inference, (iii) an uncertainty-aware causal intervention planner that optimizes a reward–uncertainty trade-off, and (iv) uncertainty-weighted adaptive DP-FedAvg under differential-privacy guarantees. Under a strictly leakage-free evaluation protocol on a signal-controlled in silico cohort (N = 800) and real TCGA-PAAD clinical data (N = 92), a capacity-matched residual graph-attention proxy with Monte-Carlo dropout recovers all planted biomarkers and attains AUC-ROC = 0.705 (95% CI [0.619, 0.787]), AUPRC = 0.716, and the highest F1 (0.715) and MCC (0.322) among evaluated models on the in silico test set. On the real clinical cohort under repeated 5 × 5 cross-validation, all models cluster within AUC 0.56–0.58 with no significant pairwise difference, quantifying the ceiling of clinical covariates alone at modest sample size. Single-split execution of the full architecture yields test AUCs of 0.716 (Bayesian twin) and 0.693 (private DP-FedAvg). DCST establishes a coherent framework jointly realizing multi-scale dynamic graphs, temporal Bayesian uncertainty, causal planning and adaptive privacy-preserving federation for PDAC treatment-response prediction.

# DCST — Extracted Tables (Main Paper + Supplementary)

All tables from the IEEE JBHI manuscript and Supplementary Materials, exported for the GitHub repository.

| ID | Caption | CSV | Markdown |
|----|---------|-----|----------|
| `table_i` | TABLE I — Data sources used in the experimental evaluation | [table_i.csv](table_i.csv) | [table_i.md](table_i.md) |
| `table_ii` | TABLE II — Test-set performance of the DCST proxy (N = 160) | [table_ii.csv](table_ii.csv) | [table_ii.md](table_ii.md) |
| `table_iii` | TABLE III — Comparative performance on the in-silico test set (N = 160) | [table_iii.csv](table_iii.csv) | [table_iii.md](table_iii.md) |
| `table_iv` | TABLE IV — Modality ablation on the in silico test set | [table_iv.csv](table_iv.csv) | [table_iv.md](table_iv.md) |
| `table_v` | TABLE V — Mean AUC ± SD across three independent in silico partitions | [table_v.csv](table_v.csv) | [table_v.md](table_v.md) |
| `table_vi` | TABLE VI — Repeated 5×5 cross-validation on real TCGA-PAAD clinical data (N = 92) | [table_vi.csv](table_vi.csv) | [table_vi.md](table_vi.md) |
| `table_vii` | TABLE VII — Paired Wilcoxon signed-rank tests on the 25 real CV folds | [table_vii.csv](table_vii.csv) | [table_vii.md](table_vii.md) |
| `table_viii` | TABLE VIII — Single-split results for full-architecture components and graph-neural baselines (TCGA-PAAD, test N = 19) | [table_viii.csv](table_viii.csv) | [table_viii.md](table_viii.md) |
| `table_ix` | TABLE IX — Research questions and findings | [table_ix.csv](table_ix.csv) | [table_ix.md](table_ix.md) |
| `table_s1` | TABLE S1 — Positioning relative to selected 2025–2026 studies | [table_s1.csv](table_s1.csv) | [table_s1.md](table_s1.md) |
| `table_s2` | TABLE S2 — Contribution profile vs. typical 2025–2026 studies | [table_s2.csv](table_s2.csv) | [table_s2.md](table_s2.md) |
| `table_s3` | TABLE S3 — Hyper-parameters for the residual graph-attention proxy and full-architecture components | [table_s3.csv](table_s3.csv) | [table_s3.md](table_s3.md) |

Also available as a single file: [`all_tables.json`](all_tables.json).
