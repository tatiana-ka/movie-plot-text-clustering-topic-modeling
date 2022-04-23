# Getting movie plot originality measure (clustering, topic modeling)
*This script is still work in progress.* 
The movie plot data is from http://www.cs.cmu.edu/~ark/personas/
Use this old data to have a proof of concept test. 
**Concept:** 
To test the relationship between movie plot creativity (originality) and movie success. After margin the files and cleaning the text, I play with clustering and topic modeling to get the measure of originality. The idea is that the more atypical (distant from center) is the movie plot within its cluster, the more original/creative it is. 
I explore a number of different approaches to get originality measure: using PCA for dimensionality reduction,  trying LDA, KMeans, Agglomerative clustering etc. (I tried BERTopic, Gaussian Mixtures, Bayesian Gaussian Mixtures, and a few other things but those were completely off, so I removed them from the script). 
I also tried to train the clustering on past years and predict the originality for the following year, so that originality of the "new" movie is not biased by historical movies. Meaning, Matrix was an original movie at it's time, but may be not so original after a few decades. 

The details what I am doing, why I am doing this and clear explanations on the natural text clustering problem approach will follow.
