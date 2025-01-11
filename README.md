# Life Expectancy Analysis Using Multiple Linear Regression

This repository contains an analysis of the factors that influence human life expectancy. The data, collected from 193 countries between 2000 and 2015, identifies variables with a significant impact on life expectancy. Multiple linear regression and data-cleaning techniques are applied to highlight measures that can potentially increase citizens’ average lifespan.

---

## 1.0 Abstract

It has become increasingly common for humans to live past 70 years of age in contemporary times, irrespective of gender, which was not as common only a few decades ago. Through the thorough analysis of data provided by [The Global Health Observatory (GHO) data repository](https://www.who.int/data/gho), a branch under the World Health Organization (WHO), factors that significantly impact human life expectancy can be identified.

Data from 193 countries collected between 2000 and 2015 highlight 20 variables suspected of influencing life expectancy. Multiple linear regression is used to identify characteristics that may affect life expectancy. The inclusion of numerous nations facilitates the detection of elements contributing to lower life expectancy, guiding the policies required to raise citizens' average lifespan.

The dataset contains multiple missing values that must be addressed. Most of the missing data pertains to population, Hepatitis B, and GDP. These missing values occur primarily in countries with less-documented data, such as Vanuatu, Tonga, Togo, Cabo Verde, etc. Due to the difficulty in finding consistent data for these countries, they were excluded from the final model dataset.  

The raw dataset consists of 22 columns and 2938 rows, incorporating 20 predictive variables. Predictive variables are divided into the following categories:  
- **Immunization-related factors**  
- **Mortality factors**  
- **Economic factors**  
- **Social factors**

Detecting and removing null values allowed the cleaning of data and the removal of outliers.

---

## 2.0 Introduction

Life expectancy can be influenced by a variety of factors. The data, gathered from 193 countries, record 22 external variables that affect human life expectancy. Factors such as alcohol consumption are suspected of impacting the lifespan. By applying a multiple linear regression model, variables that exhibit a significant correlation with life expectancy can be identified.

**Linear regression** evaluates the relationship between two variables by constructing a straight-line model based on a dataset. Since more than one variable is being evaluated, a **multiple linear regression** approach is necessary to estimate the relationship between a quantitative dependent variable and multiple independent variables.

Before building the multiple linear regression model, a thorough study is carried out on the topic under evaluation to understand why certain variations may occur. Including several variables helps generate better predictions and potentially yields more accurate results. Some variables may be removed if they do not contribute to an accurate model.

**Backward elimination** is applied to ensure that the chosen variables correspond to the model. Variables displaying **multicollinearity**—where independent variables have a relationship with one another—must be removed. Excess variables may also lead to **overfitting**, where the model becomes too complex. These steps lead to a more precise adjusted R² value.

