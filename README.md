# Web_Scraping-and-MongoDB

In this assignment, a web application scraped data from multiple sources, stored them into a document database and then published it to html page.

Sources:
- https://mars.nasa.gov/news/ source data for all Mars news using BeautifulSoup, splinter, pandas in a jupyter notebook.
- https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars source url for Mars image.
- https://twitter.com/marswxreport?lang=en source for tweet data.
- https://space-facts.com/mars/ to gather the facts table about Mars
- https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars to get the images of 4 hemispheres of Mars

Flask:
- A python script to run all of the scraping code was designed and all of the scraped data was put into one Python dictionary.

- '/scrape' route which will import the Python script and call the scrape function was created.

 MongoDB:
 - A new database and a new collection was created.
 - All of the scraped data was stored in the above created database.
 - Root route / that will query the database and pass the mars data into HTML template was created.

 HTML and BootStrap:
 - Finally a HTML file called 'index.html' was created that displayed all of the data in HTML elements.