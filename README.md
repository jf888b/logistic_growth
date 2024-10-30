R script to learn reproducibility in Github

#Question 1.
In the Plot_data file, the experiment.csv data was plotted on a dot plot in its raw form and logarithmically transformed.
In the fit_linear_model file, the data was split into two parts based on the when the exponential growth ends in the logarithmic plot from before. Both parts were then fit to linear models.
In the plot_data_and_model file, a function was created to estimate N based on the time given and a formula using inputs from the linear models of fit_linear_model. N0 was taken by looking at the N at time 0 in the experiment.csv file, which was 879. r was the estimate of t in the first model case where t is small, which was 0.009902. Intercept estimate of the second model case where N has reached carrying capacity, which was 5.903e+10. 
