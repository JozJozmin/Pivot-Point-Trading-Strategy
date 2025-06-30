# Pivot-Point-Trading-Strategy

<br>**TABLE OF CONTENTS**<br>
<br>1. Overview
<br>2. Features
<br>3. Requirements
<br>4. Usage
<br>5. Configuration
<br>6. Results
<br>7. Contributing
<br>8. License
<br>9. Acknowledgements
<br>10. Contact


<br>**OVERVIEW** <br>
<br>This repository contains the code and documentation for a swing trading strategy developed as part of my research paper for the MSc in Financial Engineering program at WorldQuant University.<br>
<br>The strategy is designed to systematically identify profitable entry and exit points in the Indian stock market, focusing on 100 high-cap stocks listed on the National Stock Exchange (NSE) over an 8-month period.<br>
<br>By integrating Pivot Point analysis with generic price pattern evaluation of daily average net price movements, this approach effectively addresses the challenges of false signals and dynamic market behavior. The resulting strategy demonstrates a win-loss ratio of 1.24 and features a clearly defined risk management framework, with a preferred holding period of 40 days.<br>
<br>All code and supporting files in this repository were finalized in December 2023 and align with the methodology and results described in my forthcoming research paper<br>

<br>**The main objectives would be**<br>
<br>1. Evaluate the standalone effectiveness of the Pivot Indicator in the Indian stock market, specifically assessing its ability to accurately identify pivot points, support, and resistance levels to enhance overall trading decisions.<br>
<br>2. Develop a profitable trading strategy tailored to the Indian stock market, with a primary focus on identifying optimal entry and exit points that contribute to the success of trades.<br>

<br>**FEATURES**<br>
<br>* Pivot Point Calculation: Implementation of pivot point calculations for high-cap stocks listed on the NSE.
<br>* Price Pattern Analysis: Utilization of generic price pattern analysis techniques to supplement pivot point signals.
<br>* Backtesting Module: Backtesting of the trading strategy on historical data to assess its performance.
<br>* Results Analysis: Analysis of trading results including win-loss ratio, risk assessment, and holding duration.

<br>**TOOLS REQUIRED**<br>
<br> Python - See https://wiki.python.org/moin/BeginnersGuide/Download for installation.
<br> Numpy - see https://docs.scipy.org/doc for more information
<br> Pandas - see http://pandas.pydata.org for more information
<br> Matplotlib - see https://matplotlib.org/contents.html for more information
<br> yfinance - see https://pypi.org/project/fix-yahoo-finance for more information
<br>Trading View -see https://in.tradingview.com

<br>**USAGE**<br>
<br>* Open the notebook on Google Colab (include badge/link)
<br>* Or clone repo and run WQU_Capstone_Final_Day.ipynb locally
<br>* Install dependencies with pip install -r requirements.txt
<br>* Run cells sequentially to reproduce results

<br>**CONFIGUREATION**<br>

<br>**Stocks List** :Modify the file or list named stocks_list.csv (or the relevant variable in the notebook) to change which NSE stocks are included in the analysis.
<br>**Date Range** :Change the start and end dates in the notebook to analyze different time periods. For example:
                 start_date = "2022-12-31",
                  end_date = "2023-09-01" 
<br>**Holding Period** :Adjust the holding duration parameter to test different trade exit timings. Default is 40 days but can be changed to optimize performance.
<br>**Pivot Point Settings** :If your code includes any pivot point calculation options (like pivot types or methods), you can modify these parameters for different sensitivity.
<br>**Risk Parameters** :Change risk management settings such as stop-loss thresholds or position sizing rules if implemented.
Other Strategy Parameters
<br>All configuration changes can be made directly in the notebook cells before running the analysis.<br>

<br>**RESULTS**<br>
<br>The analysis identified 335 breakouts among the top 100 high-cap NSE stocks over an 8-month period. Breakouts occurred most frequently on Wednesdays (78), followed by Fridays (68) and Tuesdays (67), with Mondays having the fewest.<br>
<br>Price movement analysis across holding periods from 20 to 40 days revealed that longer holding durations increase the likelihood of positive returns but also raise exposure to larger drawdowns. The percentage of stocks with price increments rose from 62.8% at 20 days to 66.8% at 40 days, while average upward movement increased from 0.8% to 2.2%.<br>
<br>Backtesting with a 40-day holding period resulted in 295 valid trades. An initial investment of ₹25,000 per trade (totaling ₹7,375,000) produced the following outcomes:<br>
<br>Winning probability: 55.2%
<br>Win-loss ratio: 1.23
<br>Total return: ₹7,616,226
<br>ROI: 3.3%
<br>Average profit per trade: ₹818<br>
<br>The equity curve illustrates consistent growth, supporting the effectiveness of the pivot point–based swing trading strategy in the Indian stock market.<br>

