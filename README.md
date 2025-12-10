# Trends-in-LFPL-Acquisitions
The intention of this project is to see if there is a noticeable trend for acquisitions for the LFPL.

Contents

1. lfpl_cleaning.ipynb
    This is the first notebook created to read in the code from the Louisville Metro site. The data file size is too big to push to github, but is linked here:
    I cleaned the code with notations in the markdown for my thought process. To summarize, I made the data more accesible to link it with the results of the API and removed any other form of media that was not categorized as a book.
2. lfpl_cleaned_data.csv
    This is the completed cleaned data from he lfpl_cleaning.ipynb
3. Split.ipynb
    I created a seperate notebook to split the data from the lfpl_cleaned_data.csv to split based on branch name. The intent of the original project was to see if there was any variation on aquisition based on library location. Due to time constraint, I would not have been able to pull the data from the API in time for the completion. This may be a continued endevor to continue post the end of Code:You cohort.
4. lfpl_northeast_branch.csv
    This is the csv that was read through the API.
5. API_search.ipynb
    This is a copy of the code used to call the API and feed the max number of isbns through to pull the subsequent data. If looked at a previous commit of the branch, I mistakingly touched the file during a push with the API key disclosed. This was an error on my part, but since the purpose of the API key was complete I then deactivated the account and deleted the previous file. To avoid future occurences, .gitignore will be utilized.