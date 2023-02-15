# data_analysis
Code is based on work activities. The goal is to check thousands of lines of data, which is assumed to be incorrect as it was maintained manually for years. Main tasks are:

awk_date_check_epoch.sh 
monthly check on the software roadmap repository, do check/change status based on the software end of life date. Based on the EOL date of <6 months, >6 <12 months, >12 <18 month and >18 months the status of the software is changed to "expiring 3", "expiring 2" , "expiring 1" or "selling", for the software missing EOL date the confirmation request is added to the output file.

The output is used as an input to further investigation and software strategy update with the respective team
