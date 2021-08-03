# Master Template
**[Justin Huang](https://github.com/Astray909)**

Master Template script written in Python3

## Requirement:
1. Python 3.8 environment under anaconda

## Testing platform:
* Windows 10 20H2

## Setup procedure:
### Recommended:
1. Launch run_gui.bat from explorer
### Or alternatively: 
1. Open either anaconda prompt or anaconda powershell prompt
2. Run `python gui.py` under anaconda prompt

## Interval test procedure:
1. Click on Import Raw Data
2. Inside the popup window, navigate to the directory containing Txxx folders
3. IMPORTANT: Must analyze T0 at least once to establish a baseline for FT comparisons
4. Select a Txxx raw data file and the script will do the rest
5. Script will output outlier result in 2_processed_data folder and retest request in 6_paperwork folder

## Parameter shift charts procedure:
1. Click on Line Plot
2. Inside the popup window, navigate to 2_processed_data directory
3. Start from import the processed csv files as instructed by the script
4. Output is stored in 2_processed_data folder as a .xlsx file

## Add new product procedure:
1. Locate and navigate to `X:\PLC\Prod Docs\Qual\qrw_script\dataAnalysis` directory
2. Open `Rel FT limits.csv` file with Microsoft Excel or any text editor
3. Add new product information (note that in Microsoft Excel formatting might be altered automatically when '-' is detected)
4. Locate and navigate to `X:\PLC\Prod Docs\Qual\qrw_script\dataAnalysis\master_template\SupportingModules` directory
5. Double click on convert.bat or run `python convert.py` under anaconda prompt
6. Select `Rel FT limits.csv` file
7. Navigate back to `X:\PLC\Prod Docs\Qual\qrw_script\dataAnalysis\master_template\SupportingModules` directory
8. Copy `products.db` file
9. Navigate to `X:\PLC\Prod Docs\Qual\qrw_script\dataAnalysis\master_template` directory
10. Paste and overwrite
11. Product info db is now up to date

## Features:
### Currently working:
1. Extended GUI
2. Product info database management
3. Data cleanup and failure detection
4. Basic parameter percentage shifts
5. Outlier detection with 3 sigma, auto exclude out of spec data
6. Compatibility for TW and OTT files
7. Automatically generate retest requests
8. One button click for data analysis and file output
9. Automatically generate dropped devices list
10. Auto removal of temporary files
11. CSV to db converter for FT limits
12. Updated individual interval test data features
### Planned:
1. Coordinating with Iman(send recent example of cp and ft data) and Chacha
2. Data visualization

## Appendix:
1. To fetch latest GIT:
    ```
    git fetch --all
    git reset --hard origin
    git pull origin main
    ```
    Or:
    ```
    git fetch --all; git reset --hard origin; git pull origin main
    ```
