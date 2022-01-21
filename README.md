# web-scraping-challenge Web Scraping 

![Screen Shot 2022-01-20 at 9 44 18 PM](https://user-images.githubusercontent.com/33403205/150458603-d092ea3d-1bec-4630-bf28-24cb8be64d4f.png)


## Step 1 - Scraping

Utilized Jupyter Notebook, BeautifulSoup, Pandas, and Requests/Splinter for Scraping task.

* Create a Jupyter Notebook file called `mission_to_mars.ipynb` and use this to complete all of your scraping and analysis tasks. The following outlines what you need to scrape.(https://redplanetscience.com/)
### NASA Mars News
![Screen Shot 2022-01-20 at 9 45 18 PM](https://user-images.githubusercontent.com/33403205/150458612-16186ca1-f45e-4500-be7b-ca981124915b.png)

* 

* Splinter was used to navigate the site [here](https://spaceimages-mars.com) to find the image url for the current Featured Mars Image and assigned the url string to a variable named `featured_image_url`.


### Mars Facts
* Pandas was used  to convert the data to a HTML table string and to scrape the table containing facts about the planet including Diameter, Mass, etc.

![Screen Shot 2022-01-20 at 9 47 41 PM](https://user-images.githubusercontent.com/33403205/150458621-6ec87da3-00ac-45f1-aded-6b1f5616b2a3.png)


### Mars Hemispheres

* Visit the astrogeology site [here](https://marshemispheres.com/) to obtain high resolution images for each of Mar's hemispheres.


## Next  - MongoDB and Flask Application

 MongoDB with Flask templating to create a new HTML page that displays all of the information that was scraped from the URLs above.

* Converted  Jupyter notebook into a Python script called `scrape_mars.py` with a function called `scrape` that will execute all of your scraping code from above and return one Python dictionary containing all of the scraped data.

* Next, created a route called `/scrape` that will import your `scrape_mars.py` script and call your `scrape` function.

  * Store the return value in Mongo as a Python dictionary.

* Created a root route `/` that will query your Mongo database and pass the mars data into an HTML template to display the data.

* Created a template HTML file called `index.html` that will take the mars data dictionary and display all of the data in the appropriate HTML elements. Use the following as a guide for what the final product should look like, but feel free to create your own design.

![final_app_part1.png](Images/final_app.png)




[screencapture-127-0-0-1-5000-2021-08-14-14_40_00 (1).pdf](https://github.com/RRbenitez77/web-scraping-challenge/files/7909968/screencapture-127-0-0-1-5000-2021-08-14-14_40_00.1.pdf)


