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

To answer the question, I used an area plot which shows all types of energy sources and their contribution to the total amount of energy produced. We can easily compare sources on the amount of energy produced, as well as track changes in the amount of energy produced over the years.

An alternative was a barplot, which would give columns instead of lines. It would contain the same information as this chart. Here I see a subjective assessment of which one is the best, some people like bar charts, I prefer lines or area plots because they have more outlined dynamics. *(I used bar chart in the Task#3)*

It was also possible to approach this question differently and to make relative charts (it is possible both with area plot and bar chart). In this way, we will be able to see a much clearer difference between energy production over the years, but we will lose the amount of energy produced over the years. For me, information about the amount of energy produced was important, so I gave up on this idea.

### Task 2: Як залежить споживання електроенергії від дня року та години доби?
My visualization:


This was the most difficult task for me because we had to outline such dimensions as: time of day, day of the year and the amount of energy released. They all have a lot of data and to make them categorical variables would be inconvenient and ugly.
So I decided to make a heapmap. The color on it reflects the amount of energy consumed. By following it, we can track changes in energy consumption for the day of the year and for the hour of the day and see all the dependencies we need.

**The downside is that we don't see the energy consumption data very accurately because they are displayed in color, but because of this, I made all the graphs in this task interactive. You can hover over the data and get more information (works in Jupyter Notebook)**

As an alternative - 3-D graphics, but I find them too complex for this task.

### Task 3: Як змінюється генерація електроенергії з різних джерел впродовж доби?
My visualization:

This task is similar to the first task. Only unlike the first task, I used a bar chart here.
