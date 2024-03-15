# COMP 551 Applied Machine Learning Course Project 2: Self-implemented NLP Analysis Algorithms

## Overview

This repository showcases our exploration and implementation of logistic regression and multi-class regression algorithms applied to text data, without direct reliance on Scikit-learn's built-in algorithms. Our work encompasses the preprocessing of datasets, feature selection through simple linear regression coefficients and mutual information scores, and the development of logistic and multi-class regression models from scratch. We validated our models using small perturbations and monitored cross-entropy to ensure robustness and accuracy. Our implementations were benchmarked against Scikit-learn's decision tree algorithm, demonstrating superior performance in terms of training speed and predictive accuracy.

## Datasets

### IMDB Reviews

The IMDB dataset consists of 50,000 movie reviews, split evenly between training and testing sets. The goal is to classify reviews as positive (rating > 5) or negative (rating <= 5) based on word frequencies. We applied preprocessing steps such as filtering out rare and common words and selected the top 500 words with the highest absolute coefficients from a simple linear regression as features.

### 20 Newsgroups

The 20 Newsgroups dataset is a collection of newsgroup documents, categorized into multiple classes. We focused on five specific categories for our analysis: comp.graphics, misc.forsale, rec.sport.baseball, sci.med, and talk.politics.guns. Feature selection was performed using mutual information, resulting in a final set of 368 unique features across the chosen categories.

## Key Results

- Implemented logistic regression and multi-class regression algorithms from scratch.
- Demonstrated higher accuracy and faster training times compared to Scikit-learn's decision tree algorithm.
- No signs of overfitting were observed within the defined maximum number of iterations.
- Employed sparse matrix representations for efficient memory usage and computational speed.
- Explored the effects of different learning rates and expanded the analysis to include more classes in the 20 Newsgroups dataset.

## Contributions

- **Jimmy Sheng**: Implemented IMDB word filtering, introduced sparse matrices, and wrote the logistic regression task.
- **Iris Wang**: Contributed to IMDB word filtering comparison and authored the report, including plot generation.
- **Keyu Wang**: Collaborated on the multi-class regression task and spearheaded the creativity section.

## Acknowledgments

We extend our gratitude to the course instructors and TAs of COMP 551 for their invaluable guidance throughout this project. Our appreciation also goes to the creators and maintainers of the IMDB and 20 Newsgroups datasets for providing rich data sources for our analysis.
