## Homework #3

### General

All code is in the Jupyter Notebook - *main.ipynb*.

Using common libraries:
- pandas
- geopandas
- numpy
- plotly (main for visualizations)

Unfortunately plotly cannot be compiled in the GitHub preview, so there is also HTML file to play with interactive plots

**Data processing:**

All data processing was done in the Jupyter Notebook.

### Task 1: В яких країнах світу населення у 2100 році буде більшим, ніж було у 2000 році, а в яких меншим?
My visualization:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW3/1.png)

I used plotly for visualization which has hover area with additional info + it is interactive (you can scale them and move, select areas and so on). For the task I decided to plot the countries, which will have less population in 2100 to color with red (as a negative value) and countries with more population as green. In the hover area you can view the country name, less or more population in 2100 and the population itself (index is there by default, could not find the way how to hide it). This type of visualization is answering the question pretty well.

One thing is that you can see the borders of countries but no countries names. To fix this I decided to make the color with opacity (~ 0.4), and to put the openstreet map underneath. This map have ocean names, continent names and counties names depending on scale. *This will be also used in the next task.*

### Task 2: На скільки відсотків збільшиться або зменшиться населення кожної країни у 2100 році у порівнянні з 2000 роком?
My visualization:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW3/2.png)

Here the visualization is pretty similar to the previous task except the we have a continious scale colormap that represents the percentage change of population. I faced a problem with the default colormaps. We have min value of ~ -0.67 and the max ~ 13.67. Default colormaps (gradients) provide the color intersection somewhere in the middle. In our case zero change should be with the intersection of colors of the gradients, but zero is not in the middle of our scale. So I decided to make my own colormap with small red area for negative values and long yellow-to-green area of colormap for higher values.

Information of the country name and population in 2100 you can get in the hover area. The one disadvantage can be the missing absolute change or population in 2000. But you it depends on how much info you want to provide. I believe that the visualizaztion answers the question perfectly.

### Task 3: Яким буде населення країн світу у 2100 році?
My visualization:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW3/4.png)

Here I decided to go with the scatter diagram over the map outline. I encoded the population as the size of the circle as well as the color of the circle. I found out that my custom colormap fits this purpose very well and the difference in population can be easily visible by color and size. Visualization is interactive so you can see the name of the country and its population in 2100 in the hover area, as well as scale and move the map. Also, considering that the circles can be small of far away plotly does pretty good job at the comfortable distance where the hover area apears. As a downside I can say that I could not set the openstreet map as the background and we are left with outline only in this example.
