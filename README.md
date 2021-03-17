 ### Web-scrapping-on-Wikipedia-Data-Engineering-
Using Python libraries to perform web scrapping 

#### A part of Summer Analytics project conducted by IIT Guwawati(April, 2020)

#### Purpose- TO Scrape the following table in https://en.wikipedia.org/wiki/Harvard_University using Python
![Web scrap](https://user-images.githubusercontent.com/80466173/111434878-15d94680-8726-11eb-9a42-f618d151e2c3.PNG)


#### Part 1: Inspect Your Data Source
The first step is to head over to the site you want to scrape. You’ll need to understand the site structure to extract the information you’re interested in.
In Chrome, you can open up the developer tools through the menu View → Developer → Developer Tools. You can also access them by right-clicking on the page and selecting the Inspect option

#### Part 2: Scrape HTML Content From a Page
Now that you have an idea of what you’re working with, it’s time to get started using Python. First, you’ll want to get the site’s HTML code into your Python script so that you can interact with it. For this task, you’ll use Python’s requests library

$ pip3 install requests

req = requests.get("https://en.wikipedia.org/wiki/Harvard_University")

 It retrieves the HTML data that the server sends back and stores that data in a Python object.
 
 #### Part 3: Parse HTML Code With Beautiful Soup
 It’s time to parse this lengthy code response with Beautiful Soup to make it more accessible and pick out the data that you’re interested in.
 Beautiful Soup is a Python library for parsing structured data. It allows you to interact with HTML in a similar way to how you would interact with a web page using developer tools

In an HTML web page, every element can have an id attribute assigned. As the name already suggests, that id attribute makes the element uniquely identifiable on the page. You can begin to parse your page by selecting a specific element by its ID.

Switch back to developer tools and identify the HTML object that contains the required demographic table. Explore by hovering over parts of the page and using right-click to Inspect.

 #### Part 4: Create dataframe
 
 After finding Elements by Class Name and Text Content , create a dataframe and then do the required data engineering.
 Ex- Calculating mean and standard deviation
