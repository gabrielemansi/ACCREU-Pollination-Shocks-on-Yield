# ACCREU_Pollination_Shocks_on_European_Crop_Yields_Dataset
This public folder contains NUTS 3-level datasets describing projected crop yields shocks associated with changes in pollination services. The datasets provide yields shocks for 104 crops by NUTS 3 region in the EU, year and scenario, under the IIASA pollination scenarios.

## Citation

> Campoleoni Mansi, G.A. (2026). Pollination Shocks on European Crop Yields. [Dataset] (Version 1.0). Zenodo. DOI. 10.5281/zenodo.23529106
> Link : https://zenodo.org/records/23529106

# Authors: 
G.A. Campoleoni Mansi, CMCC Foundation (gabriele.mansi@cmcc.it)

Produced within: ACCREU (Assessing Climate Change Risk in EUrope), Horizon Europe
Version: 1.0 (2026)

## Summary

This dataset contains projected pollination shocks on crop yields, i.e. changes in crop yields due to projected changes in pollination services in the EU. 
All `<SCENARIO>_<YEAR>` values are percentage changes in crop yield relative to 2020: values for 2020 are 0 and negative values are yield losses on 2020 cropland area. 

The dataset supports analysis of climate change impacts on crop yields through pollination services at European regional (NUTS 3) level. It was produced by the CMCC Foundation, in collaboration with IIASA, in the context of the ACCREU project.

Shocks are provided for 104 crops by NUTS 3 region and year (2020–2080, 5-year steps), under the IIASA-CLIM pollination scenarios.

The IIASA-CLIM scenarios are based on the IIASA external analysis of habitat suitability under climate and land-use scenarios from ACCREU deliverable D2.4.1 (Gerber, Palazzo et al., 2025), 
and in particular on Gerber (2026, Dataset ACCREU D2.4). 
The methodology for crop yields impact assesment is described in the ACCREU documentation (GA No. 101081358, HORIZON-CL5-2022-D1-07-two-stage), Deliverable D4.1 Section 3.3 "Biodiversity impacts based on pollination services".


# Source data and documentation:
The underlying pollination data, habitat suitability scenarios and methodology are documented in the associated 
# ACCREU deliverables 
> Deliverable D 4.1, Section 3.3 Biodiversity impacts based on pollination services. ACCREU – Assessing Climate Change Risk in EUrope.
> Deliverable D2.4. ACCREU – Assessing Climate Change Risk in EUrope. [ Gerber, G., Palazzo, A., et al. (2025) ].

and in the 
# IIASA source dataset :
> Climate and landuse full crop pollination dataset: Gerber, G. (2026). European crop pollination supply, demand, and flow under climate and land-use change workflow and dataset (Version 1.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.22743969

> Climate-only SDMS and pollination supply metrics: Gerber, G., & Jung, M. (2026). European pollinator species distribution models and pollination supply metrics under climate change (Version 1.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.22751032

##  Underlying methodology and broader context:
> Palazzo, A. , Nakhavali, A. , Gerber, G. , Arbelaez Gaviria, J., Jung, M. , Drews, M., Meuriot, O.G.M., Martin, J.S., Bacca, S., Hinkel, J., & Lincke, D. (2025). ACCREU Report: Impacts on ecosystems & biodiversity. ACCREU (Assessing Climate Change Risk in EUrope). [https://www.accreu.eu/wp-content/uploads/2026/04/ACCREU_D2.4-with-annexes_revised-April-2026.pdf]


## Repository Contents (Metadata only)

This GitHub repository hosts only the metadata (this README and the data access page). The data files reside on Zenodo (DEI 10.5281/zenodo.23529106).

## Folder Structure

```text
CMCC_pollination/
└─ IIASA_CLIM_2020_2080/
   └─ <data files>
```

---

# Dataset Documentation

## 1. Files

Files are available for download from Zenodo ( )

| File | Content |
|---|---|
| `IIASA_CLIM_2020_2080/` | Pollination shocks on yield for 104 crops by NUTS 3 region, IIASA-CLIM scenarios, 2020–2080 |


## 2. Variables (all files)

| Column | Description |
|---|---|
| `NUTS_ID` | NUTS 3 region code (e.g. `AT127`) |
| `LEVL_CODE` | NUTS level (`3` = NUTS 3) |
| `CNTR_CODE` | Two-letter country code, Eurostat convention (e.g. `AT`) |
| `NAME_LATN` | Region name in Latin script |
| `nuts_total_hectares` | Area cultivated with the crop in the NUTS 3 region (hectares) |
| `base_name_crop` | Crop name (one of the 104 crops, e.g. `plum`) |
| `<SCENARIO>_<YEAR>` | % yield shock for a given climate scenario and year, e.g. `RCP2_6_2030` = RCP2.6 in 2030 (one column per scenario and year, 2020–2080, 5-year steps) |

Example

| NUTS_ID | LEVL_CODE | CNTR_CODE | NAME_LATN | nuts_total_hectares | base_name_crop | RCP2_6_2020 | RCP2_6_2025 | RCP2_6_2030 | … |
|---|---:|---|---|---:|---|---:|---:|---:|---|
| AT127 | 3 | AT | Wiener Umland/Südteil | 279.88 | plum | 0 | -2.46 | -5.81 | … |
| AT130 | 3 | AT | Wien | 40.13 | plum | 0 | -0.66 | -1.57 | … |
| AT211 | 3 | AT | Klagenfurt-Villach | 74.53 | plum | 0 | -0.9 | -2.62 | … |
| AT212 | 3 | AT | Oberkärnten | 132.89 | plum | 0 | -0.05 | -0.12 | … |

Shock values in % relative to 2020; reference year of nuts_total_hectares; full list of scenarios: RCP2.6 , RCP4.5 , RCP7.0 , RCP8.5 . 

## 3. Definitions

| Term | Definition |
|---|---|
| Pollination shock on yield | Change in crop yield due to projected changes in pollination services, relative to the baseline potential (2020). |
| IIASA-CLIM | Scenarios based on IIASA crop pollination supply, demand and flow under climate and land-use change (Gerber, 2026). |
| RCP | Representative Concentration Pathway. RCP2.6 , RCP4.5 , RCP7.0 , RCP8.5 |
| NUTS 3 | Third level of the Eurostat Nomenclature of Territorial Units for Statistics (NUTS): small regions. |

All `<SCENARIO>_<YEAR>` values are percentage changes in crop yield relative to 2020: values for 2020 are 0 and negative values are yield losses.


## License
- Data: This dataset is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

## Contact

G.A. Campoleoni Mansi, CMCC Foundation, [gabriele.mansi@cmcc.it](mailto:gabriele.mansi@cmcc.it)

## Funding Acknowledgement

This work was supported by the Assessing Climate Change Risk in Europe (ACCREU) project, funded by the European Commission under the Horizon Europe programme (grant agreement No. 101081358).

Project website: [ACCREU Website](https://www.accreu.eu/)



