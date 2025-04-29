# Scraping School
Everything you need to get started with web scraping, beginning with simple examples and moving on to more complex ones.

Python is arguably the most suitable programming language for web scraping because of its ease and a plethora of open source libraries. Some libraries make it easy to extract the data and to transform the data into any format needed, be it a simple CSV, to a more programmer-friendly JSON, or even save directly to the database.

Web scraping with Python is so easy that it can be done in as little as 5 lines of code.

## Web Scraping in 5 Lines of Code
Write these five lines in any text editor, save as a .py file, and run with Python. Note that this code assumes that you have the libraries installed. More on this later.
```code
import requests
from bs4 import BeautifulSoup
response = requests.get("https://en.wikipedia.org/wiki/Web_scraping")
bs = BeautifulSoup(response.text,"lxml")
print(bs.find("p").text)
```
This will go to the Wikipedia page for the web scraping and print the first paragraph on the terminal. This code shows the simplicity and power of Python. You will find this code in webscraping_5lines.py file.