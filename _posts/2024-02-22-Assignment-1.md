---
title: "Assignment 1 - Cultural Heritage by the Numbers "
last_modified_at: 2024-02-27 T16:20:02-05:00
categories:
  - Blog
tags:
  - Post Formats
  - readability
  - standard
toc: true
toc_sticky: true
toc_label: "Blog Parts"
toc_icon: "calendar"
---

When we look into the marvellous pieces in the museums, do you see the "tags" behind? Cultural Heritage has a myriad of labels behind it. Although these labels cannot replace the meaning and value of Cultural Heritage itself, they show us the connection of the artifacts. This project focuses on analyzing the textual descriptions of Cultural Heritage, analyzing the number of keyword occurrences and visualizing them with wordcloud, in order to find the similarities and differences between different cultures.

## Part 1 - From the Webpage and CSV File

The [Harvard Art Museums website](https://harvardartmuseums.org) has an aesthetically pleasing design. However, I don't think it does a good job of guiding non-specialists through the process of exploring and learning about Cultural Heritage because the site doesn't do a great job of proactively recommending exhibits that, for the most part, one would need to search for on their own to explore. Of course, the filter function of the website is good to stimulate people's desire to explore. It puts filters on some of the dimensions so that we can limit out the scope of what we want and thus focus more on wanting to understand the parts. However, until one clicks through to a specific presentation of an artifact, all of the artifacts in the site are presented in an image arrangement, which makes it difficult to see a complete overview, and instead focuses more on each individual.

##### A general layout after setting a filter 'Chinese'
<img src="/assets/images/assignment_1/webpage.jpg" style="zoom:25%;" />

##### The layout after clicking into one of the artifacts
<img src="/assets/images/assignment_1/artifact_introduction.jpg" style="zoom:25%;" />

It is also hard to grasp the general idea of the cultural heritages in a certain period of time, culture, location, or any other categories in the filters just from the csv. file because all of them are listed individually and the file is too big for human to directly retrieve information from it.

## Part 2 - Biases In Museums

From the csv. file that gives all information about cultures included in the artifacts in the Harvard Arts Museum, I find some interesting patterns. 

The first is that the museum preserves a lot of artifacts from the "typical cultures" and cultures experienced the Renaissance. For example, we can see that there are more than 1000 collections in cultures like Chinese, Japanese, European, Egyptian, byzantine and American. However, it does not pay equal attention to minor cultures like Lebanese, Turkistan, South Asian, African and so on. In addition to that, some categories are repetitive. For example, it has the category of Chinese, Japanese, Korean, and it also has a category called "East Asian", which should contain the three culture above. This shows that there might be a bias 

For example, I use the API Categorical Scrapping program to sort out all the objects in "Chinese" cultures in 20th century. The statistical result of first page information shows that one of the artifact is viewed significantly more than the rest. The possible explanation is that this artifact is on display in the museum more often than the rest of the others.

<img src="/assets/images/assignment_1/Chinese.jpg" style="zoom:25%;" />

## Part 3 - Visualized Analytics

Word cloud is a statistical graph to visually show the word frequencies in a range of texts. It can help readers to find the key features or central ideas of a text just by grasping the word cloud.

I use the word cloud to look into the features of certain cultures and see if there is any connections. From the Harvard Arts Museum, I picked "Chinese","Japanese" and "Korean" out of all the cultures. 

The program first sort out all the artifacts belong to these cultures. From the result, we can see that the the three culture has a significant higher number of pieces of artifacts compared to the average. Japanese and Chinese artifacts are more collected than Korean. And from the statistical graph we can see that the accession number for Japanese works is high in 1933, and for Chinese works it is 1943. This might be explained with historical reasons. Japan was in the World War II during 19030s and the world started to pay more attention to this culture. China was in the Second Sino-Japanese War (1937-1945) during 1943, which might show that the army left China might take away the artifacts as well.

<img src="/assets/images/assignment_1/object_culture.jpg" style="zoom:75%;" />

<img src="/assets/images/assignment_1/newplot.jpg" style="zoom:100%;" />

### Word Cloud

Apart from comparing general images of the background of the artifacts in each culture, I use the word cloud to look into the key feature of the cultures one by one. I set stopwords to exclude the functional words, numbers, or words that are meaningless. I set single color for each image generated because I think the size of the words are enough to explain the frequency, adding colors might make it chaotic. Below I will explain more details about each word cloud generated.

The first word cloud shows the most frequent words that are used to describe Chinese artifacts. The most frequent word is "Decoration", which might indicate that most of the Chinese artifacts collected in HAM are for decorational purpose. The words "Bowl","Vessel" and "Jar" also appears frequently, which might show that a large portion of the collections are utensils. From these findings, we can further guess that Chinese culture cares about the aesthetics of dining because "decoration" appears together with utensils.

<img src="/assets/images/assignment_1/Chinese_words.jpg" style="zoom:100%;" />

The second word cloud shows the most frequent words in Japanese artifacts. "Series" is the top frequent word among all of the words, and is followed by words like "Poem","Tale","View" and "Chapter". This might suggest that there is a large amount of text or image works which can explain ideas and even series of ideas. From this we can possibly say that Japanese care about the art of language and are keen on expressing ideas.

<img src="/assets/images/assignment_1/japanese.jpg" style="zoom:110%;" />

The third word cloud shows the most frequent words in Korean artifacts. "Sherd" and "fragment" are two words that appeared often. Together looking at century-specific statistics for Korean artifacts, we can possibly conclude that the artifacts are too old to be well preserved compared to artifacts from the other two cultures.

<img src="/assets/images/assignment_1/Korean.jpg" style="zoom:110%;" />

<img src="/assets/images/assignment_1/century.jpg" style="zoom:110%;" />

Apart from the individual features of each culture, we definitely see some common patterns among the three east asian cultures. All of the three word clouds contain "decoration", which might suggest that the importance of aesthetics in the east asia. And from this, we can further generate that there should be at least some parts of the countries are wealthy enough to afford buying or making decorational objects. Plants seem to have some significance in East Asian culture as well. Both Japanese and Korean word clouds contain "flower" or "floral, while Chinese also contains "bamboo" and "leaves".

## Conclusion

By using the word cloud and other statistical programs, we have a whole new perspective when it comes to museums and artifacts. Unlike the one-by-one reading comprehension that humans are used to, computers can help us quickly grab information, allowing us to categorize information as a whole and find the characteristics of different categories of information. Thus, we can catch some of the main ideas while not taking the time to look at specific items one by one. And we can look at more specific features by continually narrowing down the scope.

