
<p align="center">
  <h3 align="center">Pharmaceutical Data Analysis</h3>
  <p align="center">
    A Matplotlib Project
    <br />
  </p>
</p>


<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Results](#results)


<!-- ABOUT THE PROJECT -->
## About The Project
## Background

![Laboratory](Images/Laboratory.jpg)

In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. Here I generated all of the tables and figures needed for the technical report of the study and a top-level summary of the study results.

Before beginning the analysis, I checked the data for any mouse ID with duplicate time points and removed any data associated with that mouse ID. Then I used the cleaned data for the remaining steps to generate a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. I also generated a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows  the number of total mice for each treatment regimen throughout the course of the study. Then, I generated a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study. Next, I calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin and also calculated the quartiles and IQR and quantitatively determine if there were any potential outliers across all four treatment regimens.

Using Matplotlib, I also generated a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.

Additionally, I performed following analyses too. 

* Select a mouse that was treated with Capomulin and generate a line plot of time point versus tumor volume for that mouse.

* Generate a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.

* Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.

* Write at least three observations or inferences that can be made from the data. 

### Built With
* [Python](https://www.python.org/about/)
  * [Pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/index.html)
  * [Matplotlib](https://matplotlib.org/3.3.1/contents.html)


## Results
Key inferences after data exploration:

1. Sample size appeared uniform across all drug regiment.

2. Gender distrubution was even across all drug regimen.

3. Capomulin and Ramicane appeared to be most effective drug againt tumor growth. Both of them have potential to be used for next stage of drug approval process. 

4. In the mouse selected for line plot (Mouse ID = m601), capomulin apperead very effective in reducing tumor volume with time. 

5. There is strong correlation between mouse weight and tumour volume for capomulin regimen (correlation cofficient = 0.84). This makes sense because, bigger a mouse is, it likely that the size of the tumor will be bigger based on its body size. This is further supprted by the equation of line of best fit for the relationship between weight and tumour volume, y = 0.95x + 21.55. Based on the equation, it appears that with increase of every gram of weight of mice, the tumor volume also increase by 1mm3 (0.95mm3 to be exact).

Here are some of the visualization I created after performing data analysis.
* Gender Distribution
![Gender_distribution](Images/gender_distribution.png align="left")

* Mouse weight vs average tumour volume
![Mousewt_vs_avgtumour_vol](Images/mousewt_vs_avgtumour_vol.png align="left")

* Number of mice per regimen
![Num_mice_per_regimen](Images/num_mice_per_regimen.png align="left")

* Tumour per regimen
![Tumour_col_per_regimen](Images/tumour_col_per_regimen.png align="left")

**Additional reference materials:**

_Best-README-Template_ Retrieved from: [https://github.com/othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template)






