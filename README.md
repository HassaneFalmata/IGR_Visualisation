# IGR_Visualisation
Baby names project

## Introduction

This notebook demonstrates how to create choropleth maps using the Altair library. The example uses a large dataset of first names in France from 1900 to 2019, broken down by department.

## Contents

The notebook covers the following steps:
1. Importing the necessary libraries.
2. Read first name data from a CSV file.
3. Load geographic data for French departments using `geopandas`.
4. Merge first name data with geographic data.
5. Creation and visualization of choropleth maps to analyze the distribution of first names.

## Libraries used

The notebook uses the following libraries:
- `altair`: to create interactive visualizations.
- `pandas`: to manipulate tabular data.
- `geopandas`: for working with geographic data.

## Instructions

**Library import**
   python
   import altair as alt
   import pandas as pd
   import geopandas as gpd
   ```

**Reading first-name data**
   First name data is read from a CSV file with a `;` separator.

**Geographic data loading**
   Geographic data for French departments are loaded from a `geojson` file provided by [Grégoire David](https://gregoiredavid.fr).

**Data merging**
   First name data and geographic data are merged using a `right-merge` to ensure that the data structure remains a `geopandas` dataframe.

**Visualization**
   A choropleth map is created to show the distribution of a specific first name over a given period. For example, the distribution of the first name "Lucien" over the last 120 years in mainland France.

## References

- [INSEE](http://www.insee.fr/fr/methodes/nomenclatures/cog/telechargement.asp)
- [IGN](https://geoservices.ign.fr/adminexpress)
