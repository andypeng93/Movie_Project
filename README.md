# Movie Data Analysis
## Flatiron Mod 1 Project

**Authors**: Andy Peng

The contents of this repository detail an analysis of the module one project. This analysis is detailed in hopes of making the work accessible and replicable.


### Business problem:

Microsoft tasked us into helping them understand the movie industry better. We need to retreive and explore the data relating to the movie industry. First thing to do is gather as much data relating to the movie industry as we can. Then I want to explore each dataset and see if any are worth joining together to create an even more interesting dataset. After that I want to explore the relationships between genres, directors, ratings, revenues and runtime of movies.


### Data
The following list contains the resources we used to perform our data analysis on the data relating to the movie industry.
* Box Office Mojo
* IMDB
* Rotten Tomatoes
* TheMovieDB.org
* Kaggle tmdb movie data downloaded from https://www.kaggle.com/juzershakir/tmdb-movies-dataset


## Methods
- Descriptive Analysis
- Choices made
- Key relevant findings from exploritory data analysis

## Results


#### Ratings Visual 1
<img src=./Images/directorratings.PNG width="800">
> Director's Average Movie Ratings

#### Ratings Visual 2
<img src=./Images/populardirectors.PNG width="800">
> Director's Popularity VS Average Movie Ratings

#### Ratings Visual 3
<img src=./Images/genreratings.PNG width="800">
> Average Movie Ratings for each type of genre

#### Ratings Visual 4
<img src=./Images/runtimeratings.PNG width="800">
> Length of Movies VS Ratings

#### Visual 5
![graph5](./Visualizations/AgeMax.PNG)
> Age of Individuals VS Maximum Heart Rate

#### Models
![ROC Curve](./Visualizations/ROC1.PNG)
> ROC Curve of the different Models

![Model Results](./Visualizations/ModelResults.PNG)
> Model Results of Base Model and Model Tuning

* AUC - Random Forest with GridSearchCV

* Accuracy/ F1 Score/ Recall - XGBoost

* Precision - Decision Tree with GridSearchCV



## Recommendations:

To summarize everything above, we can see from above that to correctly classified a patient as having heart disease we need to consider the following features.

1) Gener of the individual - Males have a higher chance at having heart disease than females.

2) Asymptomatic Chest Pain - Individuals with this type of chest pain have a high chance of having heart disease

3) Reversable Defect - If the thalium stress result turns out to be reversable defect, the individual would have a high chance of having heart disease.

4) Age & Maxium Heart Rate - As you get older, your maximum heart rate goes down. We can see that individuals that have heart disease tend to be older and have a lower maximum heart rate.

Our modeling shows that a regular XGBoost is the best model for our problem. This is because we want a model that generates a high recall value in order to minimize the chance of us classifying an individual as false negatives. Being that heart disease is really serious, it would be dangerous if we wrongly classify a person with no heart disease when they indeed do have heart disease.


## Limitations & Next Steps

There are many features that we haven't considered. For example whether the family has a genetic disorder, body fat percentage, and the individual's diet. Also our model can be further improved by gathering more patient's information.


### For further information
Please review the narrative of our analysis in [our jupyter notebook](./Heart Disease.ipynb) or review our [presentation](./SampleProjectSlides.pdf)

For any additional questions, please contact **andypeng93@gmail.com)


##### Repository Structure:

Here is where you would describe the structure of your repoistory and its contents, for example:

```

├── README.md                       <- The top-level README for reviewers of this project.
├── Heart Disease.ipynb             <- narrative documentation of analysis in jupyter notebook
├── presentation.pdf                <- pdf version of project presentation
└── Visualization
    └── images                          <- both sourced externally and generated from code

```
