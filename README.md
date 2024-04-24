# DS-5780-NLP
This is the repository of NLP final paper. All the code is in the code.ipynb.


## Data
The dataset could be available at: https://www.kaggle.com/datasets/ermoore/pitchfork-reviews-through-12617 
 
The dataset is the historical reviews of Pitchfork from January 5th,1999 to December 6th, 2017. The total number of music reviews is 19,554. The music reviews are across different genres including Rock, Rap, Pop, Country, Electronic and Experimental. The text of each review is the raw context in English. The predictor music album review score is a decimal score on the scale of 0 to 10. According to the description of the da-taset, the entire dataset was obtained through web crawling.

## Methodology

In this repo, the following methodologies are operated:

### TF-IDF

We vectorize each review using TF-IDF. The TF-IDF vectorizer we apply is from Scikit-learn library. To manage the vectorization process effectively, a threshold was set to include words that appear at least five times across the dataset. This approach ensures the matrix reflects more meaningful textual features. Additionally, a sublinear scaling on term frequency is applied, meaning that the logarithm of the term frequency (plus one) is used instead of the raw frequency, to temper the impact of highly recurrent yet less informative words. 


### Ridge regression

We train a Ridge regression on the TF-IDF matrix.

### Residual Analysis

Residual analysis is used to assess the performance of Ridge regression model in this study. Residual is the differ-ence between the observed value and the value predicted by the model. Residual analysis is a useful diagnostic tool in regression analysis. By plotting residuals against predicted values or other independent variables, we might be able to assess the appropriateness and accurcacy of the regression model visually.


### Feature Importance Analysis

The analysis of important feature of Ridge regression.
