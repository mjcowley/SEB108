![SEB108 Data Analysis and Visualisation banner, with charts and maps on a blue background](practicals/images/seb108-banner.png)

# SEB108 Foundations of Data Analysis and Visualisation

Teaching materials for SEB108 at QUT (Faculty of Science). Students learn Python for data analysis, then analyse real river water quality data for our industry partner, the Queensland Government's Water Quality & Investigations team (WQI).

Students reach these materials through the unit's Canvas site. This repository is where they're built and published.

## What's in this repository

| Folder | Contents |
|---|---|
| `practicals/` | Four weekly practicals, built as a website with [Quarto](https://quarto.org) and [quarto-live](https://r-wasm.github.io/quarto-live/). Python runs in the browser, so students don't install anything |
| `practicals/data/` | Practical data, Logan River at Yarrahappini |
| `assessment/` | The Assessment 1 workbook, a Google Colab notebook |
| `data/assessment/` | Assessment data for five Brisbane catchment sites, plus annual loads |

The practicals and the assessment use data from different rivers. Each practical teaches a step of the analysis on the practical data, and students then apply the same step to their own site in the workbook.

## Data

The water quality data comes from WQI's monitoring program, published on the Tahbil Water Quality Data Portal. It's used and redistributed here with WQI's permission.

Attribution wording to come.

## Building the practicals

The practicals site is rebuilt and published automatically whenever changes are pushed to `main` (see `.github/workflows/publish-practicals.yml`).

To preview it locally, install [Quarto](https://quarto.org/docs/get-started/), then run this from the repository folder.

```bash
quarto preview practicals
```

The pages have to be served over the web to run their Python, so opening the HTML files directly won't work.
