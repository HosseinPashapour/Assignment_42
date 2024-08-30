# Assignment 42
# Machine learning

# ANSUR II dataset


This project demonstrates the implementation and evaluation of the K-Nearest Neighbors (KNN) algorithm on a combined dataset of male and female measurements. The process includes preprocessing the dataset, splitting it into training and testing sets, evaluating the KNN algorithm with different values of `k`, and calculating the confusion matrix for the test dataset.

## Steps

1. **Preprocess Dataset**
   - Convert the unit of weight from pounds to kilograms.
   - Convert the unit of height from inches to centimeters.
   - Convert the datatype of gender from categorical to numerical.

## Show heights for women and men on same plot.

<img src="Output\Women & Men.png" width="550">

- ## A. Why is the data of men higher than the data of women?

  + Because there are more male data than female data (because 1985 females and 4081 males).

- ## B. Why is the data of men more right than the data of women?

  + Because men are taller.
  For a better comparison, the following chart with the same density is proposed.


## The Stature f Women and Men:

<img src="Output\Stature.png" width="550">


## Answer :

     Mean of Women height = 162.84 cm
     Mean of Men height = 175.62 cm

2. **Split Dataset**
   - Split the dataset into training and testing sets with 80% for training and 20% for testing.


### Split dataset to train and test (%80 for train and %20 for test):
- Size of training set: 4854
- Size of testing set: 1214

3. **Evaluate KNN Algorithm**
   - Evaluate the KNN algorithm on the test dataset with different values of `k = 3, 5, 7, 9, 11`.
   - The table below shows the accuracy for each value of `k`.

<img src="Output\Confusion Matix for knn.png" width="550">

   | k  | Accuracy of ``object oriented KNN algorithm`` (%) | 
   |----|--------------|
   | 3  |  [88] |
   | 5  |  [90] |
   | 7  |  [90] |
   | 9  |  [90] |
   | 11  |  [91] |


4. **Calculate Confusion Matrix**
   - Calculate the confusion matrix for the test dataset.

5. **KNN Implementation using Scikit-Learn**
   - Perform the above steps using the Scikit-Learn library to ensure correctness and compare results.
   - The table below shows the accuracy for each value of `k`.

   <img src="Output\Confusion Matix for Sklearn.png" width="550">

   | k  | Accuracy of ``scikit-learn KNN algorithm`` (%) | 
   |----|--------------|
   | 3  |  [87] |
   | 5  |  [89] |
   | 7  |  [90] |
   | 9  |  [90] |
   | 11  |  [91] |

## Results

## Accuracy for two algorithm: Myknn and sklearn


<img src="Output\Accuracy_KNN.png" width="550"> 


## How to Install
Run following commend :
```
pip install -r requirments.txt
```

## How to Run
```
Run KNN_Ansur.ipynb file in jupyter notebook
```




