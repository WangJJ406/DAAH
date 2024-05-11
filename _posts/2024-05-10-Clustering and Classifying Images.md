
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
>
>(1)Turn on your iPhone and go to album. 
>(2)Find a picture of your lovely cat or dog.
>(3)Scroll up.
>
>Do you see that iPhone helps you to recognize the breed of your lovely pet? 
>Yes, Apple uses a large database with tons of pictures to train the machine to recognize different breeds of pets by comparing with the existing ones.


<img src="/assets/images/assignment2_images/1.png" style="zoom:60%;" />

## How do Machine Recognize Your your Pet? Using Machine Learning to Ditinguish Cats and Dogs


## Introduction and Database Used

To observe how Orange analyzes and categorizes images, I downloaded a collection of cat and dog photos from kaggle. With a pre-designed data analysis procedure in Orange, the photo set input can be categorized and shown in the form of a grid. From the grid, we can guess the parameters the machine use to sort the images out.
<img src="/assets/images/assignment2_images/procedure.jpg" style="zoom:25%;" />

## Clustering
### Grid

I combined all the cat and dog pictures in one folder and input into the Orange. Using the Inception v3, the Orange cluster the images by default parameters and show the result on grid. 

<img src="/assets/images/assignment2_images/overview.jpg" style="zoom:25%;" />

Surprisingly, Orange seems to do well in distinguishing cats from dogs. From the grid, we can see that cats are mainly on the left corner, and the rest are occupied by the dogs. 

### Hierachical Clustering
To see how Orange actually classifies the photos, there is a "hierachical clustering" function in it to allow us see the relationships between groups of photos.

In the picture below, I selected the first layer of category in the Hierachical Clustering. To my surprise, the first layer is not distinguishing cats and dogs, but to sort out the light golden hairs first. Therefore, we can see from the image viewer that the pictures sorted out are all golden hair cats. There are no dogs simply because this dataset does not include any light-golden hair dogs.

<img src="/assets/images/assignment2_images/first_category.jpg" style="zoom:25%;" />


Then, I tried to go deeper into the clusters. I selected a branch inside dogs. In this branch, it seems like the machine is doing well in facial recognition. The dogs who have this similar facial pattern are sorted out.

<img src="/assets/images/assignment2_images/face_pattern.jpg" style="zoom:25%;" />

## Classification

###















