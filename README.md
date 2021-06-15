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
4. Select a Txxx folder and the script will do the rest
5. Script will output outlier result in 3_interval_test folder and retest request in 6_paperwork folder

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
1. Data formatting
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
