# machine-learning-challenge
## Exoplanet Exploration

## Background
Process data gathered by the NASA Kepler space telescope over a period of nine years in deep space and create machine learning models capable of classifying candidate exoplanets from the raw dataset.
SKLearn was used to create and determine the accuracy of these models.

## model_4
This model uses the variables categorized as 'Stellar Parameters' and fits the data to a Linear model. The r2 value for this model is extremely low (0.02), which means the model does not accurately predict the variation in the data. However, I reluctantly submit 'model_4' as my best model, even though in terms of r2 values, 'model_1' had a higher value, I was unable train and hyperparameter tune the variables used for models 1 and 2 with GridSearch. The GridSearch code was run for 3 days on my computer and... never stopped running. I believe this is due to the high number of combinations resulting from the models having more variables. I chose 'model_4' over 'model_3', although 'model_3' has a higher r2 value (0.04), because after hyperparameter tuning both models, 'model_4' had a higher accuracy (0.72) than 'model_3' (0.70). This still does not change the fact that 'model_4' is not an overall good model to classify the exoplanet data provided. I am no expert in planetary science, but the low predicatability of this model makes sense in that classifying the characteristics of the star a potential planet is orbiting does not necessarily correlate to a mass's potential as a planet--many masses orbit stars, after all.

# Submission
- Raw data `exoplanet_data.csv`
- Jupyter notebooks `model_1.ipynb`,`model_2.ipynb`,`model_3.ipynb`,`model_4.ipynb` containing training and testing of different classification models
- `Ariel_Kang.sav` containing the final `model_4` submission
