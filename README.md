# UKESM fire coupling

## Where we are

Tables Generator
LaTeX Tables
HTML Tables
Text Tables
Markdown Tables
MediaWiki Tables
Contact

 
Markdown Tables Generator 35 
  
 GeneratePut tabs between columnsCompact mode
Result (click "Generate" to refresh) Copy to clipboard
| Task                            | Contact | Evaluation                                                 | Name  | Outstanding Issues/Tasks                                                                                                | Expected Date |
|---------------------------------|---------|------------------------------------------------------------|-------|-------------------------------------------------------------------------------------------------------------------------|---------------|
| INFERNO                         | CB      | fireMIP - Burnt area                                       | DK    | Incorrect Trend Introduce Cropland Fragmentation (CB/DK)                                                                |               |
| BGC coupling in 5-pft JULES     | CB      | fireMIP - vegetation fractions                             | DK    | Excessive fire impact of tree cover in some regions Constraining mortality and recovery (veg mortality JPEG - DK/ER/CB) |               |
| BGC coupling in UKESM-JULES     | ?/DK    | fireMIP Plus UM eval below Carbon Conservation checks      | ?     | BGC coupling for 9-PFTS Carbon accounting (issue with TRIFFID 10-day timestep and CC)                                   |               |
| UM Emission coupling            | ?/GF    | fireMIP - Fire C emission Plus others...?                  | DK/RP |                                                                                                                         |               |
| UM lightning ignitions coupling | ?/GF    | Same as above                                              | DK/RP |                                                                                                                         |               |
| Atmos. Chem. coupling           | ?/GF    |                                                            | DK/RP |                                                                                                                         |               |
| UKESM paramterizations          | DK      | ESMval tools? Plus whatever we're using for UKESMv2 tuning | DK    |                                                                                                                         |               |
You can now import Markdown table code directly using File/Paste table data... dialog.

How to use it?
Using the Table menu set the desired size of the table.
Enter the table data into the table:
select and copy (Ctrl+C) a table from the spreadsheet (e.g. Google Docs, LibreOffice Calc, webpage) and paste it into our editor -- click a cell and press Ctrl+V
or just double click any cell to start editing it's contents -- Tab and Arrow keys can be used to navigate table cells
Adjust text alignment and table borders using the options from the menu and using the toolbar buttons -- formatting is applied to all the selected cells.
Click "Generate" button to see the generated table -- select it and copy to your document.
Markdown tables support
As the official Markdown documentation states, Markdown does not provide any special syntax for tables. Instead it uses HTML <table> syntax. But there exist Markdown syntax extensions which provide additional syntax for creating simple tables.

One of the most popular is Markdown Here — an extension for popular browsers which allows you to easily prepare good-looking e-mails using Markdown syntax.

Similar table syntax is used in the Github Flavored Markdown, in short GFM tables.

Example
GFM Markdown table syntax is quite simple. It does not allow row or cell spanning as well as putting multi-line text in a cell. The first row is always the header followed by an extra line with dashes "-" and optional colons ":" for forcing column alignment.

| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | $1600 |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |
    
© TablesGenerator.com AboutChangelog


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
