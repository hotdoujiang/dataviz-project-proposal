# Data Visualization Project

## Data

The datasets I proposed to visualize for my project include

* [2019 Economic Freedon Index](https://gist.github.com/hotdoujiang/addd4f2369f3457e5a09a8b89942941b) downloaded from [Heritage Organization](https://www.heritage.org/index/about)

>The Economic Freedom Index is poised to help readers track over two decades of the advancement in economic freedom, prosperity, and opportunity and promote these ideas in their homes, schools, and communities. The Index covers 12 freedoms – from property rights to financial freedom – in 186 countries. <br>


* [Ramen Rating](https://gist.github.com/hotdoujiang/41d6a5c41b9975ac55a720bd46fd6392)

The dataset comes from [Ramen Rater](https://www.theramenrater.com/)

>The Ramen Rater is a product review website for the hardcore ramen enthusiast (or "ramenphile"), with over 3000 reviews to date. This dataset is an export of "The Big List" (of reviews), converted to a CSV format. <br>
Each record in the dataset is a single ramen product review. Review numbers are contiguous: more recently reviewed ramen varieties have higher numbers. Brand, Variety (the product name), Country, and Style (Cup? Bowl? Tray?) are pretty self-explanatory. Stars indicate the ramen quality, as assessed by the reviewer, on a 5-point scale; this is the most important column in the dataset!


* [Global Terrorism Dataset](https://gist.github.com/hotdoujiang/e6064faca930a996230aa4dc3ccd8db0)

The dataset is downloaded from the [Global Terrorism Database](https://www.start.umd.edu/gtd/).

>The GTD™ is an open-source database, which provides information on domestic and international terrorist events around the world since 1970, and now includes more than 190,000 events. For each event, a wide range of information is available, including the date and location of the incident, the weapons used, nature of the target, the number of casualties, and – when identifiable – the group or individual responsible.

All the three dataset can be find in my Gist. Some preprocessing work has been conducted to make the data suitable for visualization.

## Prototypes

I’ve created a proof of concept visualization of the data. The viz shows the correlation between two important evaluation metrics 'Tax Burden' and 'Government Integrity'.

[![image](https://user-images.githubusercontent.com/42425096/67602911-a7b56d80-f745-11e9-9222-56a999340eb0.png)](https://beta.vizhub.com/hotdoujiang/4f0bcd5520b74d5a8d8d88bd88bd2f24)

We cannot seen a clear correlation between these two attributes. Tax burden is not significantly correlated with government integrity.
However, most of the countries in the world have high tax burden as well as low government integrity, with a intenser field appearing on the right lower corner of the picture.
Most European countries, the red circles on the picture, have a low tax burden and high government integrity, while most sub-saharah African countries, the green circles, have a high tax burden and low government integrity.
An interesting outlier is located at the left lower corner, which is North Korea. The country has no tax burden but relatively low government integrity.

[![image](https://user-images.githubusercontent.com/42425096/68317625-757f0680-0089-11ea-9c8b-670462d6b8a5.png)](https://beta.vizhub.com/hotdoujiang/b4d211ecb917438cae29e5277c6a565f?edit=files&file=README.md)

The viz shows the perpetrators who conducted crimes in the United States during 1975 to 2017 and their target type with corresponding weapon type.
** From the viz we can see that the Private Citizens & Property and Business are almost the common target for all the perpetrators.
** And most of the blocks are color green, which means Explosives/Bombs/Dynamite is the favourite weapon for the terrorists.

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

* How is the economic freedom distribution around the world? Is there any region pattern?
* Which are the top countries who have the most tax burden?
* Is there any relationship between trade freedom and the country location? i.e. whether it is a inland country or not?

## Sketches

* Global Terrorism Dataset
![Global Terrorist](https://user-images.githubusercontent.com/42425096/68318084-343b2680-008a-11ea-9292-ac5d408c8c88.jpg)

* Ramen Rating
![Ramen Rating](https://user-images.githubusercontent.com/42425096/68317903-e9211380-0089-11ea-93a2-c92f3518a14d.jpg)

* Economic Freedom Index
![image](https://user-images.githubusercontent.com/42425096/67602655-1a721900-f745-11e9-91da-35e3ddbbd39a.jpg)

The whole picture will be a interactive world map. Ideally, it should be a spinning earth with country maps in different brightness. The brighter country map is, the more free the country economic is.

Interactions
* Users can zoom in and out to check out more details of countries in the world.
* Each country map is clickable, which contains information about the 12-freedom-index radar chart.

## Current Visualization

* Global Terrorism Dataset

[![GTD](https://user-images.githubusercontent.com/42425096/68251447-24233880-fff1-11e9-8451-aadee278abed.png)](https://beta.vizhub.com/hotdoujiang/278556d01b4044bd9aa8d1e1858a5d38)

* Ramen Rating
[![RR](https://user-images.githubusercontent.com/42425096/68251447-24233880-fff1-11e9-8451-aadee278abed.png)](https://beta.vizhub.com/hotdoujiang/bb83820293d04fba9762d1c4071904f7)

* World Economic Freedom Index

Here's the world economic freedom index - China v.s. US.
[![WEFI](https://user-images.githubusercontent.com/42425096/68251702-b4617d80-fff1-11e9-9313-231d3f377d2d.png)](https://beta.vizhub.com/hotdoujiang/a70d524e772e4ff582fe6d0158c6df83)
