# crypto_currency_dashboard_pwoerbi
Building a crypto currency dashboard using data from "coinmarketcap"
## **Step 1: Setting Up**

1. **Create an Account**
    - Go to [CoinMarketCap Professional](https://pro.coinmarketcap.com/account) and create a free-tier account.
    - Copy and save the API key.

## **Step 2: Installing Power BI**

- Download and Install Power BI
- Visit [Power BI Download Page](https://powerbi.microsoft.com/en-us/downloads/) and install Power BI Desktop.

## **Step 3: Importing Data into Power BI**

1. **Open Power BI**
- Launch Power BI Desktop.
1. **Get Data from Web**
- Click on "Get Data" and select "Web".
- Click on "Advanced" and enter the following details:

- **URL parts:**

https://pro-api.coinmarketcap.com/v1/cryptocurrency/quotes/latest?symbol=BTC%2CADA%2CSOL%2CDOT%2CLINK%2CETH%2CREN

**HTTP request header prameters type :** X-CMC_PRO_API_KEY


