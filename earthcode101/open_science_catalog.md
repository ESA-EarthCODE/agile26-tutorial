# EarthCODE Open Science Catalog Walkthrough

[Open the EarthCODE Open Science Catalog](https://opensciencedata.esa.int/)

The Open Science Catalog is the main discovery interface for EarthCODE resources. It brings together ESA-funded Earth Observation research outputs such as projects, products, workflows, experiments, variables, missions, and thematic groupings.

For this workshop, focus on three questions:

1. What research output is available?
2. What metadata explains whether it is reusable?
3. Where is the data or workflow access point?

## Browse the Catalog

Start from the landing page and explore the main catalog groupings:

- **Themes** group resources by Earth science topic.
- **Projects** connect products to ESA-funded research activities.
- **Products** describe data products, their spatial and temporal extent, variables, documentation, and access links.
- **Workflows and experiments** describe reusable methods and processing steps where available.

When opening a product page, look for the title, abstract, temporal extent, spatial coverage, variables, project links, and source metadata. These fields help you decide whether the product is suitable for reuse before opening the data itself.

## Search and Filter

Use the catalog search page when you already have a research theme, location, project, mission, or variable in mind.

Useful filters during the workshop:

- Theme, for example land or polar science.
- Variable, for example burned area, ice, vegetation, or atmosphere-related terms.
- Project, when a dataset is linked to a specific ESA research activity.
- Free-text search, when you know only a keyword.
- Map geometry, when you want products intersecting a region of interest.

The result count changes as filters are applied. Open promising products in new tabs so you can compare metadata and access options.

## Find Access Information

Product pages may point to several kinds of resources:

- A source data URL or external repository.
- A STAC catalog or collection.
- Zarr, GeoTIFF, NetCDF, Parquet, or other analysis-ready assets.
- Documentation, publications, or project pages.

For notebook work, the most useful access points are STAC links and direct cloud-native data assets such as Zarr stores or Parquet files. The STAC and data access notebook in the next section shows how these links become Python objects that can be opened with tools such as `pystac-client`, `xarray`, `geopandas`, and `duckdb`.

## Workshop Examples

During the walkthrough, use the catalog to locate examples such as:

- SEASFIRE Cube, a global fire modelling dataset used in the Pangeo examples.
- Antarctica analysis-ready data cubes, which demonstrate how FAIRified EO data can be packaged for direct reuse.
- Other EarthCODE-hosted products that expose cloud-native access URLs.

The goal is not to memorise the catalog structure. The goal is to develop the habit of checking metadata, understanding provenance, finding the access link, and moving from discovery to analysis in a notebook.
