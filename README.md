# Predicting the Success of Pirate Attacks

This repo took shape during my Data Science course at [Propulsion Academy](https://propulsion.academy/) in Zurich and was inspired by various in-class exercises. It gives a good overview of the content covered during the first month.

![](notebooks/lego_pirates.jpg)

Image copyright: LEGO Group

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#assignment-description">Assignment Description</a></li>
    <li><a href="#approach">Approach</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#conclusion">Conclusion</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- Assignment Description -->
## Assignment Description

The task is to predict from a data set of 802 pirate attacks whether a pirate attack will be successful or not. This includes first exploring, cleaning and preprocessing the data, then feeding it into different models to compare their performance and finally fine-tuning and explaining the best-performing model.

<!-- Approach -->
## Approach

The process was the following:

First, the data was cleaned (part 2 of the jupyter notebooks), then some interesting visualizations were created (part 3) to explore the data set and see if there are any trends that are clearly visible. 

The data was preprocessed (part 4), which meant one-hot-encoding most of the variables, since much of the data is categorical. The selected features were then fed into seven different untuned baseline models (part 5). The model with the best performance was fine-tuned and tested (part 6).

As a final step, feature importance and SHAP values of the best model were explored (part 7) to explain how the model reaches its predictions.

Please note that the interactive visualizations in the notebooks 3 and 7 require Java Script and therefore will not render on GitHub. Instead, you can view them on [nbviewer](https://nbviewer.jupyter.org/).

<!-- Results -->
## Results

The Random Forest Classifier performed best overall and was therefore fine-tuned. One of the goals of the fine-tuning, besides improving the performance, was to prevent overfitting. The model finally achieved a performance of about 65% balanced accuracy on the test set. The features with the biggest impact on the prediction were the longitude and latitude of the attack location.

<!-- Conclusion -->
## Conclusion

As the results show, it is partially possible to predict the success or failure of pirate attacks from the limited amount of data provided. Overfitting of the model to the training data remains a problem, even after cleaning the data and partially constraining the model. This requires further work and it might also be interesting to finetune a more simple model, such as a logistic regression.
It is also likely that better results could be achieved with additional data, especially since the data set covers a timespan of only 18 months.

<!-- Contact -->
## Contact

If you find this repo interesting or would like to suggest improvements, please get in touch. I would be happy to hear from you.
