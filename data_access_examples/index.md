# Accessing Data on EarthCODE Examples

This section gives you additional examples to explore after the guided burnt forest area case study. The notebooks show common access patterns for EarthCODE-hosted research data products, especially Zarr and Parquet assets opened directly from object storage.

Use these notebooks as patterns: identify the dataset URL or catalog item, open it with the appropriate Python library, inspect dimensions and variables, then subset or visualise the data for your research question.

## Recommended During the Workshop

- [SEASFIRE data cube](<./seasfire/1. pangeo_on_EarthCODE_parallel.ipynb>)
  Opens a fire-focused Zarr data cube with Xarray, uses Dask-backed arrays, subsets by area and time, and connects the catalog discovery workflow to the burnt-area case study.

- [Access Antarctica Data](./antarctic-cubes/access_and_viz.ipynb)
  Opens multiple Antarctica analysis-ready Zarr cubes, merges them into a single Xarray view, subsets an ice shelf region, and visualises basal melt and calving-front variables.

## More Direct Zarr Examples

- [SEN4Amazonas](./sen4amazonas/sen4amazonas.ipynb)
  Opens a tree-cover-change Zarr cube, selects a small Amazon region, computes the subset, and visualises time-varying forest change.

- [SMART-CH4](./smart-ch4/access.ipynb)
  Opens a methane isotope signal Zarr dataset and plots selected variables for quick inspection.

- [WAPOSAL](./waposal/access.ipynb)
  Opens an altimetry-style Zarr product, inspects trajectory metadata, and plots a selected track on a map.

- [ARCEME](./arceme/access_arceme.ipynb)
  Opens an ARCEME Zarr data cube directly from object storage and inspects its dataset structure.

- [AGRICEM](./agricem/access.ipynb)
  Opens an agriculture-focused Zarr data cube and plots a selected band/time slice.

## Parquet and Tabular-Geospatial Examples

- [Lightning2EarthCARE data access](./lightning2earthcare/data_access.ipynb)
  Demonstrates Parquet access with GeoPandas and DuckDB, including spatial and column filtering.

- [Lightning2EarthCARE visualisation](./lightning2earthcare/data_visualization.ipynb)
  Visualises lightning observations and EarthCARE-related products. Some authenticated EarthCARE product cells depend on a local helper module and may need instructor setup before running end-to-end.

## What to Compare

Across the examples, look for these recurring steps:

- Where the data URL or catalog entry comes from.
- Whether the data opens with `xarray`, `geopandas`, or `duckdb`.
- Which operations stay lazy and which trigger computation.
- How small spatial or temporal subsets make large remote datasets practical to explore.
