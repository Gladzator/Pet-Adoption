# Pet-Adoption

## Table of Content
  * [Problem Statement](#problem-statement)
  * [Data](#data)
  * [Installation](#installation)
  * [About files](#about-files)
  * [Technical Approach](#technical-approach)
  * [Technologies/Libraries Used](#technologieslibraries-used)
  * [Team](#team)
  * [Credits](#credits)
  
## Problem Statement
This problem statement was part of a HackerEarth competition called "HackerEarth Machine Learning challenge: Adopt a buddy".

A leading pet adoption agency is planning to create a virtual tour experience for their customers showcasing all animals that are available in the shelter. To enable this tour experience, we are required to build a Machine Learning model that determines type and breed of the animal based on its physical attributes and other factors.

## Data

| Sr No.        | Column Name   | Description  |
| ------------- |:-------------:| -----:|
| 1 | pet_id | Unique Pet Id |
| 2 | issue_date | Date on which the pet was issued to the shelter |
| 3 | listing_date | Date when the pet arrived to the shelter |
| 4 | condition | Condition of the pet |
| 5 | color_type | Color of the pet |
| 6 | length(m) | Length of the pet (in meter) |
| 7 | height(cm) | Height of the pet (in centimeter) |
| 8 | X1,X2 | Anonymous columns |
| 9 | breed_category | Breed category of the pet (target variable) |
| 10 | pet_category | Category of the pet (target variable) |

## Installation
The Code is written in Python 3.7.6. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```
## About files
  - train.csv : Input train file.
  - test.csv : Input test file.
  - train_updated.csv / test_updated.csv : Modified train/test file after running EDA-1 and Feature Generation.
  - train_norm.csv / test_norm.csv : Modified train_updated/test_updated file after running EDA-2 and Feature Generation.
  - predicted_test_pet : Predicted pet category for test data after running Pet_prediction.
  - submission : File containing predicted pet and breed category for test data after running Breed_predict.
 
 ## Technical Approach
 This project is divided into three part:
 1. Performing EDA(Exploratory Data Analysis) to understand data much better.
 2. Generating new Features.
 3. Using ensemble technique to predict pet and breed categories.
  - Interesting knowledge about data is incurred from EDA-1 and Feature Generation file where new feature namely date_diff is generated and nan values are handled.
  - EDA-2 and Feature Generation delves into data and handles the categorical feature namely color_type. Two pairplots are even generated to see the distribution of data and get further more understanding of the same.
  - Ensemble technique namely XGBoost is used to make predictions.
  
## Technologies/Libraries Used
![](https://forthebadge.com/images/badges/made-with-python.svg)
 
[<img target="_blank" src="https://matplotlib.org/_static/logo2_compressed.svg" width=100>](https://matplotlib.org/)[<img target="_blank" src="https://numpy.org/images/logos/numpy.svg" width=100 height=100>](https://numpy.org/)

[<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=100>](https://scikit-learn.org/stable/)[<img target="_blank" src="https://seaborn.pydata.org/_static/logo-wide-lightbg.svg" width=100>](https://seaborn.pydata.org/)

## Team
<img src="https://avatars2.githubusercontent.com/u/40065133?s=460&v=4" width="200" height="200">|
-|
Yash Vora

## Credits
I want to give massive credits to the HackerEarth team without whom this project wouldn't have been possible.

 
