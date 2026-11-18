# EARTH_01

A neural network study of deforestation and climate risk, presented as a website.

**Live site:** link coming once GitHub Pages is turned on.

## What this project is about

Forests take in a large share of the carbon dioxide that people release, and every hectare cut down weakens that natural defence. At the same time, heatwaves, droughts and floods are becoming more frequent, and some countries are far less prepared for them than others. This project asks two connected questions: where is the planet losing forest, and which countries are most at risk from extreme weather in the years ahead?

**Part 1: tracking forest loss from space.** We train a convolutional neural network (CNN) to recognise forest loss in satellite images of Brazil, Indonesia, the Democratic Republic of the Congo and India. From the area the model finds, we estimate how much carbon each country's forests no longer absorb, and compare our estimates with published figures.

**Part 2: predicting climate risk by country.** We train a recurrent neural network (LSTM) on four decades of weather records together with emissions and social and economic data. It learns to classify each country's extreme-weather risk as low, medium or high. We test it on 2015 to 2024, years it never saw in training. We then run it on climate projections for a moderate and a high-emissions future to show how risk could change by the 2030s.

The results are shown on interactive world maps. Select a country to see its forest loss, its predicted risk, and how the two scenarios compare.

## What this project does not claim

- The forest model learns from an existing global forest map, so it is a fast way to spot change, not a more accurate map.
- Future risk is a projection under stated scenarios, not a forecast of specific events.
- Country averages can hide local extremes, and some countries have gaps in their data. Both are noted on the site.

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
