# Breast Cancer Prediction

## Project Overview

In this project I created a machine learning model that can predict breast cancer diagnoses. The motivation for this project was my own experience as a cancer patient, and my determination to help other people.

## Data Description

The dataset used in this project is sourced from the UCI Machine Learning Repository and can be accessed [here]([https://www.kaggle.com/datasets/iramshahzadi9/remote-work-and-mental-health](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)). It contains measurements on cells in suspicious lumps in a women's breast. Ten real-valued features are computed for each cell nucleus. Features are computed from a digitized image of a fine needle aspirate of a breast mass. They describe characteristics of the cell nuclei present in the image:

- **Radius**
- **Texture**
- **Perimeter**
- **Area**
- **Smoothness**
- **Compactness**
- **Concavity**
- **Concave points**
- **Symmetry**
- **Fractal Dimension**

The mean, standard error, and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.

These features will be use to create our classification algorithm .
  
## Libraries Used

- **Pandas**: For data cleaning, transformation, and analysis
- **NumPy**: For numerical operations
- **Scikit-learn**: For machine learning algorithms
- **Matplotlib & Seaborn**: For data visualization

## EDA and Preprocessing

I checked for missing and duplicate values, which fortunately there were none. I also checked for outliers, but due to the nature of our data decided to keep them since they could be crucial for extraordinary cases.



![Bar1](bar1.png)

While the average work life balance rating doesn't really change much between region, there is a very slight difference between each work location, with Onsite jobs being on average the work location with the lowest average work life balance rating (2.95).


![Bar2](bar2.png)

Stress level remains kind of the same between all the industries in the dataset, although the education and the healthcare industries both have a higher average stress level reported between employees (2.05, 2.04, respectively).



**Correlation Analysis**

![lineplot](lineplot.png)

To see how weekly worked hours affect stress levels among employees, I used this lineplot. There's clearly no correlation between the two variables, as there isn't a trend happening when weekly worked hours increase.
