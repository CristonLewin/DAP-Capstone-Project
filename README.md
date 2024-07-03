# DAP-Capstone-Project

This project analyzes the UK Housing Property Index dataset and performs various data analysis tasks. The project is implemented in Google Colab environment.

# Prerequisites
Before you begin, ensure you have a Google account and access to Google Colab.

# Dataset
The Dataset used in this project is pulled from a shared OneDrive folder so you do not necessarily need to download the dataset however, the dataset will be included in the repository just incase you are having issues accessing the shared folder.

# Running Codes
To run the code please download the Cap_Project.ipynb file and upload to the colab environment.

# Importing dataset (if necessary)

If the access to the shared folder does not work, replace the cell that contains the below code:

///////////////////////////////////////////////////////////
resid1 = '86516661A665CDF3%2157880'
authkey = '%21AEKz7uhL6B7MUFg'
url1_excel = ('https://onedrive.live.com/download?'
              + 'resid=' + resid1
              + '&authkey=' + authkey
              + '&em=2&app=Excel')

UK_HPI = pd.read_excel(url1_excel)
///////////////////////////////////////////////////////////

With:
//////////////////////////////////////////////////////////
from google.colab import files
uploaded = files.upload()

UK_HPI = pd.read_csv('UK_Housing_Property_Index.csv')
/////////////////////////////////////////////////////////
