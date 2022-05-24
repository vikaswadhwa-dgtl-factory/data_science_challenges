# Data Science Challenge - User Engagement
We suggest spending 1-2 hours on this, but you're welcome to spend more or less. This is your chance to wow us with creative and rigorous solutions! Please include your code via zipped attachment via email, or as a pull request on this repository. We also accept incomplete solutions.

Please send us a brief writeup of your findings (the more concise, the better), along with any summary tables, graphs, code, or queries that can help us understand your approach. Please note any factors you considered or investigation you did, even if they did not pan out. Feel free to identify any further research or data you think would be valuable.


## Data Sources
Datasets are available under the local `./data` folder.


#### `users.csv`
A `user` table with data on 12,000 users who signed up for the product in the last two years. This table includes:
1. **`name`**: the user's name
2. **`object_id`**: the user's id
3. **`email`**: email address
4. **`creation_source`**: how their account was created. This takes on one
of 5 values:
    - **`PERSONAL_PROJECTS`**: invited to join another user's personal workspace
    - **`GUEST_INVITE`**: invited to an organization as a guest (limited permissions)
    - **`ORG_INVITE`**: invited to an organization (as a full member)
    - **`SIGNUP`**: signed up via the website
    - **`SIGNUP_GOOGLE_AUTH`**: signed up using Google
Authentication (using a Google email account for their login
id)
    - **`creation_time`**: when they created their account
    - **`last_session_creation_time`**: unix timestamp of last login
    - **`opted_in_to_mailing_list`**: whether they have opted into receiving
marketing emails
    - **`enabled_for_marketing_drip`**: whether they are on the regular
marketing email drip
    - **`org_id`**: the organization (group of users) they belong to
    - **`invited_by_user_id`**: which user invited them to join (if applicable).

#### `user_engagement.csv`
A usage summary table ("user_engagement") that has a row for each day that a user logged into the product.


## The Problem
Defining an "adopted user" as a user who has logged into the product on 3 separate days in at least one consecutive week (7 days), identify which factors predict future user adoption.
