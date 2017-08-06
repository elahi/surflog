surflog
========================================================
author: Robin Elahi
date: August 7, 2017
autosize: true

1
===
![](../images/nick-1.jpg)

2
===
- The need

3
===
- User inputs
- Ocean conditions
- *surflog* outputs
  1. Visualize your sessions
  2. Predict your next session

4 - Visualize your sessions
====================================
![](/figs/plot_dat_yrm_n.png)


5 - Visualize your sessions
====================================
![](/figs/map_3_panels.png)


6 - Predicting the number of rides
====================================
<br>
<br>
Generalized linear model with four predictors
  - Swell height, period and direction
  - Tidal height
<br>
<br>
<br>
$$Rides_{i} = Poisson(\mu_{i})$$
<br>
$$E(Rides_{i}) = var(Rides_{i}) = \mu_{i}$$
<br>
$$log(\mu_{i}) = \alpha + \beta_{h}Height_{i} + \beta_{p}Period_{i} ~+$$ 
$$\beta_{d}Direction_{i} + \beta_{t}Tide_{i}$$ 

The money plot
========================================================
![](../figs/predict_session_random.png)

Observed vs predicted
========================================================
![](../figs/obs_pred_ride_count.png)

