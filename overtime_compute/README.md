# Overtime Computation Package


## Project Purpose

The purpose of this Python package `compute_overtime` is to simplify the task of calculating the amount of overtime accrued over a period whilst undertaking a particular task or job. 


## Project Objective

The objective of this package is to take away the mathematical effort involved in computing the number of overtime hours and minutes from a timesheet containing the days the tasks were performed, and the start and finish times. To achieve this, the package simply takes in the following arguments:

`Inputs`
* **lunch_length** - this is the allowable length of lunch break in minutes
* **time_format** - represents the format in which the working hours are inputted in the timesheet
* **date_format** - represents the format in which the working dates are inputted in the timesheet
* **file** - the string representing the name of the timesheet

and returns the following:

`Outputs`
* total hours and minutes worked for the given period
* total hours and minutes of overtime accrued for the given period


## Project Assumptions

As this project is basically to simplify the users' task of calculating the hours worked and overtime accrued, the following assumptions have been made;

* timesheet information is saved in a csv file
* dates are formatted as '%d/%m/%Y', i.e. day/month/year
* start and finish times are formatted as '%H:%M'm i.e. hour/minute
* number of expected working hours per day is 8 hours, therefore any time over 8 hours is considered as overtime


## Expected Updates

At this stage of the project, the package is aimed at users who have carefully completed the timesheet based on the above assumptions, as there are some functional limitations to what the package can achieve. For instance, the package gives the user one chance only to go back and correct a wrongfully inputted date or time.

Further updates will have the following:

* continuously check the validity of both date and time entries. This is to avoid entries such as `18/221/992`, `09/15/2098`, `25:02`, etc
* inform user of the specific row(s) with wrongfully inputted entries
* allow user specified date and time formats
* visually compare the total hours against overtime
* to name a few


## Installation
`compute_overtime` can be installed via pip from [PyPI]('https://pypi.org/project/pandas') with the following code

pip install compute_overtime