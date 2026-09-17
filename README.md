# Full Stack Academy RAG Chatbot (Streamlit)

## Setup
```bash
# Create a virtual environment
python -m venv .venv

# Activate it
# macOS/Linux:
# source .venv/bin/activate
# Windows PowerShell:
# .\.venv\Scripts\Activate.ps1
# Windows cmd:
# .venv\Scripts\activate.bat

# Install dependencies
pip install -r requirements.txt

# Create your local secrets file and paste your Groq key
# macOS/Linux:
# cp .streamlit/secrets.toml.example .streamlit/secrets.toml
# Windows PowerShell:
# Copy-Item .streamlit/secrets.toml.example .streamlit/secrets.toml
```

Put your PDFs (what was `/content/fsa_pds` in Colab) into the `pdfs/` folder.

## Run
```bash
streamlit run app.py
```

## Deploy to Streamlit Community Cloud
1. Push this folder to GitHub (secrets.toml is git-ignored).
2. Create an app at share.streamlit.io pointing to `app.py`.
3. In the app's **Settings → Secrets**, paste: `GROQ_API_KEY = "gsk_..."`

