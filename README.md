# CMSE202_HonorsProject

This repository holds the honors project of William Chettleburgh. The project aims to analyze the responses from SOCT data in conjuction with data from msugrades.com in order to answer the following questions:
* Is there a correlation between the responses students provide on SOCT survey questions and the grades they receive?
* How do the SOCT survey responses vary between subjects? Do certain subjects receive more favorable responses, on average?
* How do the SOCT survey responses and average grades vary between course levels?

For a detailed description of the project (along with the code and analysis), see Final_Project.ipynb. This file describes in detail how to run the code. As an overview, here are some key steps:
* Install any packages in the import cell that are not currently installed. Note that OLSplots is by Jason Sadowski, and a modified copy of the code is present in this repository.
* The webscraping does not need to be performed; instead, the data can be loaded from the output folder. Simply run all the cells excluding the one beginning with the initialization of soct_driver up until the one beginning with a call to log_in.
* If webscraping is to be performed, a proper webdriver agreeing with the user's browser must be added to the directory containing the notebook. The name of the driver should be changed in the initialization of soct_driver to match the filename of the driver. Then, valid credentials must be passed to the log_in function when it is called. If the full site is to be scraped, the argument "True" in subjects_iterate should be changed to "False".
* If any errors occur while performing the webscraping, it may be necessary to modify the starting index of the loop in subject_iterate in order to restart the scraper from where the user left off. More details of this are provided in Final_Project.ipynb.
* The rest of the code should be run in order (running the cells out of order may cause errors).

Any questions should be directed to chettleburghw@gmail.com.