
Webscraping is a process in itself. As we already know what we want to webscrap from Amazon, to later produce an analysis. It is necessary to know the challanges that come in the process, which will help to understand the necessary steps in the process.
For every search result on each specific item: Laptops, Monitors, Processors, Mouse, Keyboard, DSLR Cameras, Smartphones (include Andriod & iPhones), HeadphonesHere. Amazon would provide around 80.000 products over 400 results pages.

First: 
the first challange was to scrap the over 80.000 products resulting from the search for each items. For the latter the file: **create_search_urls.py** was created to retrieve all the resulting pages in the amazon search results for each item. The result from the process obtained from create_search_url.py will be stores in the **product_urls.txt** file, which will be later used to scrap the products contained on each results page.

Second:
after having all the result pages (**product_urls.txt**), the goal will be to scrap the products contained on each search results page. 
