# Data Science Challenge - User History
We suggest spending 1-2 hours on this, but you're welcome to spend more or less. This is your chance to wow us with creative and rigorous solutions! Please include your code via zipped attachment via email, or as a pull request on this repository. We also accept incomplete solutions.

Please send us a brief writeup of your findings (the more concise, the better), along with any summary tables, graphs, code, or queries that can help us understand your approach. Please note any factors you considered or investigation you did, even if they did not pan out. Feel free to identify any further research or data you think would be valuable.


## Data Sources
Datasets are available under the local `./data` folder.


### `attributes.json`
1. **`city`**: city this user signed up in
2. **`phone`**: primary device for this user
3. **`signup_date`**: date of account registration; in the form ‘YYYYMMDD’
4. **`last_trip_date`**: the last time this user completed a trip; in the form ‘YYYYMMDD’
5. **`avg_dist`**: the average distance in miles per trip taken in the first 30 days after signup
6. **`avg_rating_by_driver`**: the rider’s average rating over all of their trips
7. **`avg_rating_of_driver`**: the rider’s average rating of their drivers over all of their trips
8. **`surge_pct`**: the percent of trips taken with surge multiplier > 1
9. **`avg_surge`**: The average surge multiplier over all of this user’s trips
10 **`trips_in_first_30_days`**: the number of trips this user took in the first 30 days after
signing up
11. **`upgraded_user`**: TRUE if the user took an upgraded ride in their first 30 days;
FALSE otherwise
12. **`weekday_pct`**: the percent of the user’s trips occurring during a weekday


## The Problem
We are interested in predicting rider retention. To help explore this question, we have provided a sample dataset of a cohort of users who signed up for an account in January 2014. The data was pulled several months later; we consider a user retained if they were “active” (i.e. took a trip) in the preceding 30 days.

We would like you to use this data set to help understand what factors are the best predictors for retention, and offer suggestions to operationalize those insights.

1. Perform any cleaning, exploratory analysis, and/or visualizations to use the provided data for this analysis (a few sentences/plots describing your approach will suffice). What fraction of the observed users were retained?

2. Build a predictive model to help determine whether or not a user will be active in their 6th month on the system. Discuss why you chose your approach, what alternatives you considered, and any concerns you have. How valid is your model? Include any key indicators of model performance.

3. Briefly discuss the company might leverage the insights gained from the model to improve its long­term rider retention (again, a few sentences will suffice).
