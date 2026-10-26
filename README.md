# EARTH_01
Deep learning model predicting country-level climate risk vulnerability andusing satellite imagery to track global deforestation patterns .



A neural network study of deforestation and country-level climate risk, presented as a static website.

**Live site:** [link once GitHub Pages is enabled]

## Repository layout

```
.
├── data/
│   ├── raw/          # not tracked; see data/README.md for download links
│   └── cleaned/      # small, processed files used by the models
├── notebooks/        # data preparation, training and evaluation
├── outputs/          # results exported for the website (JSON)
├── site/             # static website served by GitHub Pages
├── requirements.txt
└── README.md
```

## Setup

Requires Python [version].

```bash
git clone https://github.com/[owner]/[repo].git
cd [repo]
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Some data sources need an account and an API key. Store credentials in a local `.env` file or the provider's standard config file. These are ignored by git and must never be committed.

## Running

```bash
# Open the notebooks in order, in VS Code or Jupyter
jupyter lab notebooks/
```

To preview the website locally:

```bash
cd site
python -m http.server 8000
```

Then open http://localhost:8000.

## Data

Raw datasets are too large to store here. Download links and source credits are listed in `data/README.md`. Cleaned data lives in `data/cleaned/`.

## License

[To be decided]
