# DeepSky: Planets Data

Website: [https://lawrencefmm.github.io/DeepSky/](https://lawrencefmm.github.io/DeepSky/)u

This is a collection of data on the planets in our solar system. The data is stored in a JSON file and is used to
generate the content on the [DeepSky](https://lawrencefmm.github.io/DeepSky/) website.

## Resources
    - [Gaia DR3 Catalog](www.cosmos.esa.int/web/gaia/data-release-3)
    - [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/)

## Data

For each exoplanet, we computate for all stars the magnitude and only stored stars with
apparent magnitude less than 7.0. The x, y, z also take into account the magnitude, to give a sensation of brightness.

To improve the performance, we used PostgresSQL to manipulate most part of the data, and also used C++
to process the remaining data. After doing some optimizations, like removing stars that are not visible
for all/most planets.
