# Movie_Revenue_Prediction_and_Success_Classification
The project scope is to analyze movie datasets to try to predict flops, successes, and major successes. And, to predict the revenues.

The original Kaggle notebook is available at https://www.kaggle.com/code/victorpaschoalini/movie-revenue-prediction-success-classification/notebook

Links to the data used: https://www.kaggle.com/datasets/joebeachcapital/top-500-hollywood-movies-of-all-time and https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?select=movies_metadata.csv

Here are the conclusions:

Conclusions:

- The last model works much better than the initial one (MAE of ~60 M compared to ~200 M), this could be because we are using movies with smaller budgets, so more research is needed. Also, the model struggled a lot to make the success status predictions, a quick fix may be trying to use the estimated budgets to make a new ROI estimated column.

- This work highly suggests that it is very possible to predict flops and success with the only information available in the making or even before the making of the movie... knowing that Hollywood loses hundreds of millions of dollars per year with flops, research in this direction is highly recommended.

(The following are the more technical conclusions)

Regression Model (Revenue Prediction):

- The Mean Absolute Error (MAE) is approximately USD 58.7 million. While this might seem significant, it's essential to consider the range and scale of movie revenues, which can vary widely from a few thousand dollars to billions.

Classification Model (Success Category Prediction):

- The model's accuracy is approximately 46.80%. The model has a higher precision and recall for the categories "Flop" and "Major Success" but struggles with the "Success" category.

- The imbalanced nature of the dataset might be a reason for this. There might be fewer samples of movies categorized as "Success" compared to the other categories.

Observations:

- Both models seem to have a bias toward predicting movies as either "Flop" or "Major Success". This could be due to the imbalanced distribution of the success categories in the dataset.

- The regression model, in some cases, tends to overestimate the revenue, especially for movies with moderate budgets.
