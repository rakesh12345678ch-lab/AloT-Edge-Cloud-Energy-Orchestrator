# HCL Smart Energy Dashboard

A Streamlit software prototype for SME energy monitoring and optimisation.

## Important project note

This version uses **simulated telemetry**. It does not yet read actual values from an ESP32, Schneider EM6459 meter, PZEM sensor, Delta PLC, or LoRa network. Do not use its values for electrical protection, billing, or operational control.

## Run locally

Python 3.10 or newer is recommended.

```bash
python -m pip install -r requirements.txt
streamlit run app.py
```

## Deploy on Streamlit Community Cloud

1. Extract this ZIP file on your computer.
2. Create a **public** GitHub repository.
3. Upload `app.py`, `requirements.txt`, and `README.md` to the repository's root (not inside another folder).
4. Open https://share.streamlit.io/ and sign in with GitHub.
5. Choose **Create app**, select your repository and `main` branch.
6. Set **Main file path** to `app.py`, then click **Deploy**.
7. Share the `*.streamlit.app` URL after deployment succeeds.

The dashboard generates a new sample when you click **Generate new telemetry**. Saved files on Community Cloud should be treated as temporary; download any history you need to keep.
