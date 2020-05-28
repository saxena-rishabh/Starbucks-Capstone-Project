# Starbucks-Capstone-Project

## Table of Contents

- [Project Overview](#overview)
- [Project Components](#components)
- [Files](#files)
- [Software Requirements](#sw)  
- [Credits and Acknowledgements](#credits)

***

<a id='overview'></a>

## 1. Project Overview

In this project, I'll apply data engineering to analyze disaster data from <a href="https://www.figure-eight.com/" target="_blank">Figure Eight</a> to build a model for an API that classifies disaster messages.

_data_ directory contains a data set which are real messages that were sent during disaster events. I will be creating a machine learning pipeline to categorize these events so that appropriate disaster relief agency can be reached out for help.

I will also build a web app where an emergency worker can input a new message and get classification results in several categories. The web app will also display visualizations of the data.

[Here](#ss) are a few screenshots of the web app.

<a id='components'></a>

## 2. Project Components

<ol>
    <li> Importing Libraries and Reading Dataset </li>
    <li> Data Wrangling </li>
    <li> Exploratory Data Analysis </li>
        <ol>
            <li> Univariate Analysis </li>
                <ol>
                    <li> Distplot </li>
                    <li> Bar Plot</li>
                </ol>
            <li> Bivariate/Multivariate Analysis </li>
                <ol>
                    <li> Count Plot </li>
                    <li> Box Plot</li>
                    <li> Correlation</li>
                </ol>
         </ol>
     <li> Explanatory Data Analysis </li>
     <li> Model Building </li>
     <li> Hyperparameter Tuning </li>
     <li> Conclusion </li>
</ol>


<a id='files'></a>

## 4. Files

<pre>
.
├── app
│   ├── run.py------------------------# FLASK FILE THAT RUNS APP
│   ├
│   │   
│   └── templates
│       ├── go.html-------------------# CLASSIFICATION RESULT PAGE OF WEB APP
│       └── master.html---------------# MAIN PAGE OF WEB APP
├── data
│   ├── DisasterResponse.db-----------# DATABASE TO SAVE CLEANED DATA TO
│   ├── disaster_categories.csv-------# DATA CONTAINING DISASTER CATEGORIES
│   ├── disaster_messages.csv---------# DATA CONTAINING DISASTER MESSAGES
│   └── process_data.py---------------# PERFORMS ETL PROCESS
├── requirements.txt-------------------------------# CONTAINING ALL DEPENDENCIES
├── models
│   ├── train_classifier.py-----------# PERFORMS CLASSIFICATION TASK
    └── classifier.pkl----------------# SAVED MODEL

</pre>

<a id='sw'></a>

## 5. Software Requirements

This project uses **Python 3.6** and the necessary libraries are mentioned in _requirements.txt_.

<a id='credits'></a>

## 7. Credits and Acknowledgements

Thanks to [Udacity](https://www.udacity.com/) and [Figure Eight](https://www.figure-eight.com) project for providing original dataset with [Multilingual Disaster Response Messages](https://www.figure-eight.com/dataset/combined-disaster-response-data).



