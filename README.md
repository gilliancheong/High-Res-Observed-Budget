# High-Res-Observed-Budget
 Data files and code used in the calculation of a high-resolution observed sea ice concentration budget in the Arctic's Last Ice Area. This is part of a dissertation in part fulfilment of the MSci Environmental Geoscience degree, written by Gillian Cheong.

 ## High-resolution sea ice concentration budget analysis in the Arctic’s Last Ice Area
 ### Overview
 This repository contains two custom modules, an executable Jupyter Notebook, and sample data files and code to run the sea ice concentration budget analysis. The data processing and budget calculation modules have been kindly provided by Dr Harry Heorton. Data plotting and analysis is executed on the Jupyter Notebook, Budget_Analysis.ipynb. Sample data presented in this repository is for 18-24 March 2020. 
 
 This Jupyter Notebook does not demonstrate data processing and smoothing that was executed during this project, and only demonstrates data plotting. For the full code, which allows the input of raw data formats, please refer to high-res_budget.ipynb. The full dataset and accompanying code is running on the server on /home/gch/MSci_Submission.
 
 In this project, the two modules and notebook were used in the following steps:
 ### 1. Import and process data into Jupyter
   #### Key features
   - Data formats are in raw format, with no preprocessing, smoothing or regridding needed beforehand. 
   - Capable of computing daily and monthly budget.
   - Can accomodate gaps in data.


 ### 2. Module 1: Budget inputs

 This module contains the code required to access input data on the Jupyter Notebook. Each type of input data has its own class, which enables the script to decide which data it needs to access and when to access it. The input data class is used to access the code.


 ### 3. Module 2: Budget calculation

 This module contains the custom functions used in the code. It contains the smoothing function, as well as functions to calculate the intensification, advection and divergence terms of the observed budget. The main Jupyter Notebook then derives the residual term by subtracting advection and divergence from intensification.


 ### 4. Plot data
   #### Key features
   - Timeseries of decomposed budget
   - Map composites combining sea ice drift vectors and budget components


 ### 5. Calculate volume estimates of budget components
   #### Key features
   - Mask data to constrain to regions of convergence only. This mask can be altered as you wish. 

