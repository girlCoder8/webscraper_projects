## Web scraping with Python best practices

- Your first web scraper should be basic so that you gain an understanding of the different libraries and how each of them are used. 


- Scrape several URLs in one go. There are many ways to implement such a feature. One of the simplest options is to simply repeat the code above and change URLs each time. That would be quite boring. Build a loop and an array of URLs to visit.


- Another option is to create several arrays to store different sets of data and output it into one file with different rows. Scraping several types of information at once is an important part of e-commerce data acquisition.


- Once a satisfactory web scraper is running, you no longer need to watch the browser perform its actions. Run headless versions of either Chrome or Firefox browsers and use those to reduce load times.


- Create a scraping pattern. Think of how a regular user would browse the internet and try to automate their actions. New libraries will definitely be needed. Use import time and from random import randint to create wait times between web pages. Add scrollto() or use specific key inputs to move around the browser. It’s nearly impossible to list all the possible options when it comes to creating a scraping pattern.


- Create a monitoring process. Data on certain websites might be time (or even user) sensitive. Try creating a long-lasting loop that rechecks certain URLs and scrapes data at set intervals. Ensure that your acquired data is always fresh.


- Make use of the Python Requests library. Requests is a powerful asset in any web scraping toolkit as it allows to optimize HTTP methods sent to servers.


- Configure a Python requests retry strategy that automatically retries failed requests with specified error status codes.


- Once you get the hang of the basics, utilize an asynchronous Python library to make multiple requests simultaneously. Two common asynchronous libraries come to mind – asyncio and aiohttp.


- Finally, integrate proxies into your web scraper. Using location-specific request sources allows you to acquire accurate data that might otherwise be inaccessible.