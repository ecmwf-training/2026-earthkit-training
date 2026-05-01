# earthkit-transforms

<a href="https://earthkit-transforms.readthedocs.io/en/release-1.0.0rc0/" target="_blank" rel="noopener">
	<picture>
		<source srcset="https://raw.githubusercontent.com/ecmwf/logos/refs/heads/main/logos/earthkit/earthkit-transforms-dark.svg" media="(prefers-color-scheme: dark)">
		<source srcset="https://raw.githubusercontent.com/ecmwf/logos/refs/heads/main/logos/earthkit/earthkit-transforms-light.svg" media="(prefers-color-scheme: light)">
		<img src="https://raw.githubusercontent.com/ecmwf/logos/refs/heads/main/logos/earthkit/earthkit-transforms-light.svg" alt="earthkit-transforms logo" style="width: 100%; max-width: 400px; display: block; margin: 0 auto;">
	</picture>
</a>

**earthkit-transforms** is a simple to use library of software tools to support people
working with climate and meteorology data. It is made of sub-modules designed
for  transformations of data in specific domains.
For example, the temporal module contains methods for aggregation and
statistics analysis accross time dimensions/coordinates.

Under the hood, **earthkit-transforms** uses common python libraries such as `xarray`, `pandas` and
`geopandas` to perform the various computations.
The interface is designed such that it can work with both CPU and GPU data-objects,
however working with GPU data-objects is beyond the scope of this training.


---
<!-- 
::::{grid} 1 1 3 3


:::{card}
:header: <div style="text-align:center;"><b>Daily and monthly means</b></div>
:link: ./01-calculate-and-plot-daily-monthly-mean-data
Calculate and plot monthly and daily statistics from hourly ERA5 data.
:::

:::{card}
:header: <div style="text-align:center;"><b>Country level aggregations</b></div>
:link: ./02-reduce-era5-data-over-geometries.ipynb
Calculate country level aggregations by combining gridded data with geometry data.
:::

:::{card}
:header: <div style="text-align:center;"><b>Climatologies</b></div>
:link: ./03-calculate-and-plot-climatologies
Calculate and plot monthly climatologies of ERA5 data.
:::

::::
 -->
