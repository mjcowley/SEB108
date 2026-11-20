![SEB108 Data Analysis and Visualisation banner, with charts and maps on a blue background](practicals/images/seb108-banner.png)

# SEB108 Foundations of Data Analysis and Visualisation

Teaching materials for SEB108 at QUT (School of Chemistry and Physics). Students learn Python for data analysis, then analyse real river water quality data for our industry partner, the Queensland Government's Water Quality & Investigations team (WQI).

## For students

There are two places you'll work, and they're kept separate on purpose.

| What | Where | Do you hand it in? |
|---|---|---|
| Practicals P1 to P4 | The [SEB108 practicals site](https://mjcowley.github.io/SEB108/). Python runs in your browser, so there's nothing to install or save. | No |
| Assessment 1 workbook | A Google Colab notebook. Open it from the **Open in Colab** button on Canvas. | Yes |

When the workbook opens in Colab, go straight to **File > Save a copy in Drive** and work in your copy. If you skip this, your changes won't be saved.

Everything else, including due dates and how check-offs work, is on Canvas.

## What's in this repository

| Folder | Contents |
|---|---|
| `practicals/` | The practicals website, written in [Quarto](https://quarto.org) with [quarto-live](https://r-wasm.github.io/quarto-live/) |
| `practicals/data/` | Practical data, Logan River at Yarrahappini |
| `assessment/` | The Assessment 1 workbook (Colab notebook) |
| `data/assessment/` | Assessment data, five Brisbane catchment sites, plus annual loads |

## Data

The water quality data comes from WQI's monitoring program, published on the [Tahbil Water Quality Data Portal](https://apps.des.qld.gov.au/water-data-portal/about). It's used and redistributed here with WQI's permission.

Attribution wording to come.

## Building the practicals site

The site is rebuilt and published to GitHub Pages automatically whenever changes are pushed to `main` (see `.github/workflows/publish-practicals.yml`).

To preview it on your own computer, install [Quarto](https://quarto.org/docs/get-started/), then run this from the repository folder.

```bash
quarto preview practicals
```

The pages need to be served over the web to run their Python, so opening the HTML files directly won't work.
