# MNISTClassification
This repository displays the usage of Decision Trees, Random Forests, Neural Networks, and Convolutional Neural Network.

Hello! 
This is my MNISTClassification project!

To start out, I had created a few cells to get a feel for the data I was working with. I had to preprocess some of the data to make sure it all fit in smoothly, and then I got right into the models.

For the Decision Tree model, I had wanted to create a baseline using the most intuitive, human form of decision making: everything less than a value goes to the left, everything greater goes to the right. This process branches out with different features and corresponding values that best split the data until the leaves have nearly perfect predictions where, say every O shape without a belt is a 0, and with a belt is an 8 (this is of course abstracted for the example). Using this method, I was able to obtain an accurate classification of the 10,000 test samples about 87% of the time. 

Random Forest is known to be a booster for Decision Trees, so I wanted to showcase how using multiple decision trees and pooling their votes could help reduce variance and mitigate any outliers one randomly generated decision tree might have had. This worked very well with the MNIST dataset, as the accuracy increased to about 90%, and it also backfired in the personally handwritten data. This is because when the individual decision trees are not very good at classification (as they would be with unvalidated data), pooling their votes together dramatizes the effect as now the misclassifications are more popular than the correct votes. This is what yielded the low accuracies for a solo decision tree (48%) and even lower for Random Forests (28%). 

Now that we've established our baseline Decision Trees, as well as highlighted the boosting and potentially harmful effects of the Random Forest, I wanted to dive into the Neural Networks. These are much less intuitive, with heavily interconnected layers of nodes representing logistic regression functions that use hundreds and thousands of weights and biases to optimize decisions with astounding results.

The Neural Network (NN), which only consisted of four layers of nodes, yielded an incredibly high 98% accuracy on the test data in the handwritten digits, and also performed very well (though this file showed a lower accuracy than usual) on the personally written digits.

The Convolutional Neural Network(CNN), which admittedly was geared specifically for image processing, was designed similarly to the NN, however with the added Convolutional layer. I had also plotted some characteristics of these networks to try to break down some of the numbers into more digestible values. These accuracies of 98.8% and 94% show a very optimal neural network for classification.

Prior to this project, I had very little experience with Neural Networks in general, and I had spent many hours determined to create working and thriving models to handle this massive set of data in a very computationally reasonable time. This project shows how even with concepts that are very complex and hard to understand at first, I was able to educate myself to get through the tasks at hand.
