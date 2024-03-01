## Stock Price Monitor with SMS Alerts

This project uses Python to monitor the daily closing price of a  stock and send an SMS notification if the change between two days exceeds a threshold.

### Features

* Fetches daily stock data using the Alpha Vantage API.
* Calculates the percentage change in price between yesterday and the day before.
* Sends an SMS notification with the percentage change and a relevant news headline if the change is greater than 5% (positive or negative).
* Retrieves news articles about the company from the News API.

### Usage

1. **Requirements:**
    * Python 3.x
    * `requests` library
    * `datetime` library
    * `twilio` library (requires a Twilio account)
2. **Installation:**
    ```bash
    pip install requests twilio
    ```
3. **Configuration:**
    * Replace the following placeholders in the code with your own information:
        * `STOCK`: Stock symbol (e.g., "TSLA")
        * `COMPANY_NAME`: Company name (e.g., "Tesla Inc.")
        * `alphavantage_apikey`: Your Alpha Vantage API key ([https://www.alphavantage.co/](https://www.alphavantage.co/))
        * `newsapi_apikey`: Your News API key ([https://newsapi.org/](https://newsapi.org/))
        * `account_sid`: Your Twilio account SID
        * `auth_token`: Your Twilio auth token
        * `from_phone_number`: Your Twilio phone number
        * `to_phone_number`: The phone number to receive SMS notifications
4. **Run the script:**
    ```bash
    python my_solution.py
    ```

