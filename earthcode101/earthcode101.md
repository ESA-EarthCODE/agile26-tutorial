# EarthCODE Summary

EarthCODE is an ESA Earth Observation initiative that supports Open Science practice in Earth System Science. It helps researchers discover, access, reuse, and build on ESA-funded EO research outputs, including data products, workflows, experiments, and documentation.

The practical goal is to make research outputs easier to find, easier to understand, and easier to reuse in reproducible analysis environments.

## What EarthCODE Provides

- A discovery layer through the [Open Science Catalog](https://opensciencedata.esa.int/).
- Structured metadata for projects, products, workflows, experiments, variables, missions, and themes.
- Access links to research outputs such as Zarr, GeoTIFF, NetCDF, Parquet, STAC catalogs, documentation, and code repositories.
- A route from catalog discovery to notebook-based analysis using common Python tools.

## Why It Matters

Earth Observation research often produces valuable outputs that are hard to reuse because metadata, access links, formats, and processing context are scattered across projects. EarthCODE aims to reduce that friction by making outputs more FAIR:

- **Findable**: catalog entries can be searched and filtered by theme, variable, project, mission, region, and keywords.
- **Accessible**: catalog pages point to data assets, documentation, workflows, and source repositories.
- **Interoperable**: cloud-native formats and standards such as STAC, Zarr, and common geospatial metadata make data easier to open with shared tools.
- **Reusable**: provenance, variables, documentation, and workflow links help researchers understand whether a product is suitable for their own analysis.

## Workshop Focus

In this workshop, EarthCODE is the starting point for a practical workflow:

1. Search or browse the Open Science Catalog.
2. Inspect product metadata and access links.
3. Open data in Python using STAC, Xarray, GeoPandas, DuckDB, or related tools.
4. Subset, visualise, and analyse the data in notebooks.
5. Compare examples so the same pattern can be reused for other EarthCODE products.

The aim is not to cover every EarthCODE service. The aim is to leave with a reliable path from catalog discovery to hands-on analysis.
