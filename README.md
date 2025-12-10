# Anomaly Detection POC — hack2025 (Binder-ready)

This repo contains a Binder-ready notebook that generates **synthetic time-series** data and demonstrates anomaly detection using **Z-score** and **Isolation Forest**. It also includes a **Streamlit app** to interactively visualize anomalies in Binder via `jupyter-server-proxy`.

## Quick Launch (replace `<YOUR_GH_USER>`)
- **JupyterLab**: https://mybinder.org/v2/gh/<YOUR_GH_USER>/hack2025/HEAD?labpath=notebook.ipynb
- **Classic Jupyter**: https://mybinder.org/v2/gh/<YOUR_GH_USER>/hack2025/HEAD?filepath=notebook.ipynb

**Badge:**

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<YOUR_GH_USER>/hack2025/HEAD?labpath=notebook.ipynb)

## What’s inside
- `notebook.ipynb` — step-by-step demo (Sections 1–8)
- `requirements.txt` — minimal libs + `streamlit`, `jupyter-server-proxy`, `altair`
- `runtime.txt` — pins Python for Binder stability

## Streamlit in Binder
The notebook creates `data/anomaly_results.csv` and writes `streamlit_app.py`. Run **Section 8** to start Streamlit on **port 8501** and open:

- `/proxy/8501/` (relative link in Binder)

> If you get 404 initially, wait 10–20 seconds and refresh.

## Notes
- Optional LSTM Autoencoder is _not_ installed by default. You can add a cell to install `torch` if needed.
- Binder caches builds by git ref. If you update files and don’t see changes, push a new commit and re-open Binder, or use a tag (e.g., `v1`).

Generated: 2025-12-10T21:25:19.610827Z
