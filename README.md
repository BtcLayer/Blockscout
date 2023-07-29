# Data Stitching and Analysis Readme

This repository contains three Jupyter Notebook files that are designed to work together to perform data stitching and analysis on Binance trading data.

## Raw Data Folder

The `Raw data` folder within this repository contains all the unprocessed and processed data required for the data stitching and analysis process. It is organized as follows:

- `pratham opening.csv`: This CSV file contains the raw data of opening trades.
- `pratham closing.csv`: This CSV file contains the raw data of closing trades.

Additionally, within the `Raw data` folder, there are further asset-wise subfolders that store the data after processing:

- `Year(2021).csv`: This type of file contains the CSV file with OHLC data organized on a yearly basis for that asset.
- `Year(2021)`: This type of folder contains asset-wise CSV files with OHLC data organized on a monthly basis.

The data stored in these folders is the result of the data stitching process performed by the `Stitching Data.ipynb` notebook.

## 1. Stitching Data.ipynb

**Description:**  
`Stitching Data.ipynb` is a Jupyter Notebook responsible for stitching together the monthly asset-wise data from Binance into year-wise CSV files containing OHLC (Open, High, Low, Close) data. It fetches historical data for each asset for different months, and then combines and organizes it into yearly files. The resulting CSV files provide a comprehensive collection of OHLC data for each asset for each year, making it convenient for subsequent analysis.

## 2. Final Trades.ipynb

**Description:**  
`Final Trades.ipynb` is a Jupyter Notebook designed to process opening and closing trades data in CSV format. The notebook compiles all the trades, including the trade price, asset amount, and other relevant trade details, into a final output file named `final_trades.csv`. This CSV file serves as a complete record of all the trading activity conducted over a specific period.

## 3. Basic Analysis.ipynb

**Description:**  
`Basic Analysis.ipynb` is a Jupyter Notebook responsible for conducting basic analysis on the trades data recorded in `final_trades.csv`. It calculates the Realized PnL (Profit and Loss), Net Position left after all trades, and the Average price of the position taken for each trader (identified by trader ID) and each asset. The notebook presents the analysis results in an organized manner, providing valuable insights into the trading performance of individual traders and assets.

