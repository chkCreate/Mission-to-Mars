# Mission-to-Mars

## Background
Web-scraped images of Mars’s hemispheres and its titles using tools like BeautifulSoup and Splinter. Stored the scraped data on a Mongo database and Flask, used a web application to display the data, and altered the design of the web app to accommodate these images.

### Scraping

Complete initial scraping using Jupyter Notebook, BeautifulSoup, Pandas, and Requests/Splinter.

See Jupyter Notebook file titled `Mission_to_Mars.ipynb` to complete all scraping and analysis tasks. The following outlines what was scraped.

#### NASA Mars News
Scraped the [NASA Mars News Site](https://mars.nasa.gov/news/) and collect the latest News Title and Paragraph Text. Assign the text to variables that you can reference later.

#### JPL Mars Space Images - Featured Image
Scraped the JPL Featured Space Image [here](https://data-class-jpl-space.s3.amazonaws.com/JPL_Space/index.html). Used splinter to navigate the site to find the image url for the current Featured Mars Image.

#### Mars Facts
Scraped the Mars Facts webpage [here](https://galaxyfacts-mars.com) and use Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc. Use Pandas to convert the data to a HTML table string.

#### Mars Weather
Scraped the Mars Weather from twitter account [here](https://twitter.com/marswxreport?lang=en).


#### Mars Hemispheres
Scraped the USGS Astrogeology site [here](https://marshemispheres.com/) to obtain high resolution images for each of Mar's hemispheres.


### MongoDB and Flask Application
Used MongoDB with Flask templating to create an HTML page that displays all of the information that was scraped from the URLs above.

![final_app_part1.png](Images/final_app_part1.png)
![final_app_part2.png](Images/final_app_part2.png)

- - -

## Technical Elements

* Used Splinter to navigate the sites when needed and BeautifulSoup to help find and parse out the necessary data.

* Used Pymongo for CRUD applications for the database. 

* Used Bootstrap to structure the HTML template.


## Notes / Reminders
In order for the data scraping to be performed successfully with longevity, the reference websites from which the data is extracted from should be verified for working order.
