## Description 
MFallDa is the first global dataset that compiles and harmonizes all available measurements of total mercury (THg) and methylmercury (MeHg) concentrations and fluxes in litterfall (LF) and throughfall (TF). It can be accessed via [Zenodo](https://doi.org/10.5281/zenodo.17816916). It contains data collected between 1987 and 2024 from 147 sites spanning all major biomes, accompanied by detailed metadata on ecosystem type, sampling protocols, precipitation, wet deposition, and Köppen–Geiger climate classification.

This open-access, standardized dataset provides a foundation for improving spatially explicit estimates of vegetation-mediated Hg inputs to soils, refining inter- and intra-site Hg budgets, and supporting model calibration and validation from regional to global scales. A contribution template is included to facilitate community data sharing and ensure regular updates.


## Structure of the Repository

**WOS_search.csv**, contains the results of the Web Of Science search, indicating for each publication whether data were collected and, if not, the reason for exclusion. The seven columns of the WOS_references file are described in detail in Table 1 of the associated manuscript. The references are listed in **WOS_references.bib**.

**MFallDa.csv** contains the collected data, including article sources, location, year of sampling, vegetation type at the sampling site, sampling procedure, tissues types, and THg and MeHg LF and TF concentrations and deposition fluxes. The 34 columns of the MFallDa file are described in detail in Table 2 of the associated manuscript, including units for numerical columns. The references are listed in **MFallDa_references.bib**.

**template_new_data.csv** is a template that provides the required structure for users who wish to contribute new measurements to the database. Each column corresponds to a standardized variable used in the dataset. Please fill in all mandatory fields, as described in Table 2 of the associated manuscript. 

---
## License

This dataset is distributed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
If you use or modify this dataset in your work, please refer to the `CITATION.cff` file for citation information.

---

## Contribution to this dataset

### Two branches are available: 
- **main** → Stable, published version of the dataset (matches the latest Zenodo release).  
- **dev** → Working branch for upcoming updates, additions, or documentation improvements.

All changes should be proposed as **pull requests (PRs)** targeting the `dev` branch.  
After review and validation, changes in `dev` are merged into `main`, and a new **release** is created on Zenodo.


---

###  Workflow for contributors 

1. Create your own copy of the repository ("fork"). This allows you to make changes without affecting the main repository.
2. Create a new branch from the `dev` in your fork. Use this branch to add your contributions (new data, corrections, or documentation updates).
3. Submit a pull request (PR) from your branch to the `dev` branch of this repository.  
4. The maintainers will review your PR and, once approved, merge it into `dev` in preparation for the next official release.

For users who do not use or are not familiar with GitHub, we also welcome data submissions by email using the provided template file.
