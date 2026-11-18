# EARTH_01
Deep learning model predicting country-level climate risk vulnerability andusing satellite imagery to track global deforestation patterns .

# [Project Name]

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

Requires Python 3.11 or newer.

```bash
git clone <this repository's URL>
cd EARTH_01
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Some data sources need a free account (Google Earth Engine, Copernicus, EM-DAT). Store any credentials in a local `.env` file or the provider's standard config file. These are ignored by git and must never be committed.

## Running

Open the notebooks in order, in VS Code or Jupyter. Model training runs on Google Colab's free GPU.

To preview the website locally:

```bash
cd site
python -m http.server 8000
```

Then open http://localhost:8000.

## Data

Raw datasets are too large to store here. Download links, licences and credits are listed in [data/README.md](data/README.md). Cleaned data lives in `data/cleaned/`.

## Team

Graduate Neural Networks course project. Team members: to be added.

## License

To be decided.
