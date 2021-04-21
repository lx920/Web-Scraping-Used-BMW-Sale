# Used Car Price Prediction
The used car market in the US in growing very fast. Luckily, we can easily access most companies' used car inventory data by web-scraiping. As company websites list their products for sale, we can scrape specific features from the listings and make a comprehensive dataset regarding any used car inventory. The scraped data will enable us to analyze price, feature partworth, sales trend, visualizations etc. I choose to scrape BMWs sold in the Bay area.

# Language
Most of the frontend work is done by Python. It is pretty nice to use to scrape. The scraped data are saved into files and written into local MySQL database.

# Packages
Other than the more common packages for Python:

Selenium Package plays a big role in this project. It outperforms request/get when dealing with the BMW website. There were a lot of variables to control for when accessing BMW website. Selenium Package performs marvelously in micmicing a human inaction with the web-browser and enables us to scrape the information we want.

# Tackled Problems
1: Zipcode + Radius Search Post Request
2: Mimicing Mouse Click and Keyboard Entering
3: Extract Car URL from each Page Source
4: Identify Next Page buttons
5: Micmic page scrolling to load more features
6: Scrape features
7: Connect and write to MySQL database
