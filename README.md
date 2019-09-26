# M1_exam2019

We have found a dataset containing data about students alcohol consumption, their grades and several social conditions.

In the repository, we have uploaded the dataset, two PDF files (Stakeholder report and the notebook) and the notebook as HTML. 

Link to notebook in colab: https://colab.research.google.com/drive/15ETOHyj6L8Lv8lej6tVbqit09RjP2cCE 

NOTICE: When you run our notebook, some of the results for the supervised machinelearning is going to be slightly different (even though we used seed), but it shouldn't affect the conclusions.

# Problem statement:
Are there any patterns of different groups of the students based on the features. Can we compute a model that predicts if a student is heavy drinker and can a model predict the students overall grade?

# Exploratory data analysis:

First we made a exploratory data analysis, where we examined the average overall grade based on gender and school, and how the alcohol affacted the grades.

We could see that the average overall grade was 11,28 and that females average grade was a bit higher then males. Also the GP school had markedly higher grades than MS and also most of the students went on GP.

We looked at some visualisations, where we could see that the binge and heavy drinkers had almost the same distribution as those who wasn't binge or heavy drinkers, although the drinkers was not really represented in the highest grades.

We also looked at how the grades where distributed by the age, where the older students had lower grades than the younger students, which may because this students have had trouble by passing their classes.

# Unsupervised ML:

As we computed unsupervised machine learning on the data, we could see by the PCA, that the numeric variables could be reduced to three dimensions. These dimensions explained the grades, the alcohol consumption and the absence & age.

Then we found four clusters using Kmeans, where these clusters contained the bad students, the average students, the good students and the students with high alcohol consumption.

# Supervised ML:

After the unsupervised ML, we would try to predict if a student was a heavy drinker or not, using two models: logistic regression & decision tree. These models did not performed well, when predicting if a student was a heavy drinker, which proably is because the low number of heavy drinkers in the dataset.

We also computed a regression model, which should predict the overall grade. This model included five response variables, which gave a Rsquared on 19,62% and RMSE around 3, which we considered as not that good. If the model should performe better, it need more explanatory variables, which could increase the Rsquared (explained variance) and reduce the RMSE, so the predictions would be better.
