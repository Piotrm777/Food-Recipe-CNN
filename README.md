<div align="center">
  <img src="https://i.imgur.com/NDDPCQY.png"><br><br>
</div>

-----------------

# Deep Learning food image recognition system for cooking recipe retrieval

## Overview

### Update: The Blog Article is now out. Visit [the turorial on Medium](https://medium.com/@Muriz.Serifovic/this-ai-is-hungry-b2a8655528be) for further information!

Maturaarbeit 2018: This work makes usage of deep convolutional neural networks with Keras to classify images into 230 food categories and to output a matching recipe. The dataset contains >400'000 food images and >300'000 recipes from chefkoch.de.

Hardly any other area affects human well-being to a similar extent as nutrition. Every day countless of food pictures are published by users on social networks; from the first home-made cake to the top Michelin dish, the joy of the world is shared with you in case a dish is successful. It is a fact that no matter how different you may be from each other, good food is appreciated by everyone. Advances in the classification or object recognition of individual cooking ingredients are sparse. The problem is that there are almost no public edited records available.

The code (Jupyter notebooks) is provided with numerous comments in German.
The process looks like this:

1│── **Data preparation**  
  │   └── Clearing data  
  │   └── Data augmentation  
  
2│── **Data Analyse und Visulation, Daten splitten (Train, Valid, Test)**  

3│── **Versuche mit ersten einfachen ML Modellen**  
  │   └── Nearest Neighbor classifier (kNN)  
  │   └── k-Means Clustering  
  │   └── Support Vector Machine   
  
4│── **Transfer Learning: Training von pre-trained CNN (Convolutional Neural Network)**  
  │   └── AlexNet, VGG, ResNet, GoogLeNet  
  
5│── **Training von eigenem CNN**  
  │   └── Optimization  
  
6│── **Ergebnisse visualisieren**  

7└── **Erstellen einer ~~Android~~ Web Applikation** (still open)

## Abstract

This work deals with the problem of automated recognition of a photographed cooking dish and the subsequent output of the appropriate recipe. The distinction between the difficulty of the chosen problem and previous supervised classification problems is that there are large overlaps in food dishes, as dishes of different categories may look very similar only in terms of image information. The task is subdivided into smaller areas according to the motto *divide and conquer*: According to the current state, the largest German-language dataset of more than 300'000 recipes will be presented, with a newly developed method, according to the author's knowledge, presented by the combination of object recognition or cooking court recognition using Convolutional Neural Networks (short CNN) and the search of the nearest neighbor of the input image (Next-Neighbor Classification) in a record of over 400,000 images. This combination helps to find the correct recipe more likely, as the top-5 categories of the CNN are compared to the next-neighbor category.

## DeepChef

<div align="center">
  <img src="https://i.imgur.com/IkTHOG8.png" width=50%><br><br>
</div>

The result is the product DeepChef. The web application (coming soon) expects a meal picture as input. As a result, you get the associated recipes.
