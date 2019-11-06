# Data Visualization Project

## Data

The datasets I proposed to visualize for my project include

### [2019 Economic Freedon Index](https://gist.github.com/hotdoujiang/addd4f2369f3457e5a09a8b89942941b) 

The dataset is downloaded from [Heritage Organization](https://www.heritage.org/index/about)

>The Economic Freedom Index is poised to help readers track over two decades of the advancement in economic freedom, prosperity, and opportunity and promote these ideas in their homes, schools, and communities. The Index covers 12 freedoms – from property rights to financial freedom – in 186 countries. <br>

### [Ramen Rating](https://gist.github.com/hotdoujiang/41d6a5c41b9975ac55a720bd46fd6392)

The dataset comes from [Ramen Rater](https://www.theramenrater.com/)

>The Ramen Rater is a product review website for the hardcore ramen enthusiast (or "ramenphile"), with over 3000 reviews to date. This dataset is an export of "The Big List" (of reviews), converted to a CSV format. <br>
Each record in the dataset is a single ramen product review. Review numbers are contiguous: more recently reviewed ramen varieties have higher numbers. Brand, Variety (the product name), Country, and Style (Cup? Bowl? Tray?) are pretty self-explanatory. Stars indicate the ramen quality, as assessed by the reviewer, on a 5-point scale; this is the most important column in the dataset!


### [Global Terrorism Dataset](https://gist.github.com/hotdoujiang/e6064faca930a996230aa4dc3ccd8db0)

The dataset is downloaded from the [Global Terrorism Database](https://www.start.umd.edu/gtd/).

>The GTD™ is an open-source database, which provides information on domestic and international terrorist events around the world since 1970, and now includes more than 190,000 events. For each event, a wide range of information is available, including the date and location of the incident, the weapons used, nature of the target, the number of casualties, and – when identifiable – the group or individual responsible.

All the three dataset can be find in my Gist. Some preprocessing work has been conducted to make the data suitable for visualization.

## Prototypes

I’ve created a proof of concept visualization of the data. 

1. The visualization below shows the correlation between two important evaluation metrics 'Tax Burden' and 'Government Integrity'.

[![image](https://user-images.githubusercontent.com/42425096/67602911-a7b56d80-f745-11e9-9222-56a999340eb0.png)](https://beta.vizhub.com/hotdoujiang/4f0bcd5520b74d5a8d8d88bd88bd2f24)

There isn't any clear correlation between these two attributes. Tax burden is not significantly correlated with government integrity.
However, most of the countries in the world have high tax burden as well as low government integrity, with a intenser field appearing on the right lower corner of the picture.
Most European countries, the red circles on the picture, have a low tax burden and high government integrity, while most sub-saharah African countries, the green circles, have a high tax burden and low government integrity.
An interesting outlier is located at the left lower corner, which is North Korea. The country has no tax burden but relatively low government integrity.

2. The second visualization shows the perpetrators who conducted crimes in the United States during 1975 to 2017 and their target type with corresponding weapon type.
[![image](https://user-images.githubusercontent.com/42425096/68317625-757f0680-0089-11ea-9c8b-670462d6b8a5.png)](https://beta.vizhub.com/hotdoujiang/b4d211ecb917438cae29e5277c6a565f?edit=files&file=README.md)

From the viz we can see that the Private Citizens & Property and Business are almost the common target for all the perpetrators.
And most of the blocks are color green, which means Explosives/Bombs/Dynamite is the favourite weapon for the terrorists.

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

* How is the economic freedom distribution around the world? Is there any region pattern?
* Which are the top countries who have the most tax burden?
* Is there any relationship between trade freedom and the country location? i.e. whether it is a inland country or not?

## Sketches

### Global Terrorism Dataset
![Global Terrorist](https://user-images.githubusercontent.com/42425096/68318084-343b2680-008a-11ea-9292-ac5d408c8c88.jpg)

### Ramen Rating
![Ramen Rating](https://user-images.githubusercontent.com/42425096/68317903-e9211380-0089-11ea-93a2-c92f3518a14d.jpg)

### Economic Freedom Index
![image](https://user-images.githubusercontent.com/42425096/67602655-1a721900-f745-11e9-91da-35e3ddbbd39a.jpg)

The whole picture will be a interactive world map. Ideally, it should be a spinning earth with country maps in different brightness. The brighter country map is, the more free the country economic is.

Interactions
* Users can zoom in and out to check out more details of countries in the world.
* Each country map is clickable, which contains information about the 12-freedom-index radar chart.

## Current Visualization

### Global Terrorism Dataset

[![GTD](https://user-images.githubusercontent.com/42425096/68251403-05bd3d00-fff1-11e9-9800-200ec0d3f9be.png)](https://beta.vizhub.com/hotdoujiang/278556d01b4044bd9aa8d1e1858a5d38)

The points on the map represents worldwide terrorism events which took place in 2018.

The size of the points represents the number of people who were wounded or killed in the terrorism event. The larger a point is, the more people are injured or killed in the event.

The color of the points are set to be red to make it look like blood.

*Future work* : 
1. To make multiple views by adding a time series bar chart at the bottom of the map;
2. Add brushes to interactively show the temporal and spatial changes of the number of terrorism events.
3. Tooltip can also be added to see which orginazation conduct the terrorism event or the exact number of victims.

### Ramen Rating
[![RR](https://user-images.githubusercontent.com/42425096/68251447-24233880-fff1-11e9-8451-aadee278abed.png)](https://beta.vizhub.com/hotdoujiang/bb83820293d04fba9762d1c4071904f7)

The visualization is all about Ramen Ratings! The picture includes information about the ramen score, style and which country it comes from.
** Most circles are light red and purple, which means most of the ramen reviewed are pack and bowl.
** Japan, Taiwan, the US and some other countries have ramen which shares a large range of rating scores, from lower than 0.5 to 5.

*Future Work*
Distributed map fails to be realized because of lacking geographic data, a.k.a longitude and latitude. The missing data can be added to the original dataset to make the map visualization possible.

### World Economic Freedom Index

Here's the world economic freedom index radar chart- China v.s. US.
[![WEFI](https://user-images.githubusercontent.com/42425096/68251702-b4617d80-fff1-11e9-9313-231d3f377d2d.png)](https://beta.vizhub.com/hotdoujiang/a70d524e772e4ff582fe6d0158c6df83)

The rader chart is a gorgeous [data visualization designed by Nadieh Bremer](https://beta.vizhub.com/Kuerzibe/610ea1fb51f2476f9ae9f2bf225bf564). So far I am doing well on integrating it with my [World Economic Freedom Index dataset](https://gist.github.com/hotdoujiang/addd4f2369f3457e5a09a8b89942941b), although some further changes are still necessary for better interpreting.
You can see from the chart that the data indicates that the economic of the United States is generally more free than the economic of China, except for the two aspects, Fiscal Health and Government spending.

And another scatter plot with menus. Dropdown menus added to the visualization to show the correlation between the selected 2 economic freedom indexes.
[![menus](https://user-images.githubusercontent.com/42425096/68251276-c1ca3800-fff0-11e9-88d2-2dd60959745a.png)](https://beta.vizhub.com/hotdoujiang/db9678c5d9224f3ebc9e91c8ecd30c28)

*Future Work*

1. The radar chart is flexible with the number of axis. It is not fixed, so you can have as many axises as you like. Here I have 12 indexes describing the economic freedom. Hence, my radar chart is a 12-axis chart.
2. The function of the scale need to be changed according to need. The 'default' function is about the percentage.
3. The max value of the axis is not fixed too. It is depending on the data you entered in. Changes are needed if you want the fixed maximum value.
4. It is so frustrating that the data entry is by typed not imported from csv or json. I think that for the future improvements I can use d3 to import formated data instead of typing.
5. There's no tooltip by placing the mouse on the inner information, which means that you cannot tell whether the red is China or not unless checking the src. I think I can add a tooltip to the radar chart to make it better.
