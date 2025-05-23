# Repeated upslope biome shifting during late-Cenozoic climate cooling in a diverse alpine plant clade     

## [gene trees and alignments](https://zenodo.org/record/8408326)
Follow [this link](https://zenodo.org/record/8408326) to the zenodo repository.

## [molecular branch length estimation](https://github.com/pebgroup/alpine_saxifraga/tree/main/molecular_branch_length_estimation)
This contains scripts for branch-wise analysis and gene shopping. Needs a reference [species tree](https://github.com/pebgroup/alpine_saxifraga/blob/main/molecular_branch_length_estimation/species_tree_rooted.tre) and gene trees. Gene trees are available on the related Zenodo repository. The branch_wise script is an early version of the script that was used for this study. A far faster version will be made available soon. 

## [divergence time estimation](https://github.com/pebgroup/alpine_saxifraga/tree/main/divergence_time_estimation)
This provides the necessary inputs to estimate the time-calibrated phylogenies that were estimated in this study. In each case the *treePL* configuration file is provided (ending in .treePL) and the input tree file (ending in .tre)

A more user friendly version of the congruent branches method for getting molecular branch lengths to then use in treePL is [here](https://github.com/TomCarr/GetCongruentBranches).

## [lineage specific diversification rate estimation](https://github.com/pebgroup/alpine_saxifraga/tree/main/lineage_specific_diversification_rate_estimation)
This provides the necessary inputs to perform lineage specific diversification rate estimation on the time-calibrated phylogeny designated as main, and no maximum. In each case the BAMM input file, and input time-calibrated phylogeny is provided. Also provided is an [R script](https://github.com/pebgroup/alpine_saxifraga/blob/main/lineage_specific_diversification_rate_estimation/set_priors.R) used to get appropriate priors in each case, and an [R script](https://github.com/pebgroup/alpine_saxifraga/blob/main/lineage_specific_diversification_rate_estimation/bamm_analysis.R) used for analysing and plotting outputs.

## [ClaSSE](https://github.com/pebgroup/alpine_saxifraga/tree/main/ClaSSE) 
This contains all the scripts needed to perform ClaSSE analyses that were undertaken as part of this study. [main](https://github.com/pebgroup/alpine_saxifraga/tree/main/ClaSSE/main) and [no_maximum](https://github.com/pebgroup/alpine_saxifraga/tree/main/ClaSSE/no_maximum) contain scripts for analysis on the main and no maximum trees respectively. [final_tree_and_data_frame_processing.r](https://github.com/pebgroup/alpine_saxifraga/blob/main/ClaSSE/final_tree_and_data_frame_processing.r) prunes the species tree and compiles the [biome_and_region_preference](https://github.com/pebgroup/alpine_saxifraga/blob/main/ClaSSE/biome_region.csv) into a matrix for analysis in the ClaSSE model. Note that line 118 in [final_tree_and_data_frame_processing.r](https://github.com/pebgroup/alpine_saxifraga/blob/main/ClaSSE/final_tree_and_data_frame_processing.r) needs adjusting depending on which output tree from treePL you are working on. [biome_and_region_preference](https://github.com/pebgroup/alpine_saxifraga/blob/main/ClaSSE/biome_region.csv) is equivalent to Table S5 in the manuscript.  

