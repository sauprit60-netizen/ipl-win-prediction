# IPL Victory Predictor — Streamlit Deployment

This repository contains a Streamlit app that predicts IPL match win probabilities using a pre-trained model.

Files to keep in the repo:
- `main.py` — the Streamlit app (entrypoint)
- `pipe.pkl` — the trained model pipeline
- `background.jpg` — background image used by the app
- `requirements.txt` — Python dependencies

Quick local run

```bash
pip install -r requirements.txt
streamlit run main.py
```

Deploy to Streamlit Cloud

1. Push this repository to GitHub (public or private).
2. Go to https://share.streamlit.io and sign in with GitHub.
3. Click **New app** → choose your repository, branch, and set the **File path** to `main.py`.
4. Click **Deploy**. Streamlit Cloud will install `requirements.txt` and run `streamlit run main.py`.

Notes
- Ensure `pipe.pkl` and `background.jpg` are included in the repo root when you push to GitHub.
- If your model requires a specific `scikit-learn` version, keep it pinned in `requirements.txt`.
- To change the app file name, update the **File path** in the Streamlit Cloud deploy UI.

If you want, I can:
- run a quick local test command for you to try, or
- create a small `.github/workflows` CI to validate builds before deploying.
