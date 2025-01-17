# StockTicker
This project has been updated to use the Rapid-API Yahoo finance API. For the free tier there is a limit of 500 API calls a month, so modifications have been made to not hit this limit.

This project uses an ESP8266 and two 8x32 LED matrix panels (WS2812B LEDs) to show current stock information. The user is able to update the Wifi information through the included file or via the serial port. The user can also add or remove different stock symbols by going to the IP address that is shown when the ESP8266 connects. All tickers are queried every 30 minutes to limit API calls. Along with this, the stock ticker is a clock outside of business hours.

![Alt Text](Media/StockTickerDemo.gif) 

# How to use
To use this project, you will need an API key from the YH Finance API on RapidAPI.

Once you have the API key, you will need to add the following lines with the right information to the keys header file included.

```
// Wifi
String ssid = "SSID_NAME";
String password = "WIFI_PASSWORD";

// API key
#define X_RAPID_KEY "API_KEY"
```
