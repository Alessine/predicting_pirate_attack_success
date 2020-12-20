# Predicting the Success of Pirate Attacks

This repo took shape during my Data Science course at Propulsion Academy in Zurich and was inspired by various in-class exercises. It gives a good overview of the content covered during the first month.

![](pirates_asterix.jpg)

<font size = "2"> Image copyright: Asterix & Obelix </font>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#assignment-description">Assignment Description</a></li>
    <li><a href="#approach">Approach</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#conclusion">Conclusion</a></li>
  </ol>
</details>

<!-- Assignment Description -->
## Assignment Description

Following is a short description of the assignment:

>You are provided with a dataset on vessels that have been attacked by pirates. Your task is to predict whether an attack is likely to be successful.
>
>Clean and preprocess the data. This includes:
>- Select features.
>- One-hot encode categorical variables.
>- How do you handle the date?
>- Aggregate categories with few occurrences.
>
>Compare the performance of different models. Run all of them, identify the best performing one and tune it. Finally, explain how it reaches a prediction. </font>

<!-- Approach -->
## Approach

The systematic approach taken to solve the problem was as follows. 

First, the data was cleaned (section 2 in the jupyter notebook), then some interesting visualizations were created (section 3) to explore the data set and see if there are any trends that are clearly visible.

The data was then preprocessed (section 4), which meant one-hot-encoding most of the variables, since much of the data is categorical. The selected features were then fed into seven different untuned baseline models (section 5). The model with the best performance was fine-tuned and tested.

As a final step, feature importance and SHAP values of the best model are explored to explain how the model reaches its predictions.

<!-- Results -->
## Results

The Random Forest Classifier performed best overall and was therefore fine-tuned. One of the goals of the fine-tuning, besides improving the performance, was to prevent overfitting. The model finally achieved a performance of about 62% accuracy on the test set. The features with the biggest impact on the prediction were the longitude and latitude of the attack location.

<!-- Conclusion -->
## Conclusion

It becomes clear therefore...

