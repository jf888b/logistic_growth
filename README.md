R script to learn reproducibility in Github

## Question 1.
<br /> In the plot_data file, the experiment.csv data was plotted on a dot plot with time on the x-axis and population size on the y-axis in its raw form which shows a logistic growth curve. The growth changes from flat, constant population size to exponential at t=1800 minutes and then back to flat, constant size at t=2200 minutes. The data was logarithmically transformed to better show the large range of growth rate and population size. The resulting graph shows linear growth from almost 0 to below 1e+11. 

In the fit_linear_model file, the data was split into two parts and fit into linear models. One is when the carrying capacity is greater than the initial population size and t is small. The other is when the population size is equal to carrying capacity. These are split into before and after 1800 minutes, respectively. The first linear model result showed that when t > 1800 minutes, the value is constant because N is always 5.903e+10. The second linear model result shows that when t < 1800 minutes, the slope is 0.009902 which is the rate of log population growth over time.

## Results
<br /> In the plot_data_and_model file, a function was created to estimate population size based on the time given and a formula using inputs from the linear models of fit_linear_model. N0 was taken by looking at the N at time 0 in the experiment.csv file, which was 879. r was the rate of growth in the first model case where t is small, which was 0.009902. K is the carrying capacity shown by the second model case which was 5.903e+10. 

## Question 2.
<br /> **Exponential Growth:** N = N0*e^(r*t)
<br /> N = 879*e^(0.009902*4980)
<br /> N = 2.29e+24

<br /> **Logistic Growth:** N <- K/(1+((K-N0/N0))e^(-rt))
<br /> At time = 4980, N = 5.903e+10/(1+(5.903e+10-879/879)e^(-0.009902*4980))
<br /> N = 5.903e+10

<br /> The exponential growth model is much greater than the logistic growth because there is no limit from the carrying capacity.

## Question 3.
Code in exp_log_graphs file.
<img width="552" alt="Screenshot 2024-12-13 at 9 07 29 AM" src="https://github.com/user-attachments/assets/57c3636f-3d69-48a9-b42e-b546b9ab6dae" />


  


