# MANIA-IN-YOUTH-Understanding-Latent-Trajectories-and-Key-Risk-Factors
Analyzing symptom trajectories using Rstudio and Mplus, applying growth mixture modelling to identify latent trajectory classes and logistic regression to examine associated risk factors

=> OPTION 1: To access the data, go to:
https://nda.nih.gov/study.html?id=2313
Follow the necessary steps on the website to access the 5.1 ABCD-data release. Put the data into the (currently empty) "release_5.1" folder! Use the .Rmd files to run the code yourself. Running the code will progressively generate cleaned datasets in the (currently empty) "data" folder.

=> OPTION 2: Open the .html files for a fully executed version of the code with outputs and explanations. Simply double-click the .html files to view them in your browser. You don't need to download the data. To navigate the code, follow this order:

--------------------------------------------------------------------------------------------

RSTUDIO
=> Open the "code" folder.
=> Run/ View "01_readin_mania_scale" to read in the mania data.
=> Run/ View "02_readin_demographics" to read in the demographic data.
=> Run/ View "03_mplus_prep_modelling" to prepare the data for modelling in Mplus.

MPLUS
=> Open "code > MPLUS > neg_binomial".
=> Run the negative binomial models by opening an input file (inp) and clicking "RUN" (red button). Alternatively, open the PNG "00_linear_1class_input_example_screenshot" to get an understanding for an exemplary input file.
=> Look at the output of an negative binomial model by opening an output file (out).
Alternatively, open the PNG "00_linear_1class_output_example_screenshot_p1" - "...p5" to get an understanding for an exemplary output file.
=> Open "code > MPLUS > poisson". Proceed as before (e.g. run/ view input file, then view output file).

RSTUDIO
=> Open the "code" folder.
=> Read in/ view the Mplus results by running "04_readin_negativebinomial_and_poisson_model" and calculate class counts by running "05_class_counts". 
=> To compare the models, have a look at the "05_model_comparison_table" pdf file!
=> Plot/ view the best-fitting model (4-class negative binomial) by running "06_plot_best_model".
=> Run/ View "07_risk_factors" to read in the relevant risk factors, plot them, and prepare them for Mplus. 

MPLUS
=> Open "code > MPLUS > risk predictors > with_covariates".
=> Run the input files, view the output files. Alternatively, view the exemplary input and output files as PNG: "01_sleep_exemplary_input" and "01_sleep_exemplary_output_p1" - "...p7".
=> Open "code > MPLUS > risk predictors > without_covariates", proceed as above.
=> Open "code > MPLUS > risk predictors > sleep", procede as above.

RSTUDIO
=> Run/ View "08_readin_riskfactors_mplus" to read in the odds ratios for the risk factor results.
=> Run/ View "09_pvalues_and_summarytables" to read in the pvalues for the risk factor results, and create a summary table.
=> Run/ View "10_final_plots" to create the plots, summarizing the final results.
THE END



