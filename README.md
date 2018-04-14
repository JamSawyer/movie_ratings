# Solution for DataQuest Guided Project - Analyzing Movie Reviews
In this project we analyzed data on movie review scores, based on data FiveThirtyEight published in 2015. The movie review services that data was pulled from include: RottenTomatoes, Metacritic, IMDB, and Fandango.
The data was put together by FiveThirtyEight to help detect bias in the movie review sites.

# Instructions
1. Read fandango_score_comparison.csv into a Dataframe named movies.
2. Enable plotting in Jupyter notebook with import matplotlib.pyplot as plt and run the following magic %matplotlib inline.
3. Create a histogram of the Metacritic_norm_round column. Create a histogram of the Fandango_Stars column. Look critically at both histograms, and write up any differences you see in a markdown cell.
4. Calculate the mean of both Fandango_Stars and Metacritic_norm_round. Calculate the median of both Fandango_Stars and Metacritic_norm_round.
5. Calculate the standard deviation of both Fandango_Stars and Metacritic_norm_round. You can use the numpy.std method to find this.
6. Look at the review methodologies for Metacritic and Fandango. You can find the methodologies on their websites, or by using Google. Do you see any major differences? Write them up in a markdown cell. Write up the differences in numbers in a markdown cell, including the following:
7. Why would the median for Metacritic_norm_round be lower than the mean, but the median for Fandango_Stars is higher than the mean? Recall that the mean is usually larger than the median when there are a few large values in the data, and lower when there are a few small values. Why would the standard deviation for Fandango_Stars be much lower than the standard deviation for Metacritic_norm_round? Why would the mean for Fandango_Stars be much higher than the mean for Metacritic_norm_round.
8. Make a scatterplot that compares the Fandango_Stars column to the Metacritic_norm_round column.
9. Several movies appear to have low ratings in Metacritic and high ratings in Fandango, or vice versa. We can explore this further by finding the differences between the columns.
10. Calculate the r-value measuring the correlation between Fandango_Stars and Metacritic_norm_round using the scipy.stats.pearsonr function.
11. Use the scipy.stats.linregress function create a linear regression with Metacritic_norm_round as the x-values and Fandango_Stars as the y-values.
12. Predict what a movie that got a 3.0 in Metacritic would get on Fandango using the formula pred_3 = 3 * slope + intercept.
13. Predict what a movie that got a 1.0 in Metacritic would get on Fandango using the line from the last screen. Predict what a movie that got a 5.0 in Metacritic would get on Fandango using the line from the last screen.
14. Make a scatter plot using the scatter function in matplotlib.pyplot. On top of the scatter plot, use the plot function in matplotlib.pyplot to plot a line using the predicted values for 1.0 and 5.0. Pass in both x and y to plot to create a line.

