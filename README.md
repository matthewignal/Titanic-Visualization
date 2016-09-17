## Titanic Survivor Visualization
by Matthew Ignal

### Summary

This visualization of the survivor demographics of the 1912 Titanic disaster displays the survival statistics according to three categories: the sex, cabin class, and age of the passengers. The main finding is that women, first class passengers, and children had high rates of survival, while men, third class passengers, and seniors had high rates of death.

### Design

#### Exploratory Data Analysis

A quick perusal of the Titanic dataset revealed an orientation toward the demographics of the passengers: specifically sex, class, and age. I decided to explore how these variables impacted the "survived" category. I had prior knowledge that women and children were prioritized when it came to receiving lifeboats, but I wanted to explore the extent to which these factors played into each demographic's survival rate. I decided to organize the passenger's ages into sensible groups (children, teenagers, seniors, etc.) to help reveal these trends. Cabin class was another interesting variable that I hadn't considered before.

##### Chart Type: Stacked Bar Graph

I decided that, given the overall simplicity of main features to convey, it was important for the visualization to quickly and clearly communicate the survivor demographics. Women should be compared to men while each class and age grouping should be compared to one another. As the count each demographic of passengers is an interesting (secondary) feature, I determined a bar graph would better highlight the Titanic demographics than a pie chart. A stacked bar chart would accomplish this goal most simply since we have two categories: "Survived" and "Died", which could make up a single column.

Following feedback, I replaced "count" with "passengers" on the y-axis changed "passenger class" to "cabin class".

##### Color Choices
I orignially started with green and red to indicate if passengers survived or not since I found those colors intuitive. After receiving feedback that the colors were "too Christmas-y", I changed the survivor color from green to a light blue and toned down the red to give a more natural feel. The original buttons to shift between categories were characterized as "too plain", so I went with a darker blue and rounded the corners.

##### Interactivity
Viewers of the graph generally did not play around with the original interactive buttons, which were originally located on the right side of the graph. I decided to change the color, shape, and location of the buttons. They are now placed at the top of the chart, near its title, so the connection between the category currently being visualized and the options the viewer has is more intuitive. I also added a transition effect because it's more fun.

##### Categories
I first decided to go with four age groups. I wanted to distinguish the survival rates of children and teenagers as well as adults and seniors because I thought my findings here were among the most interesting. However, I agreed with the feedback that the "adult" column dwarfed the others to the extent that it was distracting from the main findings, so I further divided the adults section into two. A guiding principle of this organization was trying to keep it as intuitive as possible so the actual parameters of the age groups did not need to be made explicit. The visualization now more clearly shows that children were most likely to survive and seniors were least likely. It was surprising to find that teenagers were no more likely to survive than adults.

### Feedback

#### First Iteration

The first iteration of the chart can be found at:

Jonathan C. (friend): I clearly see that there were more men on the titanic but a higher percentage of women survived and higher class passengers were more likely to survive. The colors are "too Christmas-y". I didn't notice the buttons for a while. The graph is very clear but the coloring could be improved.

##### Second Iteration (Added age groups, changed chart colors)

Katlin G. (colleague): The bar charts are clear and the main story is easy to follow. Women, the upper class, and children were most likely to survive the disaster. However, "count" is a little confusing at first and the interactivity is a little unclear as well and needs overhaul.

##### Third Iteration (Colored and moved buttons, changed "passenger class" labels.)

Wendy Q. (friend): I think the graph is trying to show that women, children, and people in first class were less likely to die in the Titanic disaster. The size of the "Adult" column is distracting since the more important findings are with children and seniors. I can't think of any other way the graph can be improved. Nice work!

##### Fourth Iteration (Split "adult" into two, added transition effect)

Howard E. (colleague): I think the main finding is that in the Titanic Disaster, women, children, and first class passengers were most likely to survive and men, seniors, and the poor were most likely to die. I like the transition between categories. Most charts usually display the main finding, so I'd include that in the title, but that's about it.

#### Final Iteration 

In the final iteration, I changed the subtitle to reflect this feedback.

It can be found at:

### Resources

- [dimple.js Examples](http://dimplejs.org/)
- [dimple.js Documentation](https://github.com/PMSI-AlignAlytics/dimple/wiki)
- [Udacity Forums](https://discussions.udacity.com/t/baseball-data-need-to-combine-3-separate-charts-html-files-into-one-and-create-radio-button/169661/) - Myles Callan
- [Pandas Cut](http://pandas.pydata.org/pandas-docs/stable/generated/pandas.cut.html)