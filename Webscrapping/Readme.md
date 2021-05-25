
Webscraping is a process in itself. As we already know what we want to webscrap from Amazon, to later produce an analysis. It is necessary to know the challanges that come in the process, which will help to understand the necessary steps in the process.
For every search result on each specific item: Laptops, Monitors, Processors, Mouse, Keyboard, DSLR Cameras, Smartphones (include Andriod & iPhones), HeadphonesHere. Amazon would provide around 80.000 products over 400 results pages.

FISRT: 
the first challange was to scrap the over 80.000 products resulting from the search for each items. For the latter the file: **create_search_urls.py** was created to retrieve all the resulting pages in the amazon search results for each item. The result from the process obtained from create_search_url.py will be stores in the **search_urls.txt** file, which will be later used to scrap the products contained on each results page.

SECOND:
after having all the result pages (**search_urls.txt**), the goal will be to webscrap the products contained on each search results page (about 20 products per page). For the latter two sub-process are necessary:
  - Using the extension such as "selector Gadget" or using the "source code" available on each website it is possible to provide the necessary information to the file **"search_yml"** which later will help extracting the selected information from the website.
  -  Having the latter file ready, it is possible to sue the file **search.py** to read every URL in the "search_url.txt" retrieving the information from these websites contained in the search_yml file, producing with it the two following files: 
    **search_output.jsonl** : with the summary information for each product and their details along with the corresponding URL for each product
    **product_urls.txt** : only the URL for each product
    
THIRD:
having the URL for each specific product and alaredy a summary of their details in the search_output.json. Now again two parallel processes will happen:
  - Using the** "products.yml"** the details wished to be retrieved are commanded with this code.
  - This YML file is read and used along with the** "product.py"**  file which will produce the last file **"product_output.jsonl"** with all the necessary data to start the data analysis.


