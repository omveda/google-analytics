# Exploring Google Analytics Data with MapD
Explore Google Analytics data with a platform like MapD to extract insights that are hard to find using Google's standard interface. Download the different metrics from Google Analytics account in CSV format and upload the data into MapD Core database. You can then use MapD Immerse platform to explore the GA metrics visually.

# Install Software Packages
- pip install --upgrade google-api-python-client
- pip install matplotlib pandas python-gflags
- pip install pymapd
- git clone https://github.com/omveda/google-analytics.git (this repo)

# Usage
- Copy the client_secrets.json corresponding to the Google Analytics Service Account to the directory you cloned this repository.
- python mapd_ga_data.py

# Workflow of the MapD-Google Analytics Application
This application is written in Python and based on the original work from Ryan Praski http://www.ryanpraski.com/python-google-analytics-api-unsampled-data-multiple-profiles/ and Google Developer’s Hello Analytics API: Python quickstart for service accounts sample program.  
Here is what the application does:
Create a service object to Google Analytics using the client_secrets.json file corresponding to the service account that was created in the prerequisite step. Traverse the Google Analytics management hierarchy and construct the mapping of website profile views and IDs. Prompt the user to select the profile view they would like to collect the data.
 
