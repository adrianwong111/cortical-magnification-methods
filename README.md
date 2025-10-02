# Cortical magnification across the visual hierarchy
This repository contains code, results, and plots for a cortical
magnification project that I presented a poster for at the 2025 
Optica Fall Vision Meeting. The code is based off of work done by 
Uriel Lascombes, and relies much on the neuropythy library 
developed by Noah Benson to load and process the data from the 
HCP 7T retinotopy dataset.

The "code" folder contains code that loads, analyzes, and plots 
cortical magnification data taken from the HCP 7T retinotopy 
dataset. 
- load_dist.ipynb generates a tsv file for every subject, 
each tsv contains vertex-wise geodesic area, pRF area, r2, etc. 
Cortical magnification is calculated using the distance-based
method. load_area.ipynb is very similar to load_dist except that
cortical magnification is calculated using the area-based method.
The Wang et al. (2015) atlas is applied to every subject to
identify visual areas.
- group_dist.ipynb and group_area.ipynb filters and concatenates 
the individual tsv files.
- analysis_dist.ipynb and analysis_area.ipynb fits the Harvey model
to the CM vs eccentricity data.
- plot_dist.ipynb and plot_area.ipynb plots the results and metrics
generated from analysis.
- comparison.ipynb compares the results obtained from the two CM 
calculation methods.

The "plots" folder contains plots generated from the plots scripts.

The "results" folder contains results and metrics generated from 
the analysis scripts.

To generate the individual tsv files, you will have to download 
or access the HCP 7T retinotopy dataset yourself, which requires 
registration. Details on how to do so via neuropythy can be found
here: https://github.com/noahbenson/neuropythy

Adrian Wong,
UMN, Oct 2025
