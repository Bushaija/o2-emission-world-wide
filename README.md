# Population Growth & CO₂ Emissions — Worldwide Analysis

An R / tidyverse data-analysis project examining the relationship between
world population and CO₂ emissions.

## Contents

| File | Description |
|------|-------------|
| `analysis.Rmd` | Full analysis (Tasks 4.1–4.6); knits to `analysis.html`. |
| `report.tex` / `report.pdf` | Short (≤3 page) LaTeX report (Task 4.7). |
| `results_summary.txt` | Headline numbers written out by the knit, quoted by the report. |
| `instruction.md` | Original assignment brief. |

## Data (required, not included)

Download the two CSV files from Kaggle and place them in **this folder**:

1. **World Population Dataset** — https://www.kaggle.com/datasets/iamsouravbanerjee/world-population-dataset
2. **CO2 Emission Around the World** — https://www.kaggle.com/datasets/koustavghosh149/co2-emission-around-the-world

The analysis auto-detects which CSV is which from the column names, so the
exact file names do not matter.

## How to run

From R (packages: `tidyverse`, `janitor`, `scales`, `knitr`, `corrplot`,
`rmarkdown`):

```r
rmarkdown::render("analysis.Rmd")
```

To build the report PDF (requires a LaTeX installation, e.g. MiKTeX/TinyTeX):

```bash
pdflatex report.tex
pdflatex report.tex
```

## Methods implemented

- **4.2 EDA** — variable names, head/tail, data types, shape, duplicate
  removal, missing-value counts, box-plot outlier check, median imputation and
  IQR winsorising.
- **4.3 Projection** — 2030 population via the exponential model `Nₜ = P·e^{rt}`.
- **4.4 Visualisation** — top-10 populous countries (bar), their 1990–2022
  population trend and 1990–2019 CO₂ trend (line, `ggplot2`).
- **4.5 Correlation** — correlation matrix + heatmap for population variables;
  merge on country, scatter / correlation / linear regression of population vs
  CO₂.
- **4.6 Continents** — total 2019 CO₂ per continent with a ranked bar chart.
