## Homework #5

### General

All code is in the Jupyter Notebook - *main.ipynb*.

Using common libraries:
- pandas
- json
- numpy
- plotly (main for visualizations)

Unfortunately plotly cannot be compiled in the GitHub preview, so there is also HTML file to play with interactive plots

**Data processing:**

All data processing was done in the Jupyter Notebook.

### Task 1: Створіть інтерактивну візуалізацію даних
The visualization from the previous task looks like this::

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW4/Result%20Visual.png)

We need to do the following:

- When pointing to a region on the map, it should be highlighted on the graph using the thickness of the line and its color.
- When hovering over a line on a chart, the corresponding region should be highlighted on the map with transparency.

I implemented these functionalities in my visualization, but also made sure that when you hover over a region on the map, the region also stands out with greater opacity in addition to greater line width and stronger color. Similarly, when drawn on a line on a graph, it also becomes wider and stands out with a stronger color.

This was not required in the task, but in my opinion it looks better when we hover the cursor, because we see more clearly what data we are hovering. This is especially useful on a line chart, where there are many lines that are close to each other.

So when you hover the cursor over the map, you get the following:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW5/on_map.png)

And when you hover the cursor over the line, you will see:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW5/on_line.png)

The downside of my implementation may be the speed of change - it takes about a second to select the desired line and region.

It is also worth noting that this is not some standard functionality in plotly, and I had to spend a long time understanding the documentation on how to make such an interactive functionality. The situation was complicated by the fact that this is a subplot that contains a map, and a similar scenario is not found on the forums.

But thanks to this task, I am now very familiar with the library plotly, and although it was not the main in course (as an altair), but the experience of working with it will help me a lot in my future work :)
