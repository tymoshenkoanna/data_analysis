# data_analysis
Code is based on work activities. The goal is to check thousands of lines of data, which is assumed to be incorrect as it was maintained manually for years. Main tasks are:

awk_date_check_epoch.sh 
Monthly check on the software roadmap repository, do check/change status based on the software end of life date. Based on the EOL date of <6 months, >6 <12 months, >12 <18 month and >18 months the status of the software is changed to "expiring 3", "expiring 2" , "expiring 1" or "selling", for the software missing EOL date the confirmation request is added to the output file.
The output is used as an input to further investigation and software strategy update with the respective team

awk_date_status.sh
Similar excercise as above, to review software installations which have or should have an exception based on various data available in the report

id_data_check.sh
Extracting the list of all software installation running on both development and prodcution systems. The output was checked against two lists generated above, to determine if any isntallation is missing in the software roadmap and therefore is not compliant.

loop_arrays.sh
an additional checker to identify the latest version of the software installed on the production and development systems, based on the name and verions
