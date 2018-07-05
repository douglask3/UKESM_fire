# UKESM fire coupling

## Where we are

<a href="https://docs.google.com/spreadsheets/d/1nSwfbOOgf3Xqd7l70rnaLB82b4_F2w8jkp9YMqg71u4/edit?usp=sharing">![FIRE_benchmark_tab](docs/TaskList.png "Offline fire benchmark scores") </a>

* Blue = done
* Green = ongoing
* yellow = planned
* red = stuff to figure out

## INFERNO

### Overview

![INFERNO](docs/InfernoSchematic.png "How INFERNO works")

[Mangeon et al., 2016](http://www.geosci-model-dev.net/9/2685/2016/gmd-9-2685-2016.pdf) was developed
A simple, stable parameterization
to diagnose fire occurrence, burned area, and biomass
burning emissions in the context of an Earth system model building upon the fire parameterization proposed by [Pechony
and Shindell 2009](http://onlinelibrary.wiley.com/doi/10.1029/2009JD011927/full).

It is an empirical scheme that uses vapor pressure deficit, precipitation, and soil moisture to diagnose burned area.
Humans only explicitly impact biomass burning through the number of fires. 
Vegetation-dependent average burned area:
0.6, 1.4, and 1.2 km2
for fires in trees, grasses, and shrubs,
respectively. 

### Offline Evaluation


#### Physical Model

![INFERNO_Firemip](docs/FireMaps.png "INFERNO performance")

***Add Trend Figure***

<a href="https://docs.google.com/spreadsheets/d/1nSwfbOOgf3Xqd7l70rnaLB82b4_F2w8jkp9YMqg71u4/edit?usp=sharing">![FIRE_benchmark_tab](docs/JULES-INFERNO_fire_benchmark_table.png "Offline fire benchmark scores") </a>

#### BGC impacts

![JULES_BGC_coupling](docs/lifeForm2__res-NaNmodel-S3.png "Veg Fracs without fire")
![JULES_BGC_coupling](docs/lifeForm2__res-NaNmodel-SF3.png "Veg Fracs with fire")

<a href="https://docs.google.com/spreadsheets/d/1nSwfbOOgf3Xqd7l70rnaLB82b4_F2w8jkp9YMqg71u4/edit?usp=sharing">![FIRE_benchmark_tab](docs/JULES-INFERNO_vegFrac_benchmark_table.png "Offline veg frac benchmark scores") </a>


### Parameterization

#### Cropland fragmentation

* Implement cropland fragmentation on burnt area based on Kelley et al. in prep, using "suppression index" curve:
![Limitation Curves](docs/limLines--FALSE-FALSE-.png "Kelley et al. in prep")

* Veg-dependent average fire size re-scaled against GFED4s
* Impact on offline INFERNO:

![INFERNO fragmentation](docs/fire_opt.png "Tile optimization")

* Needs re-benchmarking



#### Veg mortality

Vegetation mortality (inc. fire, generic and land use exclusion) and vegetation recovery rate are being constrained as part of the veg distribution JULES PEG:

* <a href="https://docs.google.com/document/d/1J2eMRyYfYdrsI8L5nwVVPRFVVW-TOsy5r8hLdefNEy8/edit?usp=sharing">Veg mortality JPEG</a>
* <a href="https://docs.google.com/document/d/1uS7Nks2N3GOsp_q8eeHcVF6YR-0hj2Uu08RwcBC7yTg/edit?usp=sharing">Mortality optimization</a>

