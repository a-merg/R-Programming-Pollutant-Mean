# R Programming Pollutant Mean Function
Zip file containing data:

    specdata.zip [2.4MB]

The zip file contains 332 comma-separated-value (CSV) files containing pollution monitoring data for fine particulate matter (PM) air pollution at 332 locations in the United States. Each file contains data from a single monitor and the ID number for each monitor is contained in the file name. For example, data for monitor 200 is contained in the file "200.csv". Each file contains three variables:

    Date: the date of the observation in YYYY-MM-DD format (year-month-day)
    sulfate: the level of sulfate PM in the air on that date (measured in micrograms per cubic meter)
    nitrate: the level of nitrate PM in the air on that date (measured in micrograms per cubic meter)

For this programming assignment you will need to unzip this file and create the directory 'specdata'. Once you have unzipped the zip file, do not make any modifications to the files in the 'specdata' directory. In each file you'll notice that there are many days where either sulfate or nitrate (or both) are missing (coded as NA). This is common with air pollution monitoring data in the United States.

Write a function that calculates the mean of a pollutant (sulfate or nitrate) across a specified list of monitors. The function takes three arguments: 'directory', 'pollutant', and 'id'. Given a vector monitor ID numbers, the function reads that monitors' particulate matter data from the directory specified in the 'directory' argument and returns the mean of the pollutant across all of the monitors, ignoring any missing values coded as NA.
