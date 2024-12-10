R script to learn reproducibility in Github

#Question 1.
<br /> **In the Plot_data file, the experiment.csv data was plotted on a dot plot in its raw form and logarithmically transformed. In the fit_linear_model file, the data was split into two parts based on when the exponential growth ends in the logarithmic plot from before. Both parts were then fit into linear models.**

#Results
<br /> **In the plot_data_and_model file, a function was created to estimate N based on the time given and a formula using inputs from the linear models of fit_linear_model. N0 was taken by looking at the N at time 0 in the experiment.csv file, which was 879. r was the estimate of t in the first model case where t is small, which was 0.009902. Intercept estimate of the second model case where N has reached carrying capacity, which was 5.903e+10.** 

#Question 2.
<br /> **exponential growth: N = N0*e^(r*t)**
<br /> **N = 879*e^(0.009902*4980)**
<br /> **N = 2.29e+24**

<br /> **logistic growth: N <- (N0*K*exp(r*t))/(K-N0+N0*exp(r*t))**
<br /> **At time = 4980, N = (879*5.903e+10*exp(0.009902*4980))/(5.903e+10-879+879*exp(0.009902*4980)**
<br /> **N = 4.69e+23**

<br /> **The exponential growth model is much greater than the logistic growth because there is no limit from the carrying capacity.**


  


