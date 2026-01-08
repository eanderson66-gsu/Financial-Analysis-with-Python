# Global Financial Performance Analyzer

## Project Overview:
This project analyzes the profitability of international companies using the **Nasdaq Data Link API**. By extracting and processing financial metrics (specifically **EBITDA Margin**), this tool benchmarks corporate performance across different regions and time periods.

The analysis handles data from **20+ countries**, cleaning raw API responses, removing statistical outliers, and visualizing profit trends over a 5-year period.

## Graph Results:

### 1. Profitability by Country
> <img width="1163" height="666" alt="EBITDA Margin Distribution by Country Graph" src="https://github.com/user-attachments/assets/abbd60e5-d06a-46f5-adce-aead1445069d" />
*Description: A comparative analysis of EBITDA Margins across 15+ nations. Notable trends include higher median profitability in regions like the UK and Canada, contrasted with wider volatility in emerging markets.*

### 2. Market Trends Over Time
> <img width="1390" height="590" alt="EBITDA Margin Over Time (Smoothed) Graph" src="https://github.com/user-attachments/assets/fd6b9e72-eeff-448d-94e5-93aec445a8dd" />
*Description: A temporal analysis of profitability. The orange line represents a 3-period moving average, smoothing out quarterly noise to reveal the underlying upward trend in average corporate margins from 2012 to 2016.*

### 3. Statistical Distribution
<img width="841" height="547" alt="Dsitribution of EBITDA Margin across companies graph" src="https://github.com/user-attachments/assets/bd236ba6-09ce-4cb3-ae61-352f660211d5" />
*Description: A histogram revealing the frequency of profit margins. The data follows a normal distribution centered around 15-20%, with outliers removed during the data cleaning phase.*

## Technologies Used:
* **Language:** Python 3.x
* **Data Source:** Nasdaq Data Link API (MER/F1 Table)
* **Libraries:**
    * `Pandas` (Data Cleaning & Time-series manipulation)
    * `Matplotlib` & `Seaborn` (Statistical Visualization)
    * `Requests` (API Endpoints)

## Key Features:
* **Automated Data Pipeline:** Fetches 10,000+ rows of financial data and dynamically maps ISO country codes (e.g., 'CYM' -> 'Cayman Islands').
* **Statistical Cleaning:** Identifies and removes extreme outliers (e.g., erroneous data points from *Immutep Ltd*) to ensure accurate mean analysis.
* **Trend Smoothing:** Implements rolling window calculations to visualize long-term market direction vs. short-term noise.

## How to Run:
1.  Clone the repository:
    ```bash
    git clone [https://github.com/eanderson66-gsu/Financial-Performance-Analyzer.git](https://github.com/eanderson66-gsu/Financial-Performance-Analyzer.git)
    ```
2.  **Configuration:**
    * Create a `config.py` file in the root directory.
    * Add your Nasdaq API key: `api_key = "YOUR_KEY_HERE"`
3.  Install dependencies:
    ```bash
    pip install pandas matplotlib seaborn requests
    ```
4.  Run the notebook to generate the reports.

## 📬 Contact
* **Name:** Evan Anderson
* **Email:** andersonevan636@gmail.com
* **LinkedIn:** https://www.linkedin.com/in/evan-anderson636/
