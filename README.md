# UKESM fire coupling

## Where we are

| Task                            | Contact | Evaluation                                                 | Name  | Outstanding Issues/Tasks                                                                                                | Expected Date |
|---------------------------------|---------|------------------------------------------------------------|-------|-------------------------------------------------------------------------------------------------------------------------|---------------|
| INFERNO                         | CB      | fireMIP - Burnt area                                       | DK    | Incorrect Trend Introduce Cropland Fragmentation (CB/DK)                                                                |               |
| BGC coupling in 5-pft JULES     | CB      | fireMIP - vegetation fractions                             | DK    | Excessive fire impact of tree cover in some regions Constraining mortality and recovery (veg mortality JPEG - DK/ER/CB) |               |
| BGC coupling in UKESM-JULES     | ?/DK    | fireMIP Plus UM eval below Carbon Conservation checks      | ?     | BGC coupling for 9-PFTS Carbon accounting (issue with TRIFFID 10-day timestep and CC)                                   |               |
| UM Emission coupling            | ?/GF    | fireMIP - Fire C emission Plus others...?                  | DK/RP |                                                                                                                         |               |
| UM lightning ignitions coupling | ?/GF    | Same as above                                              | DK/RP |                                                                                                                         |               |
| Atmos. Chem. coupling           | ?/GF    |                                                            | DK/RP |                                                                                                                         |               |
| UKESM paramterizations          | DK      | ESMval tools? Plus whatever we're using for UKESMv2 tuning | DK    |                                                                                                                         |               |


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


[[embed url=https://docs.google.com/spreadsheets/d/e/2PACX-1vQ5eUFRV4fWk6F4RYIeiXqrl9SM_MEfIvliT2O_vlqPLWaRtRH0n8L9laSD1jPAqazYl6YsBRKogfvw/pubhtml?gid=0&amp]]


#### Physical Model

![INFERNO_Firemip](docs/FireMaps.png "INFERNO performance")

***Add Trend Figure***

<a href="https://docs.google.com/spreadsheets/d/1nSwfbOOgf3Xqd7l70rnaLB82b4_F2w8jkp9YMqg71u4/edit?usp=sharing">![FIRE_benchmark_tab](docs/JULES-INFERNO_fire_benchmark_table.png "Offline fire benchmark scores") </a>

#### BGC impacts

![JULES_BGC_coupling](docs/lifeForm2__res-NaNmodel-S3.png "Veg Fracs without fire")
![JULES_BGC_coupling](docs/lifeForm2__res-NaNmodel-SF3.png "Veg Fracs with fire")

Add Evaluation Table

### Parameterization

#### Cropland fragmentation


#### Veg mortality

## IMOGEN


## UM


## UKESM
