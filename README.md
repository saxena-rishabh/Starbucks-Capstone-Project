# Starbucks Capstone Project

**The link to the Blog post is [here](https://medium.com/@saxena_rishabh/analyzing-starbucks-app-offers-54557645a138)**
## Table of Contents

- [1. Project Overview](#overview)
- [2. Project Motivation](#motivation)
- [3. Project Components](#components)
- [4. Files](#files)
- [5. Software Requirements](#sw)
- [6. Conclusion](#conclusion)
- [7. Credits and Acknowledgements](#credits)

***

<a id='overview'></a>

## 1. Project Overview

The data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

My task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Because this is a capstone project, I am free to analyze the data any way I see fit. For example, I could build a machine learning model that predicts how much someone will spend based on demographics and offer type. Or I could build a model that predicts whether or not someone will respond to an offer.

<a id='motivation'></a>
## 2. Project Motivation
This project is the Capstone project of my Data Scientist nanodegree with Udacity. As students in the nanodegree, we have the option to take part in the Starbucks Capstone Challenge. For the challenge, Udacity provided simulated data that mimics customer behavior on the Starbucks rewards mobile app.

In this project, I use the data to answer a business questions:
<ul>
    <li>Which demographic groups respond best to which offer type.</li>
<li>And create Machine Learning model to predict whether a customer will complete a offer by making transaction after viewing the offer.</li>
 </ul>

<a id='components'></a>

## 3. Project Components

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

├── notebook 
├── data - contains dataset in JSON format


</pre>

<a id='sw'></a>

## 5. Software Requirements

This project uses **Python 3.6** and the following necessary libraries:
<ul>
    <li> pandas </li>
    <li> numpy </li>
    <li> math </li>
    <li> json </li>
    <li> matplotlib </li>
    <li> sklean </li>
    <li> seaborn </li>
    <li> scipy </li>
</ul> 


<a id='conclusion'></a>

## 6. Conclusion

Overall, I found this project interesting and challenging, mainly due to the structure of the data. I had started out with the business question: <br>
<ul>
    <li>Which demographic groups respond best to which offer type.</li>
    <li>And create Machine Learning model to predict whether a customer will complete a offer by making transaction after viewing the offer.</li>
</ul>
So with Explanatory Data Analysis, I found
<ul>
<li>Male and Female almost equally complete the offer. So offers should be sent equally among them.</li>
<li>The two most completed offer of type are 'BOGO' and 'Discount'. So these two should be sent to more people.</li>
<li>People of age 50–70 of income between 60000–90000 respond most to offers type 'BOGO' and 'Discount'. So it will be good to send BOGO and Discount offers to these people.</li>
</ul>

And created a Machine Learning model using Random Forest Classifier with hyperparameter tuning to predict whether a customer will complete an offer by making transaction after viewing the offer with the accuracy of 1. I may be getting an accuracy of 1 due to considering only the most important features and dropping all unnecessary features.

**Future Work**:
<ul>
  <li>There may be overfitting which can be solved by considering more data.</li>
  <li>Build Machine Learning Pipeline to seamlessly classify new data.</li>
  <li>Make Machine Learning model to predict transaction amount.</li>
  <li>Deploy Machine Learning model to web.</li>
</ul>

## 7. Credits and Acknowledgements

Thanks to [Udacity](https://www.udacity.com/) for providing dataset.
