# Russia Ukraine War Time Series EDA  

Hey, Guys! In this notebook, I will do some time series EDA. This dataset can provide us with a wealth of insights. Let's explore it together.  

In this dataset, there are two days of data that require adjustments. Let's start by handling this part. Additionally, because there are numerous features available, I will focus on selecting the most important ones, including 'aircraft,' 'helicopter,' 'tank,' 'APC,' and 'field artillery.'  

### First, let's create trend plots for equipment and personnel losses.  

The losses for aircraft and helicopters increased sharply in the initial weeks but then leveled off. Losses for tanks and armored personnel carriers (APCs) showed a continuous upward trend.  
Field artillery losses also increased in the early stages but appeared to decrease somewhat in the middle.
![__results___6_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/576ba04d-ed9d-42cd-9e07-36b15f254319)  
The personnel losses increased sharply in the early stages but then increased at a more moderate pace. The number of prisoners of war (POW) increased at certain times, especially during the middle period.   

![__results___8_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/df702499-e435-4061-8f2f-c3f3e1887b5f)

### In addition to the fundamental temporal trends, we can embark on the following EDA explorations:  
**1. Cumulative Losses:** Display the cumulative losses for each type of equipment or personnel over time.

Tanks, APCs, and field artillery show a continuous increase in cumulative losses throughout the period. From the graph, it's evident that both personnel losses and the number of prisoners of war (POWs) continue to rise throughout the entire period.  

![__results___11_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/45271d3e-0555-4b2b-a014-fcf48c4f293e)


**2. Loss Distributions:** Employ box plots or violin plots to portray the distribution of losses across various equipment types or personnel.  
Aircraft and helicopters have more concentrated loss distributions, while other equipment like tanks and APCs have more scattered loss distributions. Field artillery also exhibits some extreme values in terms of losses.

![__results___13_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/0ffcffaa-6b5b-48fe-aea0-a2f127343ca2)


**3. Loss Disparities**: Calculate the differences in losses between consecutive days or weeks, enhancing our understanding of loss velocity or rhythm.  
On certain dates, the disparities in equipment losses are notably significant, which might indicate substantial conflicts or events occurring on those specific days. The differences in personnel losses are remarkably prominent on certain days, suggesting a potential association with specific events. Similarly, the variance in the number of POWs is substantial on particular days.  

![__results___15_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/1be4a049-49f4-4300-ab5a-1d8284d7de35)


**4. Moving Averages:** Compute 7-day or 30-day moving averages to smoothen the data and gain deeper insights into trends.  
We can observe smoother trend lines, especially for helicopter and aircraft losses, which aids us in gaining a better understanding of the overall trends.

The moving average of personnel losses increases during certain periods, but there is an overall upward trend. Similarly, the moving average of POWs also experiences some growth during specific periods.  

![__results___17_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/05b01724-4e34-489a-9415-2864d54cce7a)

**5. Stacked Area Chart:** This can be used to display the proportion of various equipment losses in the total losses.  
From the charts, it's evident that tank and armored personnel carrier (APC) losses constitute a significant portion of the total losses.
![__results___22_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/4faa93b6-fe9b-428e-acb3-216f49c3071a)

**6. Autocorrelation and Partial Autocorrelation Plots:**  
ACF (Auto-Correlation Function): In the initial lags, the autocorrelation decreases relatively quickly, indicating that the correlation between values of the time series decreases as the lag increases.  

PACF (Partial Auto-Correlation Function): There is a significant peak at the initial lags, such as lag 1, which may suggest the presence of some autoregressive pattern.  
![__results___32_1](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/5464c8ad-3cd0-4826-a589-58bcfb2acb56)

**7. Heatmap analysis:**  
Using a heatmap to analyze tank losses on each day of the week is an excellent approach to identify patterns specific to certain days of the week. It appears that certain weeks and weekdays experience higher losses, which could be attributed to specific events during those times.  
Interestingly, weekends (Saturday and Sunday) seem to have lower losses.

![__results___34_0](https://github.com/Elvis-YAL/Russia-Ukraine-War-Time-Series-EDA./assets/40426433/0a960e2d-f73f-47ec-88bf-9c7aeb1a1a29)

We still have some advanced analysis, if you want to see more, please feal free to look at my notebook.





