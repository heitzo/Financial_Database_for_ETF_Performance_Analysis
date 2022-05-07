# Financial_Database_for_ETF_Performance_Analysis
Build a financial database and web application by using SQL, Python, and the Voilà library to analyze the performance of a fintech ETF.

## Background
In recent years, finance has had an explosion in passive investing. Passive investing means that you invest in a basket of assets that’s called an exchange-traded fund (ETF). This way, you don’t spend time researching individual stocks or companies or take the risk of investing in a single stock. ETFs offer more diversification.

In this project, you’ll build a financial database and web application by using SQL, Python, and the Voilà library to analyze the performance of a hypothetical fintech ETF.

## What You're Creating

For this assignment, you need to create and submit the following deliverables:
1. A Jupyter notebook that contains the following:
2. Your analysis of the ETF data that a SQL database stores
3. Professionally styled and formatted interactive visualizations
4. A screenshot or video of the web application that you created by deploying your Jupyter notebook via the Voilà library
5. Upload the Jupyter notebook for this assignment to your GitHub repository. Make sure to update the READ.md file to include an explanation of your project, the screenshot or video of your deployed application, and any other information that’s needed to interact with your notebook and web application.


## Instructions:
1. Analyze a single asset in the ETF
2. Optimize data access with advanced SQL queries
3. Analyze the ETF portfolio
4. Deploy the notebook as a web application

## 1. Analyze a single asset in the ETF
For this part of the assignment, you’ll use SQL queries with Python, Pandas, and hvPlot to analyze the performance of a single asset from the ETF.
Complete the following steps:
1. Write a SQL SELECT statement by using an f-string that reads all the PYPL data from the database. Using the SQL SELECT statement, execute a query that reads the PYPL data from the database into a Pandas DataFrame.
2. Use the head and tail functions to review the first five and the last five rows of the DataFrame. Make a note of the beginning and end dates that are available from this dataset. You’ll use this information to complete your analysis.
3. Using hvPlot, create an interactive visualization for the PYPL daily returns. Reflect the “time” column of the DataFrame on the x-axis. Make sure that you professionally style and format your visualization to enhance its readability.
4. Using hvPlot, create an interactive visualization for the PYPL cumulative returns. Reflect the “time” column of the DataFrame on the x-axis. Make sure that you professionally style and format your visualization to enhance its readability.

## 2. Optimize data access with advanced SQL queries
For this part of the assignment, you’ll continue to analyze a single asset (PYPL) from the ETF. You’ll use advanced SQL queries to optimize the efficiency of accessing data from the database.
Complete the following steps:
2. Access the closing prices for PYPL that are greater than 200 by completing the following steps:
3. Write a SQL SELECT statement to select the dates where the PYPL closing price was higher than 200.0.
4. Using the SQL statement, read the data from the database into a Pandas DataFrame, and then review the resulting DataFrame.
5. Select the “time” and “close” columns for those dates where the closing price was higher than 200.0.
6. Find the top 10 daily returns for PYPL by completing the following steps:
7. Write a SQL statement to find the top 10 PYPL daily returns. Make sure to do the following:
    1. Use SELECT to select only the “time” and “daily_returns” columns.
    2. Use ORDER to sort the results in descending order by the “daily_returns” column.
    3. Use LIMIT to limit the results to the top 10 daily return values.
    4. Using the SQL statement, read the data from the database into a Pandas DataFrame, and then review the resulting DataFrame.
    
## 3. Analyze the ETF portfolio
For this part of the assignment, you’ll build the entire ETF portfolio and then evaluate its performance. To do so, you’ll build the ETF portfolio by using SQL joins to combine all the data for each asset.
Complete the following steps:
1. Write a SQL query to join each table in the portfolio into a single DataFrame. To do so, complete the following steps:
2. Use a SQL inner join to join each table on the “time” column. Access the “time” column in the GDOT table via the GDOT.time syntax. Access the “time” columns from the other tables via similar syntax.
3. Using the SQL query, read the data from the database into a Pandas DataFrame. Review the resulting DataFrame.
4. Create a DataFrame that averages the “daily_returns” columns for all four assets. Review the resulting DataFrame.
5. Use the average daily returns in the etf_portfolio_returns DataFrame to calculate the annualized returns for the portfolio. Display the annualized return value of the ETF portfolio.
6. Use the average daily returns in the etf_portfolio_returns DataFrame to calculate the cumulative returns of the ETF portfolio.
7. Using hvPlot, create an interactive line plot that visualizes the cumulative return values of the ETF portfolio. Reflect the “time” column of the DataFrame on the x-axis. Make sure that you professionally style and format your visualization to enhance its readability.

## 4. Deploy the Notebook as a Web Application
For this part of the assignment, complete the following steps:
1. Use the Voilà library to deploy your notebook as a web application. You can deploy the web application locally on your computer.
2. Take a screen recording or screenshots to show how the web application appears when using Voilà. Include the recording or screenshots in the README.md file for your GitHub repository.