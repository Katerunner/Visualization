## Homework #2

### General

All code is in the Jupyter Notebook - *main.ipynb*.

Using common libraries:
- pandas
- numpy
- plotly (main for visualizations)


**Data processing:**

All data processing was done in the Jupyter Notebook.

### Task 1: Як змінювалась структура генерації електроенергії за роками?
My visualization:

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p1.png)

To answer the question, I used an area plot which shows all types of energy sources and their contribution to the total amount of energy produced. We can easily compare sources on the amount of energy produced, as well as track changes in the amount of energy produced over the years.

An alternative was a barplot, which would give columns instead of lines. It would contain the same information as this chart. Here I see a subjective assessment of which one is the best, some people like bar charts, I prefer lines or area plots because they have more outlined dynamics. *(I used bar chart in the Task#3)*

It was also possible to approach this question differently and to make relative charts (it is possible both with area plot and bar chart). In this way, we will be able to see a much clearer difference between energy production over the years, but we will lose the amount of energy produced over the years. For me, information about the amount of energy produced was important, so I gave up on this idea.

### Task 2: Як залежить споживання електроенергії від дня року та години доби?
My visualization:

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p2.png)

This was one the most difficult task for me in terms of finding the best visualization method, because we had to outline such dimensions as: time of day, day of the year and the amount of energy released. They all have a lot of data and to make them categorical variables would be inconvenient and ugly.
So I decided to make a heapmap. The color on it reflects the amount of energy consumed. By following it, we can track changes in energy consumption for the day of the year and for the hour of the day and see all the dependencies we need.

**The downside is that we don't see the energy consumption data very accurately because they are displayed in color, but because of this, I made all the graphs in this task interactive. You can hover over the data and get more information (works in Jupyter Notebook)**

As an alternative - 3-D graphics, but I find them too complex for this task.

### Task 3: Як змінюється генерація електроенергії з різних джерел впродовж доби?
My visualization:

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p3.png)

This task is similar to the first task. Only unlike the first task, I used a bar chart here.

### Task 4: Як змінюється споживання електроенергії впродовж доби у розрізі місяців року та пір року?

For this task, I have several options for visualizations. The first - the simplest - is a schedule of energy consumption by the hour for each month. Since there are 12 months (rather than 366 categories as the second task), we can display them all on the same chart, in different colors with the legend. We use a different symbol to separate the seasons. This graph well reflects everything we need, the only problem - 12 lines may not be very convenient to compare. Here we are helped by the fact that the schedule is interactive and we can exclude lines that we do not need in the legend.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p4.png)

The next option is to display the consumption in color. We will have a graph where the x-axis is the hour, the y-axis is the month (grouped by seasons) and the values will be circles with different colors and sizes, reflecting energy consumption. Here we get the same problem as with the second task - we do not see the exact number of consumption by the color of the circle, but this graph looks very cool. We also solve the problem of inaccurate understanding of meaning through color by the fact that the graph is interactive and you can hover the cursor and look.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p5.png)

There is also a variant of the graph - stacked bar plot - where we for each month (grouped by season) will build a column on energy consumption by hours and display the value of consumption in height and color. So we will also see the information that we could in the previous graphs + the total amount of energy consumed by months.

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p6.png)

### Task 5: Як змінюється споживання електроенергії впродовж тижня?
My visualization:

![alt text](https://github.com/Katerunner/Visualization/blob/main/HW2/p7.png)

Here we used the usual line graph, which showed the change in energy consumption during the week. It would be possible to use also barchart, I like linear more - on it dynamics of changes is better visible.
