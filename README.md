## Description 
MFallda is the first global dataset resulting from compiling and harmonizing all available data on total Hg (THg) and methylmercury (MeHg) concentrations and fluxes in litterfall (LF) and throughfall (TF). The dataset includes measurements collected between 1987 and 2024 from 147 sites distributed across all major biomes, together with metadata on ecosystem type, sampling protocol, precipitation, wet deposition, and Köppen–Geiger climate classification.\
This dataset provides an open-access, standardized resource to improve spatially explicit estimates of vegetation-mediated Hg inputs to soils, refine inter- and intra-site Hg budgets, and support model calibration and validation at regional to global scales. A contribution template is provided to facilitate community data sharing and ensure regular updates.


## Structure of the file

| Column name | Type | Units | Description |
|--------------|------|--------|--------------|
| AuthorYear | Text | - | Concatenation of first author name and year of publication; identifier of the publication |
| TitleStudy | Text | - | Title of the study |
| Location | Text | - | Brief description of the sampling area (region – administrative region or province – country) |
| Continent | Text | - | Continent of sampling (Africa, Asia, Europe, North America, South America, Oceania) |
| Latitude_N | Numeric | Degree north (decimal) | Latitude of sampling |
| Longitude_E | Numeric | Degree east (decimal) | Longitude of sampling |
| Altitude | Numeric | m | Above-sea-level altitude of the sampling site |
| StudyYear | Numeric | YYYY | Sampling period (start year – end year) |
| SampleId | Text | - | Identifier of the measurement; if not provided, constructed from LandType(+_Year) or Tissues(+_Year). Each ID corresponds to one measurement. |
| LandCover | Text | - | Description of land cover; level of detail varies depending on the article |
| LandType | Categorical | DBF, ENF, RBF, EBF, Grass, Mixed, Mangrove, Savanna, Shrubs, Urban | Standardized land cover category |
| Vegetation | Text | - | Plant species reported in the study |
| Climate | Categorical | Af, Am, Aw, BSh, BWk, BWh, Cfa, Cfb, Csb, Cwa, Cwb, Dfa, Dfb, Dfc, Dwa, Dwb, Dwc | Köppen-Geiger climate classification |
| AnnualPrecip_Volume_mm | Numerical | mm | Annual precipitation volume; bold values indicate site means reported in the article |
| MethodLitterfall | Text | - | Litterfall sampling protocol and sampling period |
| MethodThroughfall | Text | - | Throughfall sampling protocol and sampling period |
| AnnualThroughfall_Volume_mm | Numeric | mm | Annual throughfall depth |
| Tissues | Categorical | Total, Needles, Leaves, Fruits, Bark, Misc, Twigs, Lichens | Litterfall plant tissues collected (“Total” = unsorted litterfall) |
| LitterfallHg_MeanConcentration_ngg | Numerical | ng Hg g⁻¹ dry matter | Mean THg concentration in litterfall, averaged over replicates and sampling period |
| LitterfallHg_AnnualMeanFlux_ugm2 | Numerical | µg Hg m⁻² yr⁻¹ | Annual THg flux deposited through litterfall |
| LitterfallMeHg_MeanConcentration_ngg | Numerical | ng MeHg g⁻¹ dry matter | Mean MeHg concentration in litterfall, averaged over replicates and sampling period |
| LitterfallMeHg_AnnualMeanFlux_ugm2yr | Numerical | µg MeHg m⁻² yr⁻¹ | Annual MeHg flux deposited through litterfall |
| LitterfallBiomass_gm2yr | Numerical | g dry matter m⁻² yr⁻¹ | Annual biomass flux through litterfall |
| WVMC_TF_Hg_ngL | Numerical | ng Hg L⁻¹ | Volume-weighted mean concentration of THg in throughfall (reported explicitly in only two studies) |
| TF_AnnualMeanConcentration_Hg_ngL | Numerical | ng Hg L⁻¹ | Annual mean THg concentration in throughfall |
| TF_AnnualMeanConcentration_MeHg_ngL | Numerical | ng MeHg L⁻¹ | Annual mean MeHg concentration in throughfall |
| OpenPrecipitation_AnnualMeanConcentration_MeHg_ngL | Numerical | ng MeHg L⁻¹ | Annual mean MeHg concentration in open precipitation |
| OpenPrecipitation_AnnualMeanFlux_Hg_ugm2yr | Numerical | µg Hg m⁻² yr⁻¹ | Annual mean THg flux in open precipitation |
| OpenPrecipitation_AnnualMeanFlux_MeHg_ugm2yr | Numerical | µg MeHg m⁻² yr⁻¹ | Annual mean MeHg flux in open precipitation |
| OpenPrecipitation_AnnualMeanConcentration_Hg_ngL | Numerical | ng Hg L⁻¹ | Annual mean THg concentration in open precipitation |
| Flag | Text | - | Additional information about sampling procedure, data quality, or contamination issues |
| DOI | Text | - | DOI of the article (starting with “10.”) |

---
## License

This dataset is distributed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
If you use or modify this dataset in your work, please refer to the `CITATION.cff` file for citation information.

---

## Contribution to this dataset

### Two branches are available: 
- **main** → Stable, published version of the dataset (matches the latest Zenodo release).  
- **dev** → Working branch for upcoming updates, additions, or documentation improvements.

All changes should be proposed as **pull requests (PRs)** against the `dev` branch.  
Once reviewed and validated, changes from `dev` are merged into `main`, and a new **release** is created.


---

###  Workflow for contributors 

1. Fork this repository and create a new branch from `dev` in your fork.  
2. Add your contributions (data, corrections, or documentation). For convenience, you may use the template CSV file available in the repository.  
3. Submit a pull request (PR) from your branch to the `dev` branch of this repository.  
4. The maintainers will review your PR and merge it into `dev` before the next official release.


