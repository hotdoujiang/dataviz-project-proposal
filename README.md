# Data Visualization Project

## Data

The data I propose to visualize for my project is downloaded from [Heritage Organization](https://www.heritage.org/index/about)

>The Economic Freedom Index is poised to help readers track over two decades of the advancement in economic freedom, prosperity, and opportunity and promote these ideas in their homes, schools, and communities. The Index covers 12 freedoms – from property rights to financial freedom – in 186 countries. <br>

The attributes are
* Country Name
* Region
* World Rank
* Region Rank
* 2019 Score
* Property Rights
* Judical Effectiveness
* Government Integrity
* Tax Burden
* Gov't Spending
* Fiscal Health
* Business Freedom
* Labor Freedom
* Monetary Freedom
* Trade Freedom
* Investment Freedom
* Financial Freedom

## Prototypes

I’ve created a proof of concept visualization of this data. The viz shows the correlation between two important evaluation metrics 'Tax Burden' and 'Government Integrity'.


[![image](https://user-images.githubusercontent.com/42425096/67602911-a7b56d80-f745-11e9-9222-56a999340eb0.png)](https://beta.vizhub.com/hotdoujiang/4f0bcd5520b74d5a8d8d88bd88bd2f24)

We cannot seen a clear correlation between these two attributes. Tax burden is not significantly correlated with government integrity.
However, most of the countries in the world have high tax burden as well as low government integrity, with a intenser field appearing on the right lower corner of the picture.
Most European countries, the red circles on the picture, have a low tax burden and high government integrity, while most sub-saharah African countries, the green circles, have a high tax burden and low government integrity.
An interesting outlier is located at the left lower corner, which is North Korea. The country has no tax burden but relatively low government integrity.

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

* How is the economic freedom distribution around the world? Is there any region pattern?
* Which are the top countries who have the most tax burden?
* Is there any relationship between trade freedom and the country location? i.e. whether it is a inland country or not?

## Sketches

![image](https://user-images.githubusercontent.com/42425096/67602655-1a721900-f745-11e9-91da-35e3ddbbd39a.jpg)

The whole picture will be a interactive world map. Ideally, it should be a spinning earth with country maps in different brightness. The brighter country map is, the more free the country economic is.

Interactions
* Users can zoom in and out to check out more details of countries in the world.
* Each country map is clickable, which contains information about the 12-freedom-index radar chart.

## Open Questions

I’m not sure how to make the earth spinning in certain ratio and how to make the earth 'clickable' and linked to the radar chart.
