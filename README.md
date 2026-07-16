# REST Fault Taxonomy Study

![Research](https://img.shields.io/badge/Research-ICSE%202026-blue) ![Python](https://img.shields.io/badge/Language-Python-3776AB?logo=python&logoColor=white) ![License](https://img.shields.io/badge/License-MIT-green)

## Overview

This repository contains the research artifacts, data, and analysis code supporting the **Defects4REST** study — a systematic taxonomy of defects in REST API implementations. The work characterizes recurring fault patterns across real-world REST APIs, providing a structured classification that helps developers, testers, and tool builders understand where and how REST services fail. The taxonomy was developed through large-scale empirical analysis and published at the **International Conference on Software Engineering (ICSE) 2026**, co-sponsored by ACM and IEEE.

## Highlights

- Systematic classification of REST API defects into a multi-level fault taxonomy
- Empirically grounded: derived from analysis of real-world REST API repositories and bug reports
- Covers fault categories spanning input validation, HTTP semantics, authentication/authorization, error handling, and resource management
- Reusable artifact: taxonomy and datasets are structured for adoption in automated testing, static analysis, and developer education
- Companion to the Defects4REST benchmark — enabling reproducibility of ICSE 2026 findings

## Tech Stack

- **Python** — data collection, parsing, and statistical analysis scripts
- **Jupyter Notebooks** — exploratory analysis and visualization of defect distributions
- **JSON / CSV** — structured storage of taxonomy definitions and annotated defect datasets
- **Git / GitHub** — version control and artifact archiving

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip

### Installation

```bash
git clone https://github.com/katkhedepushpak/REST-fault-taxonomy-study.git
cd REST-fault-taxonomy-study
```

If a `requirements.txt` is present:

```bash
pip install -r requirements.txt
```

If a `pyproject.toml` or `setup.py` is present:

```bash
pip install -e .
```

## Repository Structure

```
REST-fault-taxonomy-study/
├── taxonomy/          # Taxonomy definitions and classification schema
├── data/              # Annotated defect datasets and raw bug reports
├── analysis/          # Scripts for statistical analysis and chart generation
├── notebooks/         # Jupyter notebooks for exploratory analysis
└── results/           # Figures and tables referenced in the ICSE 2026 paper
```

> Note: Exact directory layout may vary. Refer to individual folder READMEs or inline comments for details.

## Usage

To reproduce the taxonomy analysis:

```bash
python analysis/run_taxonomy_analysis.py
```

To explore defect distributions interactively:

```bash
jupyter notebook notebooks/
```

Refer to the scripts in `analysis/` for command-line options and configuration flags.

## Citation

If you use this taxonomy or dataset in your own research, please cite the ICSE 2026 paper:

```bibtex
@inproceedings{katkhede2026defects4rest,
  title     = {Defects4REST: A Taxonomy of REST API Defects},
  author    = {Katkhede, Pushpak Vijay and others},
  booktitle = {Proceedings of the 48th International Conference on Software Engineering (ICSE)},
  year      = {2026},
  publisher = {ACM/IEEE}
}
```

> Update author list and page numbers once the proceedings entry is finalized.

## Related Work

- [Defects4REST](https://github.com/katkhedepushpak) — the associated benchmark and defect dataset
- ICSE 2026 paper preprint (link TBD)

## Author

Built by [Pushpak Vijay Katkhede](https://katkhedepushpak.github.io) — Software Engineer and MS Computer Science candidate at Oregon State University, with 3+ years of industry experience in backend engineering, cloud infrastructure, and DevOps at IBM.
