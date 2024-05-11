
---
title: "Clustering and Classifying Images "
categories:
  - Blog
tags:
  - Post Formats
  - notice
toc: true
toc_label: "Assignment 4"
toc_sticky: true
toc_icon: "calendar" #"book"

---
---

>### Try This:

>(1) Begin by powering on your iPhone and navigate to your photo album.
>(2) Search through your collection to find a favorite picture of your beloved cat or dog.
>(3) Once you've selected an image, swipe upwards on the screen.

Do you notice how your iPhone offers insights about the breed of your cherished pet? Apple incorporates an extensive database filled with countless images to train its machines. This technology allows your iPhone to recognize various pet breeds by comparing your pet’s image with the ones in its database.

<img src="/assets/images/assignment2_images/1.png" style="zoom:60%;" />

## How Do Machines Recognize Your Pet? Exploring Machine Learning in Distinguishing Cats and Dogs

## Introduction and Database Utilization

To understand how the software Orange processes and categorizes images, I initiated an experiment by downloading a diverse set of cat and dog pictures from Kaggle. Utilizing a predefined data analysis workflow in Orange, I imported these images. The software then organizes them into a visual grid format. This grid helps infer the criteria used by the machine to categorize each image.

<img src="/assets/images/assignment2_images/procedure.jpg" style="zoom:25%;" />

## Clustering Techniques
### Grid Representation

By consolidating the cat and dog images into a single folder and inputting them into Orange, the software employs the Inception v3 architecture to automatically cluster the images based on default parameters, displaying the results on a grid.

<img src="/assets/images/assignment2_images/overview.jpg" style="zoom:25%;" />

Interestingly, Orange effectively differentiates between cats and dogs. Observing the grid, it's noticeable that cats predominantly occupy the left section, while dogs are grouped on the right.

### Hierarchical Clustering Exploration

To delve deeper into how Orange classifies these images, I utilized its "hierarchical clustering" feature. This function helps visualize the relationships and distinctions between grouped photos.

The initial layer of classification interestingly does not separate cats from dogs but instead prioritizes images based on the presence of light golden fur. As a result, the selected images predominantly feature light golden-haired cats. This dataset notably lacks dogs with similar fur coloration, explaining their absence.

<img src="/assets/images/assignment2_images/first_category.jpg" style="zoom:25%;" />

Advancing further into the clusters, specifically within the dog categories, it appears that Orange excels in facial recognition. Dogs with similar facial features are grouped together, indicating a sophisticated level of detail in the machine’s analytical capabilities.

<img src="/assets/images/assignment2_images/face_pattern.jpg" style="zoom:25%;" />

## Classification Performance

Subsequently, I organized the same image set into predefined folders by species for a controlled test. This setup allows Orange to independently scan and analyze each folder, comparing its findings with the pre-assigned classifications.

###Classifying Breed

The machine is not doing well in classfiying breeds because it considers color more than breeds. 

### Confusion Matrix and Testing Accuracy

*Confusion Matrix*
<img src="/assets/images/assignment2_images/confusian_matrix.jpg" style="zoom:25%;" />

*Test Score*
<img src="/assets/images/assignment2_images/confusian_matrix.jpg" style="zoom:25%;" />

The confusion matrix and testing scores reveal that Orange performs exceptionally well in distinguishing between cats and dogs. It boasts a 100% accuracy rate, matching the classifications indicated by the folder labels. This experiment highlights the effectiveness of machine learning in recognizing and differentiating between animal species based on visual data.

## Algorithm Prediction

From this set of pictures, I think it is obvious that machine classifies the photos well, and is able to somehow recognize faces depend on the patterns and colors on the faces. However, I do think that classifiying cats and dogs are too easy for the machine because it must have been trained through significant amount of similiar data.









