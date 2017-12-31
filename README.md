# dand-p7-data-visualization
Data visualization project from Udacity's Data Analyst Nanodegree

<h4>Summary</h4>

This visualization depicts some of the findings from the Titanic dataset, which contains information about 891 of the passengers and crew members aboard. The graph breaks down the survivors by gender and by ticket class. We can see that women had a higher survival rate, as did those with better ticket classes (lower ticket class numbers).

<h4>Design</h4>

Given that this dataset was part of an earlier project, I had a sense of the findings and spent some time thinking about how to visualize it. I wanted to highlight the difference in survival rate between men and women, as well as the impact of ticket class on survival. My initial thought process can be seen in the sketch below.

<h5>Intitial sketch of the data visualization:</h5>

![Sketch](sketch.png)


Initially I was going to facet the graphs between men and women, but realised that the results might be hard to compare especially since one of the points I wanted to make was the difference in survival between the genders. As a result, I decided to use a combination of grouping and stacking with the bar charts to display the data. The bar charts made for easy comparison (positional data encoding), the stacks represented the survival, each group represented a class, and the bars inside each group corresponded to women and men respectively. A legend would be present to distinguish between the stacks.

As the bars were stacked, I would be using different colours to distinguish between the stacks. I initially played around with the colours of the stacks, but then settled on the default colours as the red corresponds to those who perished, the pastel colours were pleasing to the eye, and my initial thoughts about red and green didn't take colour blindness into consideration.

I started by first putting together the grouped horizontal bar chart and then figuring out how to add the interactivity through the use of the "Count" and "Percentage" buttons. The bar charts were stacked based on survival and grouped based on gender so that the male vs. female survival rates could be compared easily.

<h5>First version of the data visualization:</h5>

![v1](p7_v1.png)


After getting feedback on the first version of the graph I modified several aspects, namely:
- Switched from a horizontal to a vertical bar chart
- Added labels to the male and female bars
- Added a description to the visualization
- Made the percentage view the initial view

<h5>Second version of the data visualization:</h5>

![v2](p7_v2.png)


<h4>Feedback</h4>

Feedback 1 from my partner:
- Confusion over pclass vs ticket class
- Confusion over which bars related to males vs females
- Surprised at how many females survived as compared to males
- The comparisons would be easier to make if the bar was vertical rather than horizontal

Feedback 2 from my brother:
- Thought the colours related to gender
- Didn't know what the better class was
- After interacting with the diagram for a bit the distinction between the bars became clear as did the better survival of women and upper class people, but it would be better to have the bars labeled with male and female

Feedback 3 from my friend:
- Kind of difficult at first to figure out what the different bars represented (ticket class or gender...).
- It's neat how you can choose between the count and percentage, though I prefer the percentage data. It would be nice if that was the first thing that was displayed, instead of the count.
- It's not obvious that you can hover over the bars to get more data, but once I discovered that it was fun to explore the values. That also helped a lot with figuring out which bars were for men vs. women.
- It's interesting but not surprising to see that rich people and women had a higher chance of survival.

<h4>Resources</h4>

- http://dimplejs.org/examples_viewer.html?id=bars_horizontal_grouped_stacked
- https://stackoverflow.com/questions/32232518/how-to-change-the-order-of-grouped-bar-chart-in-dimple
- https://classroom.udacity.com/nanodegrees/nd002/parts/00213454010/modules/318423863275460/lessons/3066258748/concepts/31058087130923
- https://www.w3schools.com/css/css_positioning.asp
- https://stackoverflow.com/questions/22452112/nvd3-clear-svg-before-loading-new-chart
- https://stackoverflow.com/questions/21990857/d3-js-how-to-get-the-computed-width-and-height-for-an-arbitrary-element

