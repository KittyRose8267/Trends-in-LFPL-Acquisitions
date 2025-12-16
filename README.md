Trend on Louisville NorthEast Library Aquisition in 2022

SUMMARY:

The intention of this project is to see if there is a noticeable trend for acquisitions for the LFPL. While the original intent was to compare branches and see trends of aquisition over a period of time. The data was not public accesible by Louisville Metro for this analysis. Instead, I chose to focus on this specific year and analyze the different genres purchased, and how much money was spent per genre.


DATA USED:

First Data Source: https://data.louisvilleky.gov/datasets/6f00d1da8c374ff48d1f594155c341df_0/explore

Second Data Source: I accessed an API to pull specific information in relation to the ISBN of the book: https://isbndb.com/isbn-database


How to use:

In terminal create a virtual environment: python -m venv venv
Activate environment: source venv/scripts/activate
Install the packages from requirements.txt: pip install -r requirements.txt

Start in the lfpl_cleaning.ipynb notebook and run, selecting venv as the kernal.



Contents:

1. # lfpl_cleaning.ipynb #
    This is the first notebook created to read in the code from the Louisville Metro site.

    I cleaned the code with notations in the markdown for my thought process. To summarize, I made the data more accesible to link it with the results of the API and removed any other form of media that was not categorized as a book.

     # lfpl_cleaned_data.csv #
    This is the completed cleaned data from he lfpl_cleaning.ipynb

    # Split.ipynb #
    I created a separate notebook to split the data from the lfpl_cleaned_data.csv to split based on branch name. The intent of the original project was to see if there was any variation on aquisition based on library location. Due to time constraint, I would not have been able to pull the data from the API in time for the completion. This may be a continued endeavor to continue post the end of Code:You cohort.

    # lfpl_northeast_branch.csv #
    This is the CSV that was read through the API.

2.  # API_search.ipynb #
    This is a copy of the code used to call the API and feed the max number of isbns through to pull the subsequent data. If looked at a previous commit of the branch, I mistakingly touched the file during a push with the API key disclosed. This was an error on my part, but since the purpose of the API key was complete I then deactivated the account and deleted the previous file. To avoid future occurences, .gitignore will be utilized.

    # Cleaned Data Folder #
    All csvs that were saved info from the API function were saved into this folder to later be concatenated.

    # NE_ISBN_cleaning.ipynb #
    This is the notebook where I combined all of the csvs from the API, and then did the data cleaning and wrangling. According to the markdowns.

3. # library erd.jpeg #
    I touched up the ERD from earlier and fixed it with the specific information for the columns based on the name in the df.
    
4. # library_db.ipynb #
    This is the notebook where I made the connection to build the database and to import the data from the two csvs. 

Final Findings
