CRYPTO CURRENCY DASHBOARD USING POWER BI
Step 1: Setting Up
1.	Create an Account
•	Go to CoinMarketCap Professional and create a free-tier account.
•	Copy and save the API key.
Step 2: Installing Power BI
•	Download and Install Power BI
•	Visit Power BI Download Page and install Power BI Desktop.
Step 3: Importing Data into Power BI
1.	Open Power BI
•	Launch Power BI Desktop.
2.	Get Data from Web
•	Click on "Get Data" and select "Web".
•	Click on "Advanced" and enter the following details:
 
URL parts: 
https://pro-api.coinmarketcap.com/v1/cryptocurrency/quotes/latest?symbol=BTC%2CADA%2CSOL%2CDOT%2CLINK%2CETH%2CREN
HTTP request header prameters type : X-CMC_PRO_API_KEY
 

•	Now first click on source and then on data record
 
•	 
•	Click on into table.
•	Next click on the expand icon on value column
 
3.	Load and Transform Data
•	Click on "Source" and then on "Data Record".
•	Click "Into Table".
•	Click on the expand icon in the "Value" column.
•	Select columns: id, name, max_supply, circulating_supply, total_supply, quote, then click "OK".
•	Expand the "Value" column again to see all data.
•	Select price, volume_change_24h, market_cap, and click "OK".
•	Change the data types of the columns based on their values. 
 
•	Select price, volume_change_24h, market_cap and click on OK.
Step 4 Creating custom columns:-
•	The api key fetches the data of live crypto market and points the data to its current value and its volume in the market. It doesn’t access to the information on our personal holdings.
•	For the purpose of this project lets create custom columns in power bi and add random values in it. We will create two columns called coins bought and dollars_spent. This will help us analyze profit percentage.
 
•	Make sure you select from all columns while adding a new column else it won’t reflect on your power bi dashboard.
•	Now we will create Custom columns called 
o	Average price
o	Current Value
o	Profit
o	ROI 
o	As the name indicates we need these custom columns which will calculate the average, current value, profit and ROI based on the current values obtained from api which are loaded into table. These transformations are useful to add more insights to our data.
o	To create a custom column click on create custom column in add columns menu.
 

•	Lets create a column called average price which is calculated as 
•	Average Price = Dollars spent / Coins Bought. Make sure you select the columns from the right pane and click on insert or enter the correct column names .

•	Similarly create other custom columns using the formulas as below.

Current value = Coins Bought * Current Price
Profit = Current Value – Dollars Spent.
ROI = Profit / Dollars Spent

After entering these and click on Home Close and Apply.

This will now load all the transformations on our data into power bi.

Step 5:- Creating the Dashboard
1.	Using Creativity

•	Create measures using DAX expressions:
•	Top Performer: Top Performer = MAX(CryptoData[Profit])
•	Worst Performer: Worst Performer = MIN(CryptoData[Profit])
2.	Adding Visualizations
•	Add visualizations such as Cards, Donut Charts, Stacked Columns, Clustered Bar Charts, and Tables.
•	Use different colors and formats to make the dashboard attractive.
Final Touches
•	Experiment with different visualizations and measures to enhance the data insights and make your dashboard more meaningful and engaging.
This guide provides a structured approach to creating a cryptocurrency dashboard in Power BI, ensuring you can visualize and analyze real-time data effectively.
