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

Add Trend Figure

Add Evaluation table

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

<table>
    <tr>
        <td><style type="text/css"><!--td {border: 1px solid #ccc;}br {mso-data-placement:same-cell;}--></style><table xmlns="http://www.w3.org/1999/xhtml" cellspacing="0" cellpadding="0" dir="ltr" border="1" style="table-layout: fixed; font-size: 10pt; font-family: arial, sans, sans-serif; width: 0px; border-width: initial; border-style: none; border-color: initial;"><colgroup><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"><col width="100"></colgroup><tbody><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;comparison&quot;}"><div style="max-height:65px">comparison</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;observations&quot;}"><div style="max-height:65px">observations</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;time period&quot;}"><div style="max-height:65px">time period</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;metirc&quot;}"><div style="max-height:65px">metirc</td>
        <td style="border-right: 3px double rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;step&quot;}"><div style="max-height:65px">step</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" colspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;null models&quot;}">null models</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" colspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;jules-inferno&quot;}">jules-inferno</td>
    </tr><tr style="height:44px;">        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;median&quot;}">median</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;mean&quot;}">mean</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;randomly resampled&quot;}">randomly resampled</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;sf2 - fire&quot;}">sf2 - fire</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; font-weight: bold; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;sf3 -land use and fire&quot;}">sf3 -land use and fire</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="12" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;spatial burnt area&quot;}"><div style="max-height:252px">spatial burnt area</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;meris&quot;}"><div style="max-height:63px">meris</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;2006-2009&quot;}"><div style="max-height:63px">2006-2009</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="12" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;nme&quot;}"><div style="max-height:252px">nme</td>
        <td style="border-right:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:bottom;text-align:right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.71}"><div style="max-height:63px">0.71</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.13 +/- 0.072&quot;}"><div style="max-height:63px">1.13 +/- 0.072</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.95}">0.95</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.95}">0.95</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.92}">0.92</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.92}">0.92</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.93}">0.93</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.93}">0.93</td>
    </tr><tr style="height:21px;">        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;mcd45&quot;}"><div style="max-height:63px">mcd45</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;2001-2008&quot;}"><div style="max-height:63px">2001-2008</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.72}"><div style="max-height:63px">0.72</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.15 +/-0.0028&quot;}"><div style="max-height:63px">1.15 +/-0.0028</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.91}">0.91</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.91}">0.91</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.87}">0.87</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.87}">0.87</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.88}">0.88</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.88}">0.88</td>
    </tr><tr style="height:21px;">        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4&quot;}"><div style="max-height:63px">gfed4</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}"><div style="max-height:63px">1997-2014</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.72}"><div style="max-height:63px">0.72</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.14 +/- 0.0066&quot;}"><div style="max-height:63px">1.14 +/- 0.0066</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.84}">0.84</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.84}">0.84</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.8}">0.8</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.8}">0.8</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.84}">0.84</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.84}">0.84</td>
    </tr><tr style="height:21px;">        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4s&quot;}"><div style="max-height:63px">gfed4s</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}"><div style="max-height:63px">1997-2014</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.75}"><div style="max-height:63px">0.75</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.19 +/- 0.023&quot;}"><div style="max-height:63px">1.19 +/- 0.023</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.8}">0.8</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.8}">0.8</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.79}">0.79</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.79}">0.79</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.87}">0.87</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.86}">0.86</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="6" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;spatial trend in burnt area&quot;}"><div style="max-height:126px">spatial trend in burnt area</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4&quot;}"><div style="max-height:63px">gfed4</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}"><div style="max-height:63px">1997-2014</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="6" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;nme&quot;}"><div style="max-height:126px">nme</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.94}"><div style="max-height:63px">0.94</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.38 +/- 0.012&quot;}"><div style="max-height:63px">1.38 +/- 0.012</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.03}">2.03</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.04}">2.04</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.04}">2.04</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.04}">2.04</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.43}">1.43</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.43}">1.43</td>
    </tr><tr style="height:21px;">        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4s&quot;}"><div style="max-height:63px">gfed4s</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}"><div style="max-height:63px">1997-2014</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.98}"><div style="max-height:63px">0.98</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.37 +/- 0.014&quot;}"><div style="max-height:63px">1.37 +/- 0.014</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.54}">1.54</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.55}">1.55</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.54}">1.54</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.55}">1.55</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(255, 229, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.29}">1.29</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(255, 229, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.29}">1.29</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;seasonal conservation&quot;}"><div style="max-height:42px">seasonal conservation</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4&quot;}">gfed4</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}">1997-2014</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;nme&quot;}"><div style="max-height:42px">nme</td>
        <td style="border-right:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:middle;"></td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.37 +/- 0.023&quot;}">1.37 +/- 0.023</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.33}">2.33</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2.32}">2.32</td>
    </tr><tr style="height:21px;">        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4s&quot;}">gfed4s</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}">1997-2014</td>
        <td style="border-right:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:middle;"></td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.99}">0.99</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.38 +/- 0.013&quot;}">1.38 +/- 0.013</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.64}">1.64</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.64}">1.64</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;seasonal phase&quot;}"><div style="max-height:42px">seasonal phase</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4&quot;}">gfed4</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}">1997-2014</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="2" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;mpd&quot;}"><div style="max-height:42px">mpd</td>
        <td style="border-right:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:middle;"></td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.53}">0.53</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.48}">0.48</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;0.49 +/- 0.00042&quot;}">0.49 +/- 0.00042</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(164, 194, 244); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.37}">0.37</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(164, 194, 244); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.37}">0.37</td>
    </tr><tr style="height:21px;">        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfed4s&quot;}">gfed4s</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1997-2014&quot;}">1997-2014</td>
        <td style="border-right: 3px double rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle;"></td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.51}">0.51</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.49}">0.49</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;0.49 +/- 0.00098&quot;}">0.49 +/- 0.00098</td>
        <td style="border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(159, 197, 232); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.35}">0.35</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom-style: dashed; border-bottom-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(159, 197, 232); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.35}">0.35</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;spatial fire carbon emissions&quot;}"><div style="max-height:63px">spatial fire carbon emissions</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="5" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;gfas&quot;}"><div style="max-height:105px">gfas</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="5" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;2000-2009&quot;}"><div style="max-height:105px">2000-2009</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="5" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;nme&quot;}"><div style="max-height:105px">nme</td>
        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.78}"><div style="max-height:63px">0.78</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" rowspan="3" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}"><div style="max-height:63px">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" rowspan="3" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.21 +/- 0.0032&quot;}"><div style="max-height:63px">1.21 +/- 0.0032</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(164, 194, 244); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.77}">0.77</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(164, 194, 244); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.76}">0.76</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.89}">0.89</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(182, 215, 168); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.9}">0.9</td>
    </tr><tr style="height:21px;">        <td style="border-right: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(255, 229, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.02}">1.02</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(255, 229, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.02}">1.02</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;seasonal concentration fire carbon&quot;}">seasonal concentration fire carbon</td>
        <td style="border-right:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:middle;"></td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;1.36 +/- 0.00029&quot;}">1.36 +/- 0.00029</td>
        <td style="overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.64}">1.64</td>
        <td style="border-right-color: rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(234, 153, 153); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1.64}">1.64</td>
    </tr><tr style="height:21px;">        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;seasonal phase fire carbon&quot;}">seasonal phase fire carbon</td>
        <td style="border-right:3px double #000000;border-bottom:3px double #000000;overflow:hidden;padding:2px 3px 2px 3px;vertical-align:middle;"></td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.47}">0.47</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.56}">0.56</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; word-wrap: break-word;" data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;0.47 +/-0.00087&quot;}">0.47 +/-0.00087</td>
        <td style="border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(159, 197, 232); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.44}">0.44</td>
        <td style="border-right-color: rgb(0, 0, 0); border-bottom: 3px double rgb(0, 0, 0); overflow: hidden; padding: 2px 3px; vertical-align: middle; background-color: rgb(159, 197, 232); word-wrap: break-word; text-align: right;" data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:0.44}">0.44</td>
    </tr></tbody></table></td>
    </tr>
</table>
