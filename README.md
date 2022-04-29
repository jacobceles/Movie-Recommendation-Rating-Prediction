# Movie-Recommendation-Rating-Prediction
In this project, we have used the [MovieLens 100k dataset](https://grouplens.org/datasets/movielens/100k/) 
to compare different algorithms for rating prediction, and also create a movie recommendation system on top of it.
The dataset itself is open for public use since 1998, and has 100,000 ratings from 943 users on 1682 movies. Each user 
has rated at least 20 movies, and simple demographic info for the users (age, gender, occupation, zip) are given.

## Problem Statement
<ol>
    <li>Data preprocessing and split, create a training dataset and a testing dataset for experiment</li>
    <li>Rating prediction, develop an algorithm to predict the ratings in the testing set based on the information 
    (ratings and others) in the training dataset, and evaluate the predictions based on MAE and RMSE.</li>
    <li>Item Recommendation, construct a recommendation list for each user, and then evaluate the recommendation 
    quality based on precision, recall, and F-measure.</li>
</ol>

## Implementation
![High Level Design](Documents/approach.png?raw=true "High Level Design")

## Repository Structure
    ├── data                                 # Data used for the project
    ├── Documents                            # Holds documents realted to the project
    ├── README.md                            # Read this first
    └── code.ipynb                           # The code used for building the application

## How to Use
<ol>
    <li>Open code.ipynb in you jupyter installation.</li>
    <li>Run all the cells. The code inside will handle installing the required packages.</li>
    <li>If needed, you can easily modify the last cell to get recommendations for specific users.</li>
</ol>

## Results
|       RMSE and MAE scores       |                      Precision, Recall, and F-score                       |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|
| ![error_scores.png](Documents/error_scores.png?raw=true "RMSE and MAE scores") | ![precision_recall.png](Documents/precision_recall.png?raw=true "Precision, Recall, and F-score") |

### Recommendations
![Movie recommendation](Documents/recommendation.png?raw=true "Movie recommendations")

## Contributors
- [Jacob Celestine](https://jacobcelestine.com/)
- [Anirudh Negi](https://github.com/negiadventures/)
- [Meghana TN](https://github.com/MeghanaTN)

## References
- [Modin](https://github.com/modin-project/modin)
- [Surprise](http://surpriselib.com/)
- [Surprise Algorithms](https://surprise.readthedocs.io/en/stable/prediction_algorithms_package.html)
- [Surprise - Original Paper](https://joss.theoj.org/papers/10.21105/joss.02174)
- [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/100k/)
- [Issue: Adding more features to the train set](https://github.com/NicolasHug/Surprise/issues/285)