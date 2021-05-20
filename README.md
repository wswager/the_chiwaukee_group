***
![chicago_pic.jpg](https://github.com/wswager/the_chiwaukee_group/blob/main/images/chicago_pic.jpg)
***
# The Chiwaukee Group

A startup real estate development firm looking to capitalize on growth and business development in the geographic area between Chicago, Illinois and Milwaukee, Wisconsin, through investment in new residential projects.

# Business Problem

The Chiwaukee Group are specifically looking to target the counties located between Cook County, IL (Chicago) and Milwaukee County, WI:
* Lake County, IL
* Kenosha County, WI
* Racine County, WI

The Chiwaukee Group have requested a recommendation of the top-five zipcodes within which to invest.
***
## Background
### Business Development

The area has experienced significant recent business development:
* Amazon - 2015 - New Distribution Center
* Uline - 2010 - New Headquarters, 2018 - New Distribution Center
* Foxxconn - 2020 - New Manufacturing Plant, New Network Operations Center
* Meijer Inc. - 2014 - New Distribution Center
* Rust-Oleum Corp. - 2014 - New Distribution Center
* Gordon Food Service - 2010 - New Distribution Center

### Future Development

Marquette University Law School in Milwaukee has projected that the two metro areas will continue to merge into a single megaregion. They are currently conducting a [running project](https://law.marquette.edu/facultyblog/2012/07/milwaukees-future-in-the-chicago-megacity/) mapping the interconnection of the two geographic and economic entities while working with policymakers to encourage and facilitate the process going forward.

### Connection

The two cities are connected by a major interstate, I-94, as well as a train route, the Hiawatha Service, operated by Amtrak, which includes a stop in the city of Sturtevant in Racine County.
***
# Evaluation Metrics

**Risk**
Evaluated through Coefficient of Variance, ratio of the standard deviation to the mean, with an upper-limit set at 50%

**Historic Return on Investment**
Areas with prove return on investment, with a threshold of top 25% across the existing data’s timeframe

**Expected Future Returns**
Final recommendations will be based on future returns
***
# Data
Monthly median housing sales values between 1997 and 2017 downloaded from [Zillow](https://www.zillow.com/research/data/), an American online real estate marketplace.

![chi_mke_data.PNG](https://github.com/wswager/the_chiwaukee_group/blob/main/images/chi_mke_data.PNG)

### Working Zipcodes

60047 - Lake Zurich, IL
53142 - Kenosha, IL
53144 - Kenosha, IL
53158 - Pleasant Prairie, WI
53181 - Twin Lakes, WI
53108 - Caledonia, WI
53139 - Eagle Lake, WI
53404 - Racine, WI
53405 - Racine, WI
53185 - Waterford, WI

![monthly_price_v_zipcode.png](https://github.com/wswager/the_chiwaukee_group/blob/main/images/monthly_price_v_zipcode.png)
***
# Modeling
**SARIMAX**

Seasonal Auto Regressive Integrated Moving Average with Exogenous Factors

Time Series Model where each data point is associated with a time and the model predicts the next data based on statistical assessment of previous data.

## Evaluation Metrics
**Akaike Information Criterion** (AIC)
* A measurement error, comparing the model’s predictions to the actual data
* Adds a penalty for complexity, higher complexity can increase the likelihood of overfitting, if a model too closely reflects the actual data it will be less accurate in predicting future results
* Provides a standardized score which can be compared relative to other models
* Used to evaluate potential SARIMAX modeling parameters in order to determine the best parameters for the final model

**Root Mean Square Error** (RMSE)
* The standard deviation of the residuals of the model
* A measure of how concentrated the actual data is around the model’s prediction
* Used the assess the quality of fit of the final SARIMAX model

### Example Plot of Predictions v Existing Data
![53185_train_v_prediction.png](https://github.com/wswager/the_chiwaukee_group/blob/main/images/53185_train_v_prediction.png)

### Example Diagnostic Visuals Following Model Fitting
![60047_model.png](https://github.com/wswager/the_chiwaukee_group/blob/main/images/60047_model.png)
***
# Conclusions
## Top-Five-Zipcodes
![top5.PNG](https://github.com/wswager/the_chiwaukee_group/blob/main/images/top5.PNG)

## Recommendations
* Invest in in the area fifteen-to-twenty-five-miles West of Interstate-94, North of the Illinois border
* Invest in the area within five-miles of Interstate-94 in Kenosha County
* Discard interest in Illinois

## Detailed Observations

### Invest in in the area 15-25miles West of I94, North of the IL-border

Three of the top-five zipcodes, including the top-two,are located sequentially, fifteen-to-twenty-five-miles West of Interstate-94, from the north-most border of Racine County south to the Illinois border

Based on projections that Chicago and Milwaukee will continue to merge into a singular megaregion, it was anticipated that the area directly between, East of Interstate-94 to Lake Michigan, containing cities Kenosha, Racine, and Oak Creek would have been one of the areas on the rise

**Follow-Up Questions**
* Is the attraction to this area potentially associated with higher rated school system further separated from the cities? (Racine and Milwaukee cities have historically ranked among the worst school systems in the US)
* Are the higher forecasted returns potentially being driven by specific, smaller geographic areas, weighting the average for the zipcode? (Nearby Lake Geneva has historically one of wealthiest areas in the Midwest)
* Is the growth of the area even connected with commuting access to Milwaukee and/or Chicago? Are people looking for an area separated from the cities but still within commuting distance or is the growth of this area being driven be completed disassociated factors?

### Invest in the area within 5miles I94 in Kenosha County

The final two of the top-five-zipcodes were more predictably the area directly surrounding the major business developments along Interstate-94 in Kenosha.

This area would also have the most direct access to Interstate-94 and the Hiawatha Train service stop for commuter access (both Milwaukee and Chicago are approximately forty-five-minutes drive)(the Hiawatha train stop in Sturtevant, Wisconsin is two-miles from Interstate-94 in Racine County, approximately ten-totwenty-minutes drive from this area)

**Follow-Up Questions**
* What is type of competition exists for the development residential projects in this area?
* What types of residences are in-demand in this area? What type of socioeconomic profile is being drawn to the area by the business development?
* Are people moving to this area for distribution center and manufacturing jobs or for commuter access to Milwaukee and/or Chicago?

### Discard interest in Illinois

All five of the top-five zipcodes are all located in Wisconsin, not Lake County in Illinois

**Follow-Up Questions**
* How big a factor is the significant discrepancy between state tax-rates in Wisconsin compared to Illinois?

## Next Steps
* Additional research can be performed regarding factors such as:
  * Tax Rates
  * Interest Rates
  * School District Ratings
  * Crime Rates
  * Median Household Incomes
* Additional modeling types can be utilized in the analysis of further data types
* Polling can be performed with current residents, with specific emphasis on people who moved to the area recently, to gather further data regarding personal driving factors potentially not captured by available statistics
* Further research can be performed narrowing the geographic range within the top zipcodes to attempt to discover more specifically which areas The Chiwaukee Group should look to invest in
***
# The Chiwaukee Group
***
![milwaukee_pic.jpg](https://github.com/wswager/the_chiwaukee_group/blob/main/images/milwaukee_pic.jpg)
***
# Thank You

### Wes Swager
* [Email](mail.westin.swager@lsventures.com)
* [GitHub](https://github.com/wswager)
* [LinkedIn](linkedin.com/in/wes-swager-36a84a2a)
