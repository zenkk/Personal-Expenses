# Personal-Expenses
Combines Monefy data to track expenses, sending reminders and graphs to your mobile.

## About
I've been using the Monefy App to keep track of my daily expenses since it's easy to immediately add expenses and decided to write an R script to automatically send messages and graphs to my mobile at the end of every week and month. These remind me to keep within my budget by showing how much I've spent and utilise the behaviour modification technique of intermittent reinforcement through a fixed interval schedule (i.e. weekly & monthly) to encourage behaviour maintenance/change. This is my beginner attempt at learning R through a personal project. 

## What it does  
1. Gets the Monefy .csv and Cashback .xlsx files from a folder in your computer
2. Prepares the data for analysis
3. Summarises the combined data into a monthly format 
4. Creates new dataframe for calculating next month's budget 
5. Generates a graph showing monthly expenditure and budget (to view weekly)
6. Generates a graph showing a breakdown of the monthly expenditure (to view weekly)
7. Sends graphs and messages to your Slack Account
8. Determines if budget goals met, sends corresponding message
 
## To use this
1. Download Monefy's mobile app
2. Set up a Slack Account and download the mobile app
3. Set up Windows Task Scheduler to run the R scripts at the desired time 
    e.g. every Sun evening/end of each month 

## Graphs
Code generates these two graphs to show expenditure over time to quickly identify areas of high expenditure and changes in spending. 
Also shows monthly budget, taking excess/deficit from previous months into account. 

![both](https://user-images.githubusercontent.com/35417392/34953625-59be27a2-fa58-11e7-935f-8226fd2ae85d.png)

## Caveats
1. If using the free Monefy App, the .csv file needs to be exported from the app to a folder on the computer. I sync mine to my OneDrive on the day I run the R script.
2. As Slack is used to send the graphs and messages to the mobile, the computer needs to be connected to the Internet while running the R script for Slack to work.
