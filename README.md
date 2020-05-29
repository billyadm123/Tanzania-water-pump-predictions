For my third project for Flatiron school, I had to create a model that classifies water pumps in Tanzania between three different classes: Functional, Non-Functional, and Functional but needs repair. After careful data exploration and some feature engineering I chose:

amount_tsh
funder
installer
longitude
latitude
basin
region
population
construction_year
extraction_type
management
payment 
water_quality
quantity
source
source_class
waterpoint_type
status_group
years_since_checked

as my predictor variables.

K-Nearest Neighbor performed the best with an accuracy score of 76%. It also correctly classified non-functional pumps 82% of the time, which I think is the most important class in this problem. Correctly classified non-functional pumps can increase maintenance response times, prevent illness, and prevent negative impact on the economy and environment. The multi-layer nueral network performed second best with 76% accuracy but only 76% precision for the non-functional pumps. However, when using a boxplot to compare my models, except for the nueral network, the decision tree and adaboost classifier had two of the highest mean values and lowest variances. I think more data is needed such as road conditions, events that are occuring at the time which may also affect accessibility and sensor data for the actual pump to improve the predictions.¶
