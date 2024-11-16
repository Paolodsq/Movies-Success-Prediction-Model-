## Dataset Source:
https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies/data

The dataset is from the TMDB community and consists of 1M+ movies from late 19th century till 2024. The dataset was then reduced to 10K observations due to missing values and specific research goals.

## Research Goals:
Provide valuable insights that could be leveraged by a local cinema chain. In particular:
1. Gain consumer preference insights.
2. Optimize movie offerings: identify movies that lead to higher chances of being successful, while reducing risk of selecting movies that will not succeed. Goal: Increase long-term customer retention. 
3. Forecast the number of movies that will be released monthly, enabling more effective budget planning and promotional activities. Goal: Effective scheduling.

## Target Variable:
The success of a movie can be defined both quantitatively, in terms of revenues, and qualitatively, in terms of popularity and reviews. So the target variable is going to be a binary variable which combines revenues and vote_average, making this a classification problem. 

## Models Evaluation:
Several configurations of classification models have been implemented and compared, including: 
- Logistic Regressions (algorithm: Newton-Raphson/SGD, regularization: LASSO/Ridge)
- Classification Trees (pruning/no pruning, Gini Index/Gain Ratio)
- Random Forest (Information Gain/Information Gain Ratio/Gini Index)
- XGBoost (parameter optimization loop/feature selection loop)
- MLP

## Best Model:
Random Forest with Information Gain splitting rule (Accuracy = 0.748, AUC = 0.803)







