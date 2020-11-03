# INST126_Project_3

INST126 Project 3: Log File Parser/Checker

Noah Shaw, Melody Cheng

Based upon the prompt given to us, I feel like I have a pretty good idea of how I want to approach this project.

I am going to sort all of the data based upon the user first, and then have all of the other data contained within that user.

*updated organization*

Dictionary of users(list) ----> user = Dictionary of days -----> each day is a dictionary of times -----> each times is a list of the server and activity

The use of lists allows for them to be easily sorted as well.

I think I'm going to define 4 functions, one for each of the insights that have been assigned.

Each of them will scrap and process the user log data based upon each of the given conditions. Since the data is organized by user and by specific days, it should not be that hard to access the right data.

The four functions are:
-sus(user)
-irr(user)
-glitch(user)
-domains()

One for each of the four types of analysis

For the analysis reports, if the user fulfills the requirements for that specific analysis, then all their user data must be included in that report

All four analysis reports must be seperate.
