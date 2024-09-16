# ETL_USING_PYTHON
## Introduction
In this project, we will build an ETL (Extract, Transform, Load) pipeline using the Spotify API. The pipeline will retrieve data from the Spotify API, transform it into the desired format, and load it into multiple storage locations, including local storage, a PostgreSQL database, and cloud services such as AWS S3 and Azure Data Lake.

 ## Problem Statement
Build a data pipeline to extract, process, and store the top 50 trending Telugu songs from the Spotify API. The pipeline should be capable of fetching the data, transforming it into a structured format, and storing it in multiple locations, including local storage, a database, AWS S3, and Azure Data Lake for further analysis.

## Architecture
![Architecture Diagram](https://github.com/vinay-github-2024/ETL_USING_PYTHON/blob/main/etl_using_python_architecture.png)

## Steps Involved
  - #### Integrating with Spotify API and Extracting Data:
    - Extract the unstructured data from Spotify's API using proper authentication methods for further processing.
  - #### Data Processing in Jupyter Notebook:
    - Create a Python script to connect to the Spotify API.
    - Transform the unstructured data into a structured format using Python and Pandas.
  - #### Load the Structure data into Local, A Database, AWS S3 and Azure Data Lake Integration:
    - Stored the transformed data in Four locations: locally for immediate access, on PostgreSQL database, on AWS S3 for scalable and secure cloud storage, and in Azure Data Lake for long- term storage and advanced analytics.
## Step-by-Step Approach
  - Visit the Spotify Developers website, create an account, and then create an app to obtain the credentials like client_id and client_secret.
  - **Explore the Spotify library using python:**
      - **Import Necessary Libraries:** Begin by importing the libraries required for making authenticated requests to Spotify's API. Specifically, you'll use spotipy, a lightweight Python library for the Spotify Web API.
      - **Set Up Authentication:** Use the "SpotifyClientCredentials" from "spotipy" to authenticate your requests. This will involve setting up your client credentials to access Spotify's data.
  - **Extract, Transform, and Convert Data from Spotify API**
      - **Extract data:** Use the spotipy library to make requests to the Spotify API and retrieve the necessary data. This include information about tracks, albums, or artists.
      - **Transform data:** Processed and cleaned the extracted data and organized it into a structured format, handling missing values, or selecting relevant fields.
      - **Convert to DataFrame:** Use the pandas library to convert the transformed data into a DataFrame for easier manipulation and analysis.
  - Convert the Dataframe to csv by using the "to_csv" method provided by pandas and store the csv file on Local Storage.
  - Import sqlalchemy to connect with PostgreSQL and store Data
  - Import Necessary Libraries to Authenticate AWS and Azure Storage Accounts
  - Upload the CSV File to AWS S3 and Azure Data Lake.

## Conclusion
We have successfully extracted the top 50 trending Telugu songs, including details about the performing artists and the movies they are associated with. This information has been organized into separate tables, allowing for comprehensive analysis and insights into the music trends.

  
