# Satellite Image Handling and Interpretation: A Study of Surat, Gujarat

**Geospatial Analysis | Remote Sensing | ArcGIS Pro**

## Project Overview

This project focuses on the application of multispectral satellite imagery for image preprocessing, spectral signature analysis and visual interpretation of land-cover features in Surat, Gujarat.

The study uses Landsat 9 Collection 2 Level-1 and Level-2 imagery, together with Sentinel-2 Level-2A imagery. The practical analysis was carried out using ArcGIS Pro and involved satellite data acquisition, preparation of an Area of Interest (AOI), reflectance conversion, image resampling, spectral analysis and visual interpretation.

A selected 1 km × 1 km window within Surat was digitised to identify and estimate the spatial distribution of different land-cover classes.

## Objectives

- Examine Landsat 9 and Sentinel-2 satellite imagery and their sensor characteristics.
- Perform satellite image preprocessing, including reflectance conversion, band stacking, clipping and resampling.
- Examine the spectral characteristics of selected land-cover classes using multispectral reflectance values.
- Interpret Natural Colour, Colour Infrared and Shortwave Infrared composites.
- Digitise and estimate the area distribution of selected land-cover classes.
- Prepare a thematic land-cover map using satellite imagery and GIS-based interpretation.

## Data Sources

| Satellite | Product | Data source |
|---|---|---|
| Landsat 9 | Collection 2 Level-1 and Level-2 | USGS EarthExplorer |
| Sentinel-2 | Level-2A | Copernicus Data Space Ecosystem |

**Acquisition dates:**
- Landsat 9: 7 May 2026
- Sentinel-2A: 15 October 2026

The datasets were acquired on different dates, which is relevant when interpreting differences between the imagery.

## Study Area

- **Location:** Surat, Gujarat, India
- **Area of Interest:** Approximately 60.85 km²
- **Coordinate Reference System:** WGS 1984 UTM Zone 43N
- **EPSG Code:** 32643
- **Interpretation window:** 1 km × 1 km

## Methodology

The analysis was carried out through the following stages:

### 1. Satellite Image Preprocessing
- Acquisition and organisation of Landsat 9 and Sentinel-2 imagery.
- Preparation of the Area of Interest.
- Conversion of Landsat Level-1 digital numbers into Top of Atmosphere (TOA) reflectance using metadata coefficients.
- Conversion of Landsat Level-2 bands into surface reflectance.
- Clipping and band stacking of selected imagery.

### 2. Reflectance Analysis
TOA reflectance values from Landsat Level-1 imagery were calculated and compared with corresponding Level-2 surface reflectance values for blue (B2) and red (B4) bands across water, vegetation and built-up sample locations.

### 3. Sentinel-2 Resampling
Sentinel-2 Band 11 was resampled using:
- Nearest Neighbour
- Bilinear Interpolation

The outputs were compared along a transect to examine differences in pixel values and spatial appearance.

### 4. Spectral Signature Analysis
Five representative land-cover categories were examined using six Landsat 9 Level-2 bands:

- Water
- Dense vegetation
- Built-up
- Bare ground
- Tidal mudflat

A 3 × 3-pixel neighbourhood was used to obtain mean reflectance values across bands B2 to B7.

### 5. Visual Interpretation and Land-Cover Mapping
Three multispectral composites were prepared:

- Natural Colour Composite (4-3-2)
- Colour Infrared Composite (5-4-3)
- SWIR Composite (7-6-4)

A selected 1 km × 1 km window was manually digitised using the Colour Infrared composite as the primary visual reference.

## Key Findings

- The TOA and surface reflectance comparison showed differences across the selected land-cover categories and spectral bands.
- Nearest Neighbour and Bilinear Interpolation produced different pixel values, while retaining a broadly similar spatial pattern.
- The resampling comparison showed a mean absolute difference of 35.58 and a correlation of approximately 0.996.
- The mean positional offset between selected Landsat and Sentinel control points was approximately 7.24 m, with an RMSE of approximately 7.53 m.
- Water showed relatively low reflectance across the six selected bands.
- SWIR1 (B6) provided the widest reflectance range among the five sampled land-cover categories.

## Land-Cover Mapping Results

The selected 1 km × 1 km interpretation window covered 100 hectares.

Nine polygons were digitised, covering a total 52.386 hectares.
and-cover class

Area (ha)

Agricultural land

8.097

Barren land

2.970

Built-up

19.383

Dense vegetation

19.733

Fallow land

2.203

Total digitised area

52.386

 The mapped polygons represent selected, visually distinguishable land-cover patches rather than a complete classification of the interpretation window.

Limitations

Landsat 9 and Sentinel-2 imagery were acquired on different dates.

Land-cover interpretation was based on visual interpretation of selected satellite composites.

Only 52.386 hectares of the 100-hectare interpretation window were digitised.

The findings are based on the selected study area and representative sample locations.

Tools Used

ArcGIS Pro

Landsat 9 multispectral imagery

Sentinel-2 multispectral imagery

Raster Calculator

Composite Bands

Nearest Neighbour and Bilinear Resampling

Spectral signature analysis

GIS-based digitisation and visual interpretation



Large satellite imagery, raster datasets and geodatabases may be maintained separately due to their file sizes. Their sources and access information will be documented where available.

## Project Map

The following map presents the land-use/land-cover classification of the selected study area in Surat, Gujarat, developed through visual interpretation and manual digitisation of Landsat 9 imagery.

**Land-use/Land-cover Classification Map**

[View the full-resolution map](maps/surat_land_cover_classification_map.png)

## Author

Kaustubh Nagrare

Undergraduate Student – Analytics & Sustainability Studies
Tata Institute of Social Sciences (TISS), Mumbai
