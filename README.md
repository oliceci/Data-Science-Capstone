# Movie Production Investment - Data Science Capstone Project
## What is this about?
For the end of a 3 months immersive course in Data Science, I have worked on a Movie Production Investment project to predict movies that would be successful or have a high review score. With the increase of streaming platforms and the consumption of movies as “fast” culture, I want to analyse a regression and classification model focused on budget, tagline, IMDb voting of films.

This would be targeted to cultural investors, corporates interested in investing in the arts, film production companies, government cultural departments or even film councils and festivals.

The success metrics would be revenue, ROI, IMDb score and valid investment.

Apart from the regression and classification models to determine, I will also use an NLP to review which keywords are more likely used in successful movies.

You can find the full final presentation here: [Presentation](https://drive.google.com/file/d/13ArjcJvJxSgU26o6gYyKnUr5I4HkOlHa/view)

## The Data
The dataset has come from Kaggle: [link](https://www.kaggle.com/rounakbanik/the-movies-dataset?select=movies_metadata.csv) and reports on movies from 1902 up to July 2017. It has 45,000 rows and 23 columns.

The data within the columns was not as clean so with slicing and Regex I have managed to have more readable and comparable data. ![](column_clean.png)

Once I cleaned all the data, I created new variables as year, month and day release, as well as ROI. That's when I realized that my dataset had been reduces to less than 15%. As films were from such a large time frame, I have also taken into consideration the inflation throughout the years.

## EDA
Whilst doing the EDA, I realised that many film productions had very high, or low numbers and have done some clean to take away outliers. Analysing the heatmap, I have realized that the ROI is not very correlated to the variables, which made me review how we could do not only a regression but also a classification problem. 

It was also very important to understand what are the most profitable production companies, genres, countries and year. 

## Modeling
I have decided to split this into three parts: Regression, Classification and NLP.

### Regression
I have done regression modeling with ROI, Vote Average and Revenue (after inflation) and used Linear Regression, Ridge, Lasso, Elastic Net, Gradient Boosting Regressor and MLP Regressor. 

#### ROI
Gradient Boosting Regressor
Best Mean Cross-validation scores: -6.964105485269398
Train score: 0.9999251487004943
Test score: 0.32616472228789206

#### Vote Average

