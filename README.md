# Python-Project
Python-Based Analysis and Visualization of MgO Nanoparticle Characterization Data

Project Description:
This project provides an automated Python-based analytical pipeline for processing, quantifying, and visualizing characterization data of Magnesium Oxide (MgO) nanoparticles. It processes raw spectroscopic CSV files from X-Ray Diffraction (XRD) and Fourier-Transform Infrared Spectroscopy (FTIR), performing dynamic peak detection, baseline signal filtering, crystallite size calculation using Scherrer's equation, and functional group band identification.

Objectives:
Automate Data Cleaning: Ingest and preprocess raw, noisy numeric spectroscopic datasets from XRD and FTIR instruments.
Signal Filtering & Peak Isolation: Filter background noise using moving-average convolution and extract Bragg diffraction peaks automatically via dynamic thresholding.
Structural Quantification: Calculate Full Width at Half Maximum (FWHM) and derive crystallite sizes (D) using Scherrer's equation.Spectroscopic Transformation: Convert FTIR Transmittance (T) to Absorbance (A) using Beer-Lambert's Law (A = -\log_{10} T) and index characteristic Mg-O lattice modes.
Automated Output Generation: Export publication-ready vector plots (.png) and structured summary tables (.csv).

Requirements:
Software & EnvironmentPython Version: Python 3.8 or higher
Required Libraries: Install the necessary dependencies using pip:pip install numpy pandas scipy matplotlib

Instructions to Execute the Program:

Clone or Download the Repository:
git clone (https://github.com/your-username/MgO-Nanoparticle-Characterization.git)
cd MgO-Nanoparticle-Characterization

Prepare Data Files:
Ensure the following raw CSV input files are located in the root directory alongside Project.py:
MgO_XRD_sample.csv
MgO_FTIR_digitized.csv

Run the Script:
Execute the Python analytical pipeline from your terminal or command prompt:
python Project.py

View Results:
Upon completion, the program generates the following output files in the directory:
Figures: MgO_XRD_pattern.png, MgO_FTIR_Spectrum.pngData 
Tables: MgO_Scherrer_results.csv, MgO_FTIR_Results.csv
