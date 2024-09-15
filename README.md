# Waste-Classification-using-Deep-Learning

This project addresses the business problem of efficiently classifying waste into distinct categories to support automated waste sorting systems, a critical need in waste management for improving recycling efforts and reducing environmental impact. The classification of waste materials can significantly enhance the operational efficiency of recycling facilities, leading to better resource management and sustainability.

## Business Problem:

With the growing emphasis on sustainable practices, recycling and waste management are essential processes for minimizing environmental damage. Manual sorting of waste is time-consuming and prone to errors, creating a demand for automated systems that can classify waste materials accurately. The goal of this project is to develop a machine learning model capable of automatically classifying six types of waste (cardboard, glass, metal, paper, plastic, and vegetation) based on image data. Improving the accuracy of waste classification would lead to increased recycling rates and reduced contamination in waste streams.

## Dataset:

The dataset comprises 2,864 labeled images across six categories of waste:

Cardboard: 461 images
Glass: 420 images
Metal: 547 images
Paper: 500 images
Plastic: 500 images
Vegetation: 444 images
The images were preprocessed, and a variety of deep learning models were applied to classify the waste types accurately.

## Methods:

We explored three deep learning architectures to classify the waste images:

Artificial Neural Network (ANN): A simple model with one hidden layer.
Convolutional Neural Networks (CNNs): Two CNN architectures were developed, including the best-performing model, which consisted of multiple convolution layers, max pooling layers, and dense layers, with dropout to prevent overfitting.
Key Performance Indicators (KPIs):

Test Accuracy: Measures the model's ability to correctly classify unseen data.

Kappa: A metric that corrects for chance agreement, providing a more accurate measure of performance.

Precision: Measures the proportion of positive predictions that are actually positive.

Recall: Measures the proportion of actual positive cases that are correctly predicted as positive.

F1-score: The harmonic mean of precision and recall, providing a balanced measure.

## Experiments:

Twelve models were experimented with:

Model 3 and Model 11 consistently demonstrate strong performance across all KPIs, indicating their superiority in terms of overall classification accuracy and balanced performance.

Models 5 and 1 exhibit poor performance, likely due to overfitting or underfitting issues.

Models 2, 4, 6, 7, 8, 9, 10, and 12 show varying degrees of performance, with some models excelling in specific metrics while others struggle in others.

## Results:

The best-performing model (Model 3) achieved a strong overall test accuracy of 70.65% with a kappa score of 0.648, indicating moderate agreement. Among the categories, "plastic" was the most challenging to classify, with a precision of 0.51, recall of 0.63, and an F1-score of 0.70, indicating the need for further optimization to enhance the classification performance of this class.

This project demonstrates that advanced CNN architectures are effective for image-based waste classification, although further model refinements and class-specific adjustments are necessary to improve overall accuracy, particularly for challenging classes like plastic.
