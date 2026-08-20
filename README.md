# Stellar Catalog Exploration and Clustering

This project explores the HYG stellar catalog with Python and SQLite. It combines data loading, filtering, statistical visualization, feature scaling, KMeans clustering, and two- and three-dimensional views of astronomical catalog data.

## Objective

Investigate relationships among stellar magnitude, luminosity, distance, color index, and spatial position while demonstrating an exploratory workflow that spans SQL, scientific visualization, and introductory machine learning.

## Tools and Technologies

- Python and pandas
- SQL, SQLite, and SQLAlchemy
- Matplotlib, Seaborn, and Plotly
- scikit-learn (`StandardScaler` and `KMeans`)
- Jupyter Notebook

## Workflow and Analysis

1. Load the HYG v4.1 catalog into pandas and a local SQLite database.
2. Query a sample through SQL and inspect the catalog's 119,626 records.
3. Filter magnitude outliers and remove incomplete rows for selected analyses.
4. Visualize distributions, pairwise relationships, correlations, and logarithmic-scale comparisons.
5. Standardize luminosity, distance, and color-index features.
6. Apply three-cluster KMeans as an exploratory segmentation technique.
7. Plot stellar positions in three dimensions with Matplotlib and Plotly.

## Key Results and What This Demonstrates

- The notebook reports a weak Pearson correlation of approximately 0.126 between apparent magnitude and distance in the unfiltered catalog.
- KMeans separates the selected standardized features into three exploratory groups; the clusters are not presented as established astrophysical classifications.
- The project demonstrates large-catalog ingestion, SQL access, missing-value handling, scaling, clustering, and scientific plotting across very different numerical ranges.

## Visualization

![Three-dimensional stellar position plot](3d%20interactive%20plot.png)

## Repository Contents

| Path | Description |
| --- | --- |
| [`HYG star.ipynb`](HYG%20star.ipynb) | Catalog exploration, SQL workflow, clustering, and visualizations |
| [`3d interactive plot.png`](3d%20interactive%20plot.png) | Saved view of the three-dimensional position analysis |

## Viewing and Reproducibility Notes

[View the notebook in nbviewer](https://nbviewer.org/github/Salgadod123/Star-Data-Project/blob/main/HYG%20star.ipynb) if GitHub does not render every plot.

The HYG source CSV is not stored in this repository, and the notebook currently references a local file path. A later reproducibility pass should add a documented download source and configurable data path.
