### Google Earth Engine code for Data Fusion of Sentinel-2 and NAIP Optical Imagery for High-Resolution Urban Vegetation Classification in the Los Angeles Megacity. 

0: Impervious surface\
1: Tree (mixed evergreen/deciduous)\
2: Grass (assumed irrigated)\
3: Shrub\
4: Non-photosynthetic vegetation\	
5: Water (masked using MNDWI/NDWI\

EPSG: 4326/WGS84 

# Notes: 
	- Non-urban and shadow regions classified with ESA Sentinel-2 imagery (10-60 m)
	- Urban regions classified with USDA National Agricultural Imagery Program (NAIP) imagery (0.6-1 m)
	- Aggregated 30m pixels are aligned with projection of 2016 NLCD classification 

classified_SoCAB: 1-band 0.6-10m classification of 6 land cover classes across SoCAB
30m_majority_SoCAB: 1-band 30m classification of majority land cover class within each 30m pixel across all of SoCAB 
30m_fractional_SoCAB: 5-band 30m classification of 60cm fractional land cover class within each 30m pixel, where bands correspond to the following labelling (band1 = impervious, band2 = tree, band3 = grass, band4 = shrub, band5 = npv, band6 = water)

SoCAB: Southern California Air Basin 
SB: San Bernardino County
RI: Riverside County
OR: Orange County
LA: Los Angeles County 

A portion of this research was carried out at the Jet Propulsion Laboratory, California Institute of Technology, under a contract with the National Aeronautics and Space Administration. Support from the Earth Science Division OCO-2 program is acknowledged. Copyright 2020. All rights reserved.
