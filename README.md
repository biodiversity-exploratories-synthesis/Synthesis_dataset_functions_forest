(https://github.com/biodiversity-exploratories-synthesis/Synthesis_dataset_functions_forest/assets/59728330/4cbc09c5-ecb2-48d4-9394-1a0eab6652e6))(https://github.com/biodiversity-exploratories-synthesis/Synthesis_dataset_functions_forest/assets/59728330/5cd478bf-fbec-40be-b7ec-35f9757f373b)# Synthesis_dataset_functions_forest
Released at Zenodo : NOT YET RELEASED

Code used for generation of the synthesis grassland function dataset [https://github.com/biodiversity-exploratories-synthesis/Synthesis_dataset_functions_forest/Synthesis_dataset_functions_forest.R](https://github.com/biodiversity-exploratories-synthesis/Synthesis_dataset_functions_forest/blob/main/forest_synthesis.R)

### License

This project is licensed under the terms of the Creative Commons Attribution 4.0 license (cc-by-4.0).

# Versions

- July 2023: Currently the synthesis dataset functions forest is under construction.

# Scripts

- `forest_synthesis.R` : R-script to assemble and calculate variables for the synthesis dataset functions forest (i.e. [BE_synthesis_forest_dat.txt](https://github.com/biodiversity-exploratories-synthesis/Synthesis_dataset_functions_forest/blob/main/BE_synthesis_forest_dat.txt)). Download the raw data from BExIS (https://www.bexis.uni-jena.de/ddm), unzip them and adjust the "pathtodata" variable to read in raw data and process it. Variables selected from the raw data are sorted by the "Process and component name" (i.e. Soil carbon cycling) and are processed in the respective code blocks.
- `multidiversity.R` : contains function required to calculate mini-multifunctionalities, such as "soilCflxs_2011". Is sourced by forest_synthesis.R.

## Notes

- Negative values of scaled variables have been corrected, by scaling (sd = 1), but not centering (mean =/= 0). Affected variables are for example dung_removal (21206_3_Dataset) and the leaf area damaged by different herbivores (24806_2_Dataset). Dung removal was scaled and centered in the grasslands functions synthesis dataset (BExIS ID 27087). In a future update, scaled variables in the grasslands dataset will not be centered anymore to avoid negative values (not yet implemented).
