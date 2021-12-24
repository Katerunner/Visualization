## Final Project

### General

All code is in the Jupyter Notebook

---
**!! IMPORTANT !!**

Jupyter file is to large for git repo as well as the html file. I dropped it on drive:

>https://drive.google.com/drive/folders/1LmgBGMUvr2ANV86wsfw0hr6U7tis4ocG?usp=sharing

If you want to run them, drop to the Visualization/Final Project folder (this one)

---


Using common libraries:
- numpy
- json
- pandas
- plotly (main for visualizations)

Unfortunately plotly cannot be compiled in the GitHub preview, so there is also HTML file to play with interactive plots

**Work:**

### Visualization 1
![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/p1.png)


In the first visualization, we show the distribution of the population by sex and age.
We also want to show how many people of what age and articles were in Ukraine at a certain point in time - that is, by year.

To do this, we used the population pyramid. This is an important type of visualization in the analysis of the population
of a country or region, as it can point us to many problems related to generation gaps, gender differences, and the results of major events (wars, pandemics, disasters).

In my version of the population pyramid:

- Display by year is implemented through animation. You can select the year on the slider below, or turn on the animation.
- There is a hover window, which displays the number of people in the appropriate category, age, gender of the current year, as well as the year of birth.
- The floor is marked with color, there is a legend and all the necessary elements.

**Amount of Information**

In this visualization we can clearly see:

- The results of the Holodomor - a much lower birth rate
- The results of World War II - lower birth rates and fewer men
- The collapse of the USSR and the 90s (begins after the Chernobyl tragedy) - a gradual decline in birth rates by the 2000s
- Rise in birth rate before the war in 2014, and decline after that.

In fact, this visualization shows how many hardships the Ukrainian people have gone through in their recent history.
In my experience, this chart appears in almost every course or discussion with politicians or historians about the problems and challenges for Ukraine.

**Alternatives**

It is difficult for me to come up with an alternative chart that can explain so much information in one chart so well.
However, for some, understanding this chart can be difficult, it takes a long time to look at it to easily navigate and find insights.
As an alternative, I would propose to divide into separate graphs of births and deaths by year by sex + bar graph of the distribution of the existing population by age by the same years.

**Possible Improvements**

Footnotes or divisions could also be added to reflect important events in certain years, such as those we highlighted above.
Also in such graphs add an slightly darker or brighter parts of the columns - as a reflection of mortality and birth rate in specific years

**Screens**
![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/p_1_2.png)

### Visualization 2

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_2.png)

This is a simple chart that provides information on the birth rate and mortality rate with natural population growth over the years.
For us, it is interesting because it shows how the situation with population growth has deteriorated since Ukraine's independence.
This graph also shows well the development trends of these coefficients and helps in visual forecasting.

**Alternatives**

A small amount of information is displayed here, so it's hard to talk about any alternatives - a bar chart will not reflect the change in time of three variables so well.
Is a area chart, can better reflect the volume.

### Visualization 3

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_3.png)

This is the hardest visualization I've ever done. The task was to reflect the volume and sources (purposes) of migration of the population of Ukraine by countries in 2020.

I decided to make the following visualization structure:

- We have two visualization modes:
- - right: emigration
- - left: immigration
- Switch between modes with the slider by clicking right or left.
- In the middle - a map that shows the number of people who immigrate (emigrate) using the size and color of the bubbles over the respective countries.
- By turning on the move mode in plotly we can bring the map closer, the size of the bubbles will change accordingly, so we can get a good look at the details.
- Hover window will be displayed when you hover over the bubble, showing us information about the country and the number of people who immigrated (emigrated)
- On the right of the map we have a bar chart, which gives us sorted in descending order top-20 countries where Ukrainians emigrate, distributed across continents that are also highlighted in color.
- On the left we have the same bar chart, but for immigration data.
- When hovering on the bar chart, we also have a hover window with information about the number of people and country.
- When selecting a mode, a chart that does not belong to it has more transparency to better show which mode is currently active. It does not disappear completely, so we can compare in any case.
- We also have a legend with continents, where we can turn off / on the continents to display in bar charts.
- Ukraine with regions is also visually highlighted in color

I think this chart works very well with the amount of information that needed to be displayed.

**Amount of Information**

In this chart, we can clearly see which countries Ukrainians usually emigrate to and where immigrants come from.
We see that a lot of people come to us from Russia, Belarus and Moldova in Europe, as well as from Turkey and India in Asia. We also see that Ukrainians usually go to Russia and Germany in Europe and to Turkey and China in Asia.
Many people also come to America from us.

This graph refuted my theory that Ukrainians are most likely to emigrate to Canada now, and also showed
that a very large number of people are immigrating to Ukraine from Russia and Belarus, most likely due to repression or deteriorating situation in those countries.

**Alternatives**

Alternatively, it may be just a bar chart for the top 20 countries, but then we will not be able to
see other data. You can't make a bar chart for all countries because there will be too many columns.
An alternative here may be to simply divide this graph on the frame of the graph without an interactive element, but then the
elements of comparison and integrity of the representation will be lost. You can also replace bar charts with pie charts, but in favor of the design I went with the bar ones.
Also the are many ways of sorting the countries in the bar charts. It can be by number of people only without the continent contribution, but I like such division, so it is as it is.

**Improvements**

- Now we can turn off the continents on the bar chart, but we can't on the map, it would be cool to add such interaction.
- It's very difficult to do plotly, but it would be cool to add some text to the map, either with countries or with meaning

**Screens**

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_3_2.png)

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_3_3.png)

### Visualization 4

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_4.png)

The task is to reflect changes in population density by region, persons per 1 sq. Km by year - from independence to 2014.
To do this, I use the map of Ukraine divided into areas marked by color - as a percentage change in density from the previous year.
To display by year, I use animation and the same range of change.

**Amount of Information**

We can see that in the period from 1995 to 2012 we had a period of declining density in most areas.
We can also see that in the western regions there was less reduction in density than in other regions.

**Alternatives**

The main alternative to this graph is a linear graph by year.
It better reflects the change and the numerical value of the change.
But it has one big downside - it has a lot of lines that often intersect on every chart and it looks very unpleasant.
Personally, I prefer the current version with the map.

**Improvements**

As an option, you could add a side line chart, there are people who like it more, but unfortunately due to frequent changes
in values and values close to 0, 25 lines do not look very good.
The main improvement option is to add text over areas with density values. Unfortunately in plotly this is hard to do.

**Screens**

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_4_2.png)

### Visualization 5

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_5.png)

Here we have the final task - to explain the distribution of ethnic groups among the population of Ukraine, also in terms of urban and rural population.

To do this, you can choose different types of visualization, I chose - treemap, or hierarchical square pie chart.
It is interactive, so you can go inside a group (such as an urban population) and compare the distribution there.
The population of the corresponding group is reflected by the size of the rectangle. Since we do not see accurate
data as well as small rectangle labels, the main tool for working with this graph is the hover window, which contains data on the ethnic group and its number.

**Amount of Information**

The main insight I got from this chart is that there are more Ukrainians in the city than in the countryside, which I did not expect.
It is also interesting that among the urban population we also have many Belarusians, Moldovans and Crimean Tatars.

**Alternatives**

As the main alternative to such a chart - two pie charts. But due to the fact that we have groups that have a very small number,
it did not look as good as the current schedule. We could also use a bar graph, or a relative bar graph.

**Improvements**

- Better color scheme - to colorize rural and urban rectangles as well
- Displaying labels and values and text positioning - but very hard in plotly

**Screens**

![alt text](https://github.com/Katerunner/Visualization/blob/main/Final%20Project/plt_5_2.png)

