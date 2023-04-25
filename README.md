# _Lab Test 3 For Predictive Analytics_

# Naive Bayes Classifier and clustering using Zoo Animal Classification

# Objective of assignment
- [x] Download the Zoo dataset from Kaggle, [Zoo Animal Classification | Kaggle](https://www.kaggle.com/datasets/uciml/zoo-animal-classification/code)
- [x] Use Naïve Bayes Classifier to perform classification.
- [x] Generate the confusion matrix and report balanced accuracy
- [x] Perform K-means clustering and report the optimal number of clusters.
- [x] Draw the dendrogram using single and complete linkage methods using hierarchical clustering.

# About Dataset
The purpose for this dataset is to be able to predict the classification of the animals, based upon the variables. 
It is the perfect dataset for those who are new to learning Machine Learning.

## Data Description
This dataset consists of 101 animals from a zoo. 
There are 16 variables with various traits to describe the animals. 
The 7 Class Types are: Mammal, Bird, Reptile, Fish, Amphibian, Bug and Invertebrate

### zoo.csv

Attribute Information: (name of attribute and type of value domain)

- animal_name: Unique for each instance
- hair Boolean
- feathers Boolean
- eggs Boolean
- milk Boolean
- airborne Boolean
- aquatic Boolean
- predator Boolean
- toothed Boolean
- backbone Boolean
- breathes Boolean
- venomous Boolean
- fins Boolean
- legs Numeric (set of values: {0,2,4,5,6,8})
- tail Boolean
- domestic Boolean
- catsize Boolean
- class_type Numeric (integer values in range [1,7])

### class.csv

This csv describes the dataset

- Class_Number Numeric (integer values in range [1,7])
- Number_Of_Animal_Species_In_Class Numeric
- Class_Type character -- The actual word description of the class
- Animal_Names character -- The list of the animals that fall in the category of the class

## Naive Bayes Classifier
The performance metrics for the model were:

1. Accuracy: 0.95
The accuracy score of 0.95 means that the model is able to correctly classify 95% of the animals in the testing set. It is a measure of the overall performance of the model.

2. Precision: 0.78
Precision is a measure of how many of the animals that the model predicted to be in a particular class actually belong to that class. A precision score of 0.78 means that out of all the animals predicted to belong to a certain class, only 78% of them actually belong to that class.

3. Recall: 0.83
Recall is a measure of how many of the actual instances of a class the model is able to identify. A recall score of 0.83 means that the model is able to correctly identify 83% of the animals that actually belong to a particular class.

4. Balanced Accuracy: 0.83
Balanced accuracy is the average of recall obtained on each class. It is useful when there is an imbalance in the number of samples in each class. A balanced accuracy score of 0.83 indicates that the model performs well on both the majority and minority classes.

Overall, the high accuracy score of 0.95 suggests that the Naive Bayes classifier model performs well in classifying the animals in the zoo dataset. However, the precision score of 0.78 suggests that there may be some false positives, and the recall score of 0.83 suggests that there may be some false negatives.

## K-Means Clustering

  The elbow method is used to determine the optimal number of clusters for KMeans clustering by plotting the within-cluster sum of squares (WCSS) as a function of the number of clusters. The elbow point is the value of k where the decrease in WCSS starts to level off, indicating that the additional clusters do not explain much more of the variance in the data. In this case, the elbow point occurs at k=4, suggesting that four clusters may be the optimal number for this data.

  After determining the optimal number of clusters, we fit the KMeans clustering model with 4 clusters and visualize the results using dendrograms with single and complete linkage methods. The dendrograms show the hierarchy of clusters and their distances to each other. From the dendrograms, we can see that the animals in the dataset can be divided into four distinct groups.

## Contributing
Contributions are always welcome!

## Author
- [@Aman Kumar Tiwary](https://github.com/titaniumspy07)

## License
[MIT](https://choosealicense.com/licenses/mit/)
