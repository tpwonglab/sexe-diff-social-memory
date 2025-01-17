# "Social Valence Dictates Sex Differences in Identity Recognition": Source Code
## Ensemble analysis

MATLAB codes in this folder can be used to generate data for figures in the publication *Social valence dictates sex differences in identity recognition* by Larosa et al. Raw MATLAB data of this study can be found in [Dryad] (https://doi.org/10.5061/dryad.cfxpnvxhx).

* Load raw data with calcium imaging data and mouse coordinates during recordings (look for the mat file with its name containing raw.mat. e.g., raw data for mouse 1144 will be `1144_SDT_raw.mat`)
* Run the following 4 sets of codes to identify social ensembles:
  * `ensembles_A.m` for social ensembles for the negative valence mouse
  * `ensembles_N.m` for social ensembles for the neutral mouse
  * `ensembles_Ae.m` for nonsocial ensembles for the empty cup of the negative valence mouse
  * `ensembles_Ne.m` for nonsocial ensembles for the empty cup of the neutral mouse
* Note that the results from these analyses must be saved into another mat file. For instance, after running `ensembles_A.m`, the following variables should be saved in `1144_SDT_ensb.mat`: `ensb_BehavA`, `ensb_BehavA10`, `ensb_BehavA20`, `ensb_BehavA30`, `ensb_BehavA40`. A set of files with data from ensb analyses can also be found in Zenodo.
* After running all ensemble analyses, load all variables from the raw and ensb data file (e.g. 1144_SDT_raw.mat and 1144_SDT_ensb.mat), run “output_data.m” to extract values for Fig. 4 and Fig. S10 of the paper.

## SVM analysis
Use the raw data for SVM analysis (data with *Amanda.mat) from the Dryad repository and follow the readme in the SVM analysis folder.
