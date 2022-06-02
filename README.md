# Diamond price prediction algorithms

The R and R Markdown code in this respository covers several supervised machine learning algorithms to predict the price of diamonds. It includes linear regression using lm, generalized linear regression using glmnet, random forest using the ranger engine, and deeplearning using keras.

The **diamond-price-prediction.Rmd** Markdown file in this repository analyzes the **diamonds** dataset from the **tidymodels** library, trains several machine learning models and crossvalidates and tunes them for the optimal performance.

## Requirements

The R script requires the following packages and their requirements:

```r
library(tidymodels)
library(GGally)
library(gridExtra)
```
## Settings

In the ggpairs plot eval is set to FALSE to decrease time to knit the document. Set eval to TRUE to plot the correlation plots of the variables.

```r
{r, out.width='100%', fig.height=7, eval=FALSE}
```


## Results

The table below shows the result of the R-Squared values for the four different supervised machine learning models:

| Engine        | Model                         | R-Squared Value     |
| ------------- | ----------------------------- | ------------------- |
| ranger        | random forest                 | 0.984               |
| lm            | Linear regression             | 0.965               |
| glmnet        | Generalized linear regression | 0.965               |
| keras         | Deep Learning                 | 0.965               |
