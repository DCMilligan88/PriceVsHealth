# City Health inspections vs Yelp Price Classification


## Objective:
To discover if there is a connection between the price categories of yelp ($, $$, $$$) and the cities health inspection rating for that respective business. We quantify this through linear regressions.

## Step 1 Gathering Data:
The resources we used were yelp and data from the city of portland. We used the yelp API and asked the city for a csv that contained information pertaining to Health Inspections across portland. 

## Step 2 Combining Data:
To complete our objective the data we have from the city health inspections doesn't mean much by itself, we needed a way to combine them into one data frame. We could have created two csvs and combined them on like business names but instead we created one DataFrame from the health inspections csv and used iterrows to programatically collect each business name and then run it through a search in the yelp API and if it got a response it would fill out rows in our DataFrame that pertained to our objective and if it didn't find anything it would drop that row. From the csv we started with out about 3300 points of data and ended up with about 1/3 of that. We believed that was enough to make an argument either for or against wether there is a connection between price point and health inspections. ![DataFrame](https://github.com/DCMilligan88/PriceVsHealth/blob/master/Pngs/Capture.PNG)

## Step 3 Making some Graphical Representation:
We then used matplotlib to make our graphical representations of the data. Box Plot Linear Regressions were the most informative graphs we could make. <br> 
![Boxplot](https://github.com/DCMilligan88/PriceVsHealth/blob/master/Pngs/Box%20plot.png) 
![LinearRegression](https://github.com/DCMilligan88/PriceVsHealth/blob/master/Pngs/moderate_LR.png)