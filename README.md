We have chosen H1-B visa petitions data set for the years 2015 and 2016 which consists of status of the case, employer’s name, job title, etc.
Our data source contains 469 Mega Bytes of data with more than 1,000,000 records. The file extension is .csv(Excel). The format of dataset is structured.
Volume is the main big data problem for this data set.

Volume: Volume of the data set is 469 Mb. There are over 1,000,000 records.

Variety: It is a structured data stored in excel file with .csv extension.

Velocity: Data is between 2015 and 2016.

Map Reduce Problems:

To find which professional background has maximum acceptance for the year 2015

To find which professional background has minimum acceptance for the year 2016

Mapper Input:

                JOB_TITLE                                               YEAR

                CHIEF OPERATING OFFICER                         2015

Mapper output/Reducer Input:  Mapper function will produce the Intermediate key values pairs. The format is shown below.

                (CHIEF OPERATING OFFICER, 1)

Reducer Output:  Reducer will produce the following sample output.

      CHIEF OPERATING OFFICER 789, PRESIDENT 774, . . .

Language: Python.

We will be processing both text & numeric and there is no need for cleaning the data since it is well structured.

*****

Pulling the repo:
$ git clone https://github.com/Shashank7T/DDIS---P12---H1B.git

*****
Executing the code:
$ mapper.py reducer.py output.txt