## Homework #6

### General

All code is in the Jupyter Notebook - *main.ipynb*.

Using common libraries:
- numpy
- json
- pandas
- plotly (main for visualizations)

Unfortunately plotly cannot be compiled in the GitHub preview, so there is also HTML file to play with interactive plots

**Data processing:**

All data processing was done in the Jupyter Notebook.

### Task 1: Ідентифікувати та описати проблеми у цій візуалізації даних
Original chart:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/original.png)

So, the purpose of this visualization is to show the change in the structure of activities in the regions of Ukraine in 2017 compared to 2010. There are several issues with this visualization:
- There are a lot of columns, not separated in any way
- It is difficult to concentrate and find the right data quickly
- Due to the fact that we have columns with relative data, we have a problem with comparing the parts of the columns that are responsible for the type of activity. The middle parts of the columns are difficult to compare because they can be at different heights.

In general, due to the last point, this graph does not reflect well the change in structure. We can notice a change in size (and it is difficult, because of the different heights), but we can not follow the significance of this change.

### Task 2: Зробити альтернативний варіант презентації цих даних
I have several options for visualizing this task, depending on the things we want to emphasize.

Version 1:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot1.png)

If we want to focus on activities, we can use several bar charts for each activity. In these diagrams, we will show the difference between 2010 and 2017 by the intersection of the columns with the value of the volume of these years, and the increase or decrease will be denoted by color. In addition, we will use interactive plotly functions, where we can take a closer look at the volume or difference through the hover area.

This chart copes well with this task. There is a downside to it - it has not very visible regions, because there are many of them. But if we need to emphasize the type of activity and display all the regions, we can use the maps.

Version 2:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot2.png)

Here on the maps, we will also divide them into activities and mark the change from 2010 to 2017 with the color of the region. Color gives us a general understanding of the change in volume, but in order to see the exact data of the change, we use the interactive functions plotly - hover window.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot2_1.png)

We have no information about Crimea, but we will bring it out so that the borders of Ukraine can be clearly seen. We will also note that there is no data for this region.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot2_2.png)

Version 3:
Dashboard:
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot3.png)

As an option, we can make such a relative dashboard, where we can use the hierarchy by region -> year -> type of activities, and with the ability to browse within these categories and compare data.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot3_1.png)
We can view the exact data through the hover window.
![alt text](https://github.com/Katerunner/Visualization/blob/main/HW6/plot3_2.png)
