# Time Series Analysis of Google Stock Data

### Key Steps in the Notebook
1. **Install yfinance**: Installs the `yfinance` library, which is used to fetch financial data from Yahoo Finance.
2. **Import yfinance**: Imports the `yfinance` library for use in the notebook.
3. **Download Stock Data**: Retrieves historical stock data for Google (GOOG) from January 1, 2010, to January 1, 2025, including columns for Open, High, Low, Close, and Volume.
4. **Inspect Data**: Displays the first five rows of the downloaded data using the `.head()` method to confirm successful retrieval and explore the dataset's structure.

### Purpose
This notebook serves as an introductory example for working with financial time series data in Python. It can be extended for further analysis, such as visualizing stock price trends, calculating returns, or building predictive models.

## Prerequisites
- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `yfinance` (installed within the notebook)
  - `pandas` (comes pre-installed with `yfinance` dependencies)

## Installation
1. Clone or download this repository to your local machine.
2. Ensure you have Python 3.x installed.
3. Open the `Time series.ipynb` notebook in Jupyter Notebook or JupyterLab.
4. Run the first cell to install `yfinance` if it is not already installed:
   ```bash
   !pip install yfinance
   ```

## Usage
1. Open the `Time series.ipynb` notebook in a Jupyter environment.
2. Run the cells sequentially to:
   - Install and import `yfinance`.
   - Download Google stock data for the specified date range.
   - Display the first five rows of the data.
3. Modify the ticker symbol (e.g., replace "GOOG" with another stock ticker) or date range as needed for your analysis.
4. Extend the notebook by adding cells for data visualization (e.g., using `matplotlib` or `seaborn`) or additional time series analysis.

## Example Output
The notebook outputs a pandas DataFrame with the following structure (first five rows):

| Date       | Close     | High      | Low       | Open      | Volume      |
|------------|-----------|-----------|-----------|-----------|-------------|
| 2010-01-04 | 15.536651 | 15.605068 | 15.474429 | 15.541608 | 78541293    |
| 2010-01-05 | 15.468233 | 15.563671 | 15.407499 | 15.547310 | 120638494   |
| 2010-01-06 | 15.078297 | 15.514587 | 15.031197 | 15.514587 | 159744526   |
| 2010-01-07 | 14.727282 | 15.121431 | 14.691337 | 15.106557 | 257533695   |
| 2010-01-08 | 14.923613 | 14.954103 | 14.603584 | 14.675224 | 189680313   |

## Notes
- The `yfinance` library fetches data from Yahoo Finance, which may occasionally have downtime or changes in API behavior. Ensure an active internet connection when running the notebook.
- The date range in the notebook extends to January 1, 2025. If running after this date, update the `end` parameter in the `yf.download` function to a future date or the current date.
- The notebook assumes the default settings for `yfinance`, where `auto_adjust=True` adjusts prices for stock splits and dividends.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or contributions, please open an issue or submit a pull request on the repository.
