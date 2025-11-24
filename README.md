# HEPData export for CMS SMP-22-009

This repo contains a small workflow to convert CMS ROOT histograms for the
SMP-22-009 analysis into HEPData YAML tables and a submission tarball.

## Layout

- `HEPdata.ipynb` – Jupyter notebook with the export script.
- `input/` – place the ROOT file here (e.g. `ZNuNuGPrePostFitPostFitEBEE.root`).
- `hepdata_output/` – auto-generated YAML tables and `submission.yaml`.
- `submission.tar.gz` – tarball produced by `hepdata_lib.create_files`, ready to
  upload to HEPData.

## Requirements

- Python 3
- ROOT (PyROOT)
- `hepdata-lib`
- `PyYAML`

Install Python deps, e.g.

```bash
pip install hepdata-lib pyyaml
