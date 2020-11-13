# INST126_Project_3

INST126 Project 3: Log File Parser/Checker

Noah Shaw, Melody Cheng

Based upon the prompt given to us, I feel like I have a pretty good idea of how I want to approach this project.

I am going to sort all of the data based upon the user first, and then have all of the other data contained within that user.

*updated organization*

Dictionary of users(list) ----> user = Dictionary of days -----> each day is a dictionary of times -----> each time is a list of the server and activity

The use of lists allows for them to be easily sorted as well.

I'm going to define 4 functions, one for each of the insights that have been assigned.

Each of them will scrap and process the user log data based upon each of the given conditions. Since the data is organized by user and by specific days, it should not be that hard to access the right data.

The four functions are:

-sus(user)

-irr(user)

-glitch(user)

-domains()

One for each of the four types of analysis

For the analysis reports, if the user fulfills the requirements for that specific analysis, then all their user data must be included in that report

All four analysis reports must be seperate.

The four analysis files that will be generated are:

-suspicious_report.txt

-irresponsible_report.txt

-glitch_report.txt

-domain_report.txt

All the time, activity, and server information for the particular days for each user are listed in ascending order, sorted on the basis of time.

Error 1: When I first read in all the log data, every line still had the \n and \t characters present in them. In order to clean up the data, I used str.replace() to replace/remove both characters

Error 2: When I was writing the sus(user) function, I had an issue where it would sometimes double count the days if that day fulfilled both conditions. So I addded an extra condition where the loop would stop if the first condition has already been met

Error 3: When I first starting writing to the separate reports, the times would not be correctly displayed in order. So to fix that, I would go through every time in a day, insert them into a list, sort the list, and then just print the times in order using that sorted list.

