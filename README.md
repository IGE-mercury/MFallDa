## Description 
MFallda is the first global dataset resulting from compiling and harmonizing all available data on total Hg (THg) and methylmercury (MeHg) concentrations and fluxes in litterfall (LF) and throughfall (TF). The dataset includes measurements collected between 1987 and 2024 from 147 sites distributed across all major biomes, together with metadata on ecosystem type, sampling protocol, precipitation, wet deposition, and Köppen–Geiger climate classification.\
This dataset provides an open-access, standardized resource to improve spatially explicit estimates of vegetation-mediated Hg inputs to soils, refine inter- and intra-site Hg budgets, and support model calibration and validation at regional to global scales. A contribution template is provided to facilitate community data sharing and ensure regular updates.


## Structure of the file

| Column name | Type | Units | Description |
|--------------|------|--------|--------------|
| AuthorYear | Text | - | Concatenation of first author name and year of publication, identifier of publication |
| TitleStudy | Text | - | Title of the study |
| Location | Text | - | Brief description of the sampling area (region – administrative region or province – country) |
| Continent | Text | - | Continent of sampling (Africa, Asia, Europe, North America, South America) |
| Latitude_N | Numeric | Degree north (decimal) | Latitude of sampling |
| Longitude_E | Numeric | Degree east (decimal) | Longitude of sampling |
| Altitude | Numeric | m | Above-sea-level altitude of sampling |
| StudyYear | Numeric | YYYY | Period of sampling (Year start – Year end) |
| SampleId | Text | - | Identifier of the measurement in the study; when not provided, constructed from LandType(+_Year) or Tissues(+_Year). Each ID corresponds to one measurement. |
| LandCover | Text | - | Description of the land cover, variable level of detail depending on the article |
| LandType | Categorical | DBF, ENF, RBF, EBF, Grass, Mixed, Mangrove, Savanna, Shrubs, Urban | Categorical description of land cover type |
| Vegetation | Text | - | Plant species reported in the article |
| Climate | Categorical | Af, Am, Aw, BSh, BWk, BWh, Cfa, Cfb, Csb, Cwa, Cwb, Dfa, Dfb, Dfc, Dwa, Dwb, Dwc | Climate classification (Köppen-Geiger) |
| AnnualPrecip_Volumemm | Numerical | mm | Annual precipitation volume; bold values represent site means reported in the article |
| MethodLitterfall | Text | - | Description of litterfall sampling procedure and period |
| MethodThroughfall | Text | - | Description of throughfall sampling procedure and period |
| AnnualThroughfall_Volume_mm | Numeric | mm | Annual throughfall depth |
| Tissues | Categorical | Total, Needles, Leaves, Fruits, Bark, Misc, Twigs, Lichens | Litterfall plant tissues collected (“Total” = unsorted litterfall) |
| LitterfallHg_MeanConcentration_ngg | Numerical | ng Hg g⁻¹ dry matter | Mean Hg concentration in litterfall, averaged over replicates and sampling period |
| LitterfallHg_AnnualMeanFlux_ugm2 | Numerical | µg Hg m⁻² yr⁻¹ | Annual flux of Hg deposited through litterfall |
| LitterfallMeHg_MeanConcentration_ngg | Numerical | ng MeHg g⁻¹ dry matter | Mean MeHg concentration in litterfall, averaged over replicates and sampling period |
| LitterfallMeHg_AnnualMeanFlux_ugm2yr | Numerical | µg MeHg m⁻² yr⁻¹ | Annual flux of MeHg deposited through litterfall |
| LitterfallBiomass_gm2yr | Numerical | g dry matter m⁻² yr⁻¹ | Annual biomass deposited through litterfall |
| WVMC_TF_Hg_ngL | Numerical | ng Hg L⁻¹ | Volume-weighted mean concentration of Hg in throughfall (only two articles report this explicitly) |
| TF_AnnualMeanConcentration_Hg_ngL | Numerical | ng Hg L⁻¹ | Annual mean concentration of Hg in throughfall |
| TF_AnnualMeanConcentration_MeHg_ngL | Numerical | ng MeHg L⁻¹ | Annual mean concentration of MeHg in throughfall |
| OpenPrecipitation_AnnualMeanConcentration_MeHg_ngL | Numerical | ng MeHg L⁻¹ | Annual mean concentration of MeHg in open precipitation |
| OpenPrecipitation_AnnualMeanFlux_Hg_ugm2yr | Numerical | µg Hg m⁻² yr⁻¹ | Annual mean flux of Hg in open precipitation |
| OpenPrecipitation_AnnualMeanFlux_MeHg_ugm2yr | Numerical | µg MeHg m⁻² yr⁻¹ | Annual mean flux of MeHg in open precipitation |
| OpenPrecipitation_AnnualMeanConcentration_Hg_ngL | Numerical | ng Hg L⁻¹ | Annual mean concentration of Hg in open precipitation |
| Flag | Text | - | Supplementary information about sampling procedure, data, or contamination |
| DOI | Text | - | DOI of article, starting with “10.” |

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


