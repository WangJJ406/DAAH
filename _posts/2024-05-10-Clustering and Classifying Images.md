
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
### Try This

(1)Turn on your iPhone and go to album. 
(2)Find a picture of your lovely cat or dog.
(3)Scroll up.

Do you see that iPhone helps you to recognize the breed of your lovely pet? 
Yes, Apple uses a large database with tons of pictures to train the machine to recognize different breeds of pets by comparing with the existing ones.
<img src="/assets/images/assignment2_images/dog.jpg" style="zoom:125%;" />
<img src="/assets/images/assignment2_images/cat.jpg" style="zoom:125%;" />

## How do Machine Recognize Your your Pet? Using Machine Learning to Ditinguish Cats and Dogs


## Introduction and Database Used

To observe how Orange analyzes and categorizes images, I downloaded a collection of cat and dog photos from kaggle. With a pre-designed data analysis procedure in Orange, the photo set input can be categorized and shown in the form of a grid. From the grid, we can guess the parameters the machine use to sort the images out.
<img src="/assets/images/assignment2_images/procedure.jpg" style="zoom:125%;" />

## Clustering
### Grid

I combined all the cat and dog pictures in one folder and input into the Orange. Using the Inception v3, the Orange cluster the images by default parameters and show the result on grid. 

<img src="/assets/images/assignment2_images/overview.jpg" style="zoom:125%;" />

Surprisingly, Orange seems to do well in distinguishing cats from dogs. From the grid, we can see that cats are mainly on the left corner, and the rest are occupied by the dogs. 

### Hierachical Clustering
To see how Orange actually classifies the photos, there is a "hierachical clustering" function in it to allow us see the relationships between groups of photos.

<img src="/assets/images/assignment2_images/first_category.jpg" style="zoom:125%;" />

In the picture above, I selected the first layer of category in the Hierachical Clustering. To my surprise, the first layer is not distinguishing cats and dogs, but to sort out the light golden hairs first. Therefore, we can see from the image viewer that the pictures sorted out are all golden hair cats. There are no dogs simply because this dataset seems to not include any light-golden hair dogs.



**Warning Notice:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. [Integer nec odio](#). Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet.
{: .notice--warning}

**Danger Notice:** Lorem ipsum dolor sit amet, [consectetur adipiscing](#) elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet.
{: .notice--danger}

**Success Notice:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at [nibh elementum](#) imperdiet.
{: .notice--success}

Want to wrap several paragraphs or other elements in a notice? Using Liquid to capture the content and then filter it with `markdownify` is a good way to go.

```html
{% raw %}{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}{{ notice-2 | markdownify }}{% endraw %}</div>
```

{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}

<div class="notice">
  {{ notice-2 | markdownify }}
</div>

Or you could skip the capture and stick with straight HTML.

```html
<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>
```

<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>