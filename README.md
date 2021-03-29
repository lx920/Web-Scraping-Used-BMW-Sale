# Web-Scraping-Used-BMW-Sale
This is a project of scraping used BMW's sold in the Bay area. It aims at scraping car features such as VIN, year, make, model, mileage, engines, options, packages, imperfections etc from CARVANA web page. It is a nice way to scrape data for used car price analysis.

The primary Python packaged used for the scrape is the Selenium package and chrome web driver. This is lesser-known than the most popular REQUEST and GET methods. However, it is much more powerful when there are a lot of things to control on the website.

Carvana website has a lot of things going-on in the background. To best scrape the information we want, we will need to imitate a human interaction with the website. Standard POST and GET is will not get a satisfactory result due to the complexity of the website.

The code tells the web driver to search for BMW listed around San Fransico, ZIP CODE 94103. It then download the source code of the current page. After downloading, the code tells the browser to search for the "next page" button, click it, then download the content of the next page. This iteration ends after reaching the last page. The code saves all contents to local files and extract url for all the BMW listings.

It also opens all the BMW url one by one. After opening, it scrolls all the way down to load everything that may be hidden behind "load more". Now we have everything related to every BMW ready to download!

Once all is done, the scraped items are saved in a MySQL database.
