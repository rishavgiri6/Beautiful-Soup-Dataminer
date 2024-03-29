# Beautiful-Soup Dataminer

Fetches news headlines using beautiful soup and displays in JSON format.

There are mainly two ways to extract data from a website. They include:

Use the API of the website (if it exists). For example, Facebook has the Facebook Graph API which allows retrieval of data posted on Facebook.
Access the HTML of the webpage and extract useful information/data from it. This technique is called web scraping or web harvesting or web data extraction.


This project involves the implementation of a Web Scraping framework of Python called Beautiful Soup and it's usage to extract relevant news headlines from prominent sites. Relevant sorting will be implemented later using collaborative filtering recommendations.

Steps involved in web scraping:

1. Send an HTTP request to the URL of the webpage we want to access. The server responds to the request by returning the HTML content of the webpage. For this task, we will use a third-party HTTP library for python-requests.

2. Once we have accessed the HTML content, we are left with the task of parsing the data. 

3. Since most of the HTML data is nested, we cannot extract data simply through string processing. One needs a parser which can create a nested/tree structure of the HTML data. There are many HTML parser libraries available but the most advanced one is html5lib.

4. Now,all we need to do is navigating and searching the parse tree that we created, i.e. tree traversal. For this task, we will be using another third-party python library, Beautiful Soup. It is a Python library for pulling data out of HTML and XML files.
