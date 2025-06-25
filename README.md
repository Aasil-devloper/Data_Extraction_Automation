# Data_Extraction_Automation
This repository houses a robust and flexible solution for automating the extraction of data from various sources. Designed to streamline data acquisition workflows, this tool significantly reduces manual effort, accelerates data processing, and ensures consistency in data collection.
You're seeing the raw JSON content of your .ipynb file in the GitHub code view, while the "Preview" tab renders it correctly as a Jupyter Notebook. This is expected behavior for .ipynb files on GitHub.

Here's a description for your README.md file based on the content of your Data_Extraction_Automation (1).ipynb notebook:

Data_Extraction_Automation
This repository contains a powerful Python Jupyter Notebook designed to automate the extraction of detailed business information from Google Maps using the Places API (New). It efficiently gathers data for various business categories within a specified city and provides organized output in both CSV and Excel formats.

🚀 Key Features
Automated Data Extraction: Quickly fetches information for diverse business types (e.g., mobile service centers, jewelry showrooms, car dealerships, banks, restaurants, hotels, fashion stores, etc.).

Comprehensive Business Details: Extracts key data points including:

Business Name

Full Address

Formatted Phone Number

Website URL

Customer Rating and Total Ratings

Price Level (e.g., Inexpensive, Moderate)

Business Status

Business Types (categories)

Latitude and Longitude for mapping

Flexible Dual Output:

CSV Files: Generates individual CSVs for each business category, a combined CSV of all data, and a summary CSV.

Excel Workbook (.xlsx): Creates a single, comprehensive Excel file containing multiple sheets for organized viewing. This includes:

All_Businesses: A sheet with all combined extracted data.

Summary: A sheet providing statistics and insights (e.g., total count, percentage with phone/website, average rating per category).

Individual sheets for each searched business category.

Intelligent Data Handling: Includes mechanisms for cleaning data by removing low-quality entries and handling duplicates.

Interactive Command-Line Interface: Guides the user through the process, prompting for necessary inputs like the API key and city name.

Detailed API Key Setup Guide: Provides clear, step-by-step instructions within the notebook on how to obtain, enable, and securely restrict your Google Maps API key in the Google Cloud Console to prevent REQUEST_DENIED errors.

⚙️ Technologies Used
Python: The core programming language.

googlemaps library: For interacting with the Google Places API (New).

pandas: For data manipulation and creating DataFrames.

openpyxl: (Optional but Recommended) For full Excel file (.xlsx) generation capabilities.

🚀 Getting Started
To use this tool, follow these steps:

Clone this repository:

Bash

git clone https://github.com/YourUsername/Data_Extraction_Automation.git
cd Data_Extraction_Automation
(Replace YourUsername with your actual GitHub username and adjust the folder name if necessary).

Install Required Python Packages:
Open your terminal or command prompt in the project directory and run:

Bash

pip install --upgrade googlemaps pandas openpyxl
This ensures you have all necessary libraries, including openpyxl for Excel output.

Google Maps API Key Setup (Crucial!):
This tool requires a Google Maps API Key with the 'Places API' enabled and billing activated in your Google Cloud Console. Follow the detailed instructions provided in the initial output of the Jupyter Notebook (Data_Extraction_Automation (1).ipynb) to correctly set up and restrict your API key.

🌐 Go to Google Cloud Console: https://console.cloud.google.com

📁 Select or Create a Project

💳 Enable Billing for your project

🔧 Enable 'Places API'

🔑 Create or Get Your API Key

🔒 Highly Recommended: Restrict your API key to 'Places API'.

Run the Jupyter Notebook:

Navigate to the cloned directory in your terminal.

Start Jupyter Notebook: jupyter notebook "Data_Extraction_Automation (1).ipynb"

This will open the notebook in your web browser. Execute the cells sequentially.

The notebook will prompt you to enter your API key and the city you wish to search.

📂 Output Files
The script will generate output files in the same directory where the notebook is run. Filenames will include the city and a timestamp for easy identification (e.g., Mumbai_businesses_20250625_113000_complete.xlsx).

CSV Files:

[city]_businesses_[timestamp]_all_data.csv

[city]_businesses_[timestamp]_summary.csv

[city]_businesses_[timestamp]_[Business_Type].csv (e.g., Mumbai_businesses_20250625_113000_Airtel_Service_Centers.csv)

Excel File:

[city]_businesses_[timestamp]_complete.xlsx

This single file contains multiple sheets: All_Businesses, Summary, and individual sheets for each business category.

Contributing
(Optional section - if you want others to contribute)
We welcome contributions! Please feel free to open issues or submit pull requests.

License
(Optional section - specify your license)
This project is licensed under the MIT License - see the LICENSE file for details.
