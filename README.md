# TMAE/PMTA Experiment Repository

Authors: Vladimir Vasilenko (b102e)  
Date: May 2026

This repository contains the code and reproducibility assets for the TMAE/PMTA experiment on adversarial attacks against persistent-identity LLM agents. It includes activation extraction, metric computation (M1/M2/M3), phase classification, pilot-gate tooling, and statistical analysis scripts aligned with the v1.0.1 preregistration plan.

## Links
- Preregistration repository: [https://github.com/b102e/tmae-pmta-preregistration](https://github.com/b102e/tmae-pmta-preregistration)
- OSF preregistration: [https://osf.io/ugqbp/overview](https://osf.io/ugqbp/overview)
- Registration DOI: [10.17605/OSF.IO/UGQBP](https://doi.org/10.17605/OSF.IO/UGQBP)
- arXiv preprint: [https://arxiv.org/abs/2604.12016](https://arxiv.org/abs/2604.12016)

## Reproducibility
1. Install dependencies:
   - `python -m venv .venv && source .venv/bin/activate`
   - `pip install -r requirements.txt`
2. Run pilot gates (after implementation):
   - `python pilot/m6_threshold_pilot.py`
   - `python pilot/stochasticity_check.py`
3. Run extraction/metrics pipeline (after implementation):
   - `python src/extract_activations.py`
   - `python src/compute_m1_m2.py`
4. Reproduce analysis (after implementation):
   - `python analysis/primary_analysis.py`
   - `python analysis/survival_analysis.py`
   - `python analysis/tost_h3.py`
   - `python analysis/permanova_h4.py`
   - `python analysis/confound_checks.py`

## Repository Structure
- `src/` — extraction, metrics, gates, anchors, phase detection
- `analysis/` — preregistered statistical analyses
- `data/` — data format and schema docs
- `pilot/` — pilot-phase gates and checks
- `results/` — output location for post-collection reports
- `SEED.md` — fixed random seed commitment

## License
This repository is licensed under the MIT License.
