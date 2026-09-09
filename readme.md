interpretable_ML_outlet_longterm

Repository for "Conditional predictability of Greenland outlet glacier retreat"

by Kevin Shionalyn, Ginny Catania, Daniel Trugman, Michael Shahin, Leigh Stearns, and Denis Felikson

Details of public data used as model input variables in this project can be found in the "Materials and Methods" section of the manuscript, with further details in the "Data and Methods" section of "Outlet glacier seasonal terminus prediction using interpretable machine learning". The process used for pre-processing data and running the XGBoost machine learning model is:

    Save input variable data time series as a .csv file with 3-digit glacierid at the start of each file. Data should be formatted with a header row, a 'Date' column and a 'Mean Variable' column (or revise processing codes to fit your schema).
    Run processing_scripts/GCV_Fitting.ipynb.
    Run processing_scripts/SSA.ipynb.
    Run processing_scripts/create_main_df_by_glacier.ipynb.
    Run xgboost_model.ipynb.

When running the above scripts, you'll need to set your own file paths for input files and output files, as these have been simplified.
