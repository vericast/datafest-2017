# Exercises for Data Fest Python tutorial 2017

Note: there is a set of example solutions sitting in this directory. It will be best to try the exercises on your own first and refer to these examples if you become stuck. For each exercise start from a scratch empty notebook so that all of the potential issues with solving a data science problem are apparent. What packages should you import? What cell magics should be used? How are the various pieces of functionanlity you have learned accessed?

### Data Description
The dataset contains fundamental and market ratios for some of the S&P 500 companies.  We use this dataset to analyze the different factors that affect the price to earnings (P/E) multiple of various firms.  Firms with identical earnings per share can have different price due to several factors such as profitabilty, debt load, tax regime, cash cycle, near-term and long-term growth prospects, business risks etc.  We run simple regression model to identify such factors.

Columns in the dataset

    TickerSymbol     => Stock symbol that identifies the individual firm
    EarningsPerShare => Earnings per share of the firm
    Pre-TaxROE   => Net income before tax divided by average stockholder's equity.
    AfterTaxROE  => Net income after tax divided by average stockholder's equity.
    CashRatio    => Ratio of cash plus marketable securities to current liabilities
    QuickRatio   => Ratio of cash plus marketable securities plus accounts receivable to current liabilities
    GrossMargin  => Ratio of gross profit to sales
    OperatingMargin => Ratio of operating profit to sales
    Pre-TaxMargin   => Ratio of pretax income to sales
    operating_cash_flow_margin => Ratio of operating cash flow to sales
    profit_margin    => Ratio of net income to sales
    ebit_margin      => Ratio of earnings before income and tax to sales
    capital_surplus_to_asset => Ratio of excess capital to average asset
    Goodwill_to_asset        => Ratio of goodwill to asset
    debt_to_asset  => Ratio of long term debt to average asset
    debt_to_equity => Ratio of long term debt to average stockholder's equity
    p/e => price per share to earnings per share multiple
    p/s => price per share to sales per share multiple


### 1. First Look
Employ the techniques taught in the "Taking a first look at your data" portion of the course to review the data in file relative_valuation.csv.

### 2. Univariate Stats
Using the things we have learned in the "Univariate statistics" portion of our class, review the data in relative_valuation.csv. Before you begin come up with some hypotheses about the data before you begin, and check them as you proceed.

### 3. Regression
Produce a regression model using relative_valuation.csv. The target variable is p/e (price to earning ratio) and the remainder of the data can be used as covariates. The code in baseball_regression_lasso.ipynb will be useful.


