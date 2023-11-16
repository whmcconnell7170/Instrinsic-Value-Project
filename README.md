# Stock Intrinsic Value Analysis

This project aims to provide the user with a stock’s Intrinsic Value (IV). The Intrinsic Value is, essentially, the true value of an equity, and is calculated with current and projected financial metrics. 
This code should be used to filter out potentially risky investment opportunities and to identify conservative buy-prices.
There are two paths to run this code, the first (and most dynamic) utilizes a Finnhub API key that I have not provided. This path allows the user to search any publicly-listed company for the analysis. You can receive an API key for free at https://finnhub.io/.
The second pathway allows the user to perform the same analysis, selecting from up to four companies, provided via CSVs. The difference is that these CSVs contain data otherwise requested by the Finnhub API.


## How to Run the Code

There are two paths to run this code:

1. **Dynamic Analysis with Finnhub API Key (Not Provided):**
   - Obtain a Finnhub API key for free at [Finnhub](https://finnhub.io/).
   - Use the API key to dynamically analyze any publicly-listed company.

2. **Static Analysis with Provided CSVs:**
   - Perform the same analysis on up to four provided companies using pre-existing CSVs.
   - These CSVs contain data otherwise requested by the Finnhub API.

## Running the Program

1. After cloning the repo to your machine, navigate to the project folder in GitBash/Terminal.
2. Create a virtual environment in the project folder.
3. Activate the virtual environment.
4. Install the required packages.
5. Launch Jupyter Lab and run the program
6. When done, deactivate the virtual environment.

## Virtual Environment Commands

| Command    | Linux/Mac                       | GitBash                         |
|------------|---------------------------------|---------------------------------|
| **Create** | `python3 -m venv venv`          | `python -m venv venv`           |
| **Activate** | `source venv/bin/activate`    | `source venv/Scripts/activate`  |
| **Install** | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| **Launch Jupyter Lab** | `jupyter lab`      | `jupyter lab`                    |
| **Deactivate** | `deactivate`                   | `deactivate`                    |



## Data Dictionary

| Abbreviation         | Description                                                                                                 |
|----------------------|-------------------------------------------------------------------------------------------------------------|
| **Open Price**        | The price at which the shares were trading to start the day.                                                  |
| **Current Price**     | The current price at which the shares are trading.                                                           |
| **Price to Earnings (P/E)** | The ratio of a company's share price to its earnings per share.                                         |
| **Earnings per Share (EPS)** | The monetary value of earnings per outstanding share of common stock.                                   |
| **Five Year Projection** | An estimated growth rate based on the company’s past performance and future market estimates.           |
| **Intrinsic Value**   | The “True” price of a share, calculated using a modified version of Graham’s formula.                       |
| **Buy Price**         | The price at which one should consider purchasing the share (set to 0.75 x intrinsic value).               |
| **Recommendation**    | Indicates whether certain parameters are met and how strongly.                                              |
| **% Allocation**      | Hypothetical allocation of capital if one were to invest in their selection.                                |


## Included Features

### Loading Data
- **[Path 1 + 2]** Read TWO data sets in with an API (or use two different APIs that have data you can combine to answer new).
- **[Path 2]** Read TWO data files (JSON, CSV, Excel, etc.).

### Clean and Operate on the Data while Combining Them
- Clean your data and perform a pandas merge with your two data sets, then calculate some new values based on the new data set.
  - [Path 1] Aggregate values into a dict, then perform a pandas `from_dict` function to create a table. Later, iterate over the values in the DataFrame to yield calculated values.
  - [Path 2] The code dynamically concatenates CSVs depending on the user selection.

### Visualize / Present Your Data
- Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data.

### Best Practices: Enhance Your Project
- Utilize a virtual environment and include instructions in your README on how the user should set one up.
- Build a custom data dictionary and include it either in your README or as a separate document. This will only apply if your data set does not already have a data dictionary or if you’re building a custom data set. For an example, see the resources to the right.

### Interpretation of Your Data
- Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md. Tidy up your notebook, and make sure you don’t have any empty cells or incomplete cells that don’t do anything. Make sure it’s all functional before your final GitHub commit.


5. **Interpretation of Your Data**
   - a. Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md. Tidy up your notebook, and make sure you don’t have any empty cells or incomplete cells that don’t do anything. Make sure it’s all functional before your final GitHub commit.
