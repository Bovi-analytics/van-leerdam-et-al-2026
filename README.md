# van-leerdam-et-al-2026
Code for the delayed milk ejection/bimodality paper where we looked at difference in lactation curve characteristics associated with delayed milk ejection. 

Delayed milk ejection (DME), characterized by a slow or interrupted increase in milk flow after the milking unit is attached, occurs in a substantial proportion of milkings. Although previous studies have shown that DME is associated with reduced milk yield during individual milkings, its implications for milk production over an entire lactation are less clear. In this study, a higher proportion of milkings with DME was associated with lower peak and cumulative milk yield, but little effect on persistency. These findings suggest that repeated DME may be relevant to dairy farm productivity and highlight the potential value of optimizing milking routines and genetic selection for favorable milkability.

The lactationcurve Python package was used for the creation of the lactation curves: van Leerdam, M. B., de Kok, D., Osei-Tete, J. A., & Hostens, M. (2026). Bovi-analytics/bovi lactationcurve: v.1.1.6 (Version 1.1.6) [Computer software]. https://doi.org/10.5281/zenodo.18715144. It thereby serves as an example of what can be done with the package.  

The workflow of the notebooks is the following: 
1. bi_modal_milk_flow_data_prep > Ingests the data from many excel files coming from the DelPro milk meter. It cleans data and removes unnecesary columns.
2. bi_modal_lactation_curve_characteristics > uses the lactationcurve package to fit the milk recordings to the lactation curves and calculates the lactation curve characteristics. Also gives the code to calculate the proportion of delayed milk ejection over the lactation.
3. For each characteristic there is a seperate notebook for the models: it includes data visualisation, train-test split, linear regression, xgboost and random forest hyperparameter tuning, model results and model test. For the tree models there is also permutation feature importance and Shapely value analysis.
   bi_modal_cumulaitve_milk_yield
   bi_modal_peak_yield
   bi_modal_persistency
   bi_modal_time_to_peak

The data for this project is currently not open source as it is private farm data. The code can be run, however, with any milkmeter data. 


If you have any questions or concerns feel free to reach out to me (Meike van Leerdam, mbv32@cornell.edu) 
