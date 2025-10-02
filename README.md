# cortical-magnification-methods
This repository contains code for loading, analyzing, and plotting cortical 
magnification data from the HCP 7T retinotopy dataset (Benson et al., 2018). 
Two methods are available for computing cortical magnification, one based on
the geodesic distance between vertices on the brain surface, and the other 
based on the surface area around a vertex. The load script uses the neuropythy 
library for loading and processing HCP data, applies the Wang et al. (2015) 
atlas to each subject, and generates individual tsv files for each subject 
containing vertex-wise information like prf eccentricity, r2, and cortical 
magnification. The group script concatenates those tsv files into one 
dataframe. The analysis script analyzes and plots the data, and the comparison
script compares the results of the two methods. 

Authors: Adrian Wong, Uriel Lascombes
