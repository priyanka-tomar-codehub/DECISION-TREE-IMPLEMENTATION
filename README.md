# DECISION-TREE-IMPLEMENTATION
*COMPANY*:CODTECH IT SOLUTIONS
*NAME*:PRIYANKA TOMAR
*INTERN ID*:CT04DY481
*DOMAIN*:MACHINE LEARNING
*DURATION*:4 WEEKS
*MENTOR*:NEELA SANTOSH

##Description of the Task: Decision Tree Implementation on the Iris Dataset

The task presented here involves the implementation of a Decision Tree Classifier on the well-known Iris dataset, a classic dataset widely used in machine learning and statistical modeling. The objective is to build a supervised learning model capable of classifying flowers into their respective species based on their physical measurements. This process includes several steps, namely loading the dataset, preprocessing, training and testing the model, evaluating its performance, and visualizing the results. Each step contributes to building a deeper understanding of how decision trees work and how they can be applied to real-world problems.

Dataset Overview

The Iris dataset, introduced by Ronald A. Fisher in 1936, is one of the most famous datasets in the machine learning community. It consists of 150 samples of iris flowers from three different species: Iris Setosa, Iris Versicolor, and Iris Virginica. Each flower is described by four features:

Sepal length (in cm)

Sepal width (in cm)

Petal length (in cm)

Petal width (in cm)

The target variable is the species, which makes this a multi-class classification problem with three classes. Because of its small size and clear structure, the dataset is often used for introductory demonstrations of classification algorithms.

Methodology and Implementation

The first step was loading the dataset into a Pandas DataFrame from a CSV file. After loading, the features (X) and the target variable (y) were separated. Features included the four flower measurements, and the target consisted of the species labels.

Next, the data was divided into training and testing subsets using an 80-20 split (or 70-30 in this case) via the train_test_split function. Splitting ensures that the model is trained on one portion of the data and evaluated on unseen data, thereby preventing overfitting and allowing us to gauge the model’s generalization ability.

A Decision Tree Classifier from the Scikit-learn library was then implemented. The decision tree algorithm works by recursively splitting the dataset into subsets based on feature values that provide the highest information gain (using criteria such as Gini Index or Entropy). In this implementation, the Gini Index was chosen as the splitting criterion, and the maximum depth of the tree was restricted to 3 for simplicity and interpretability. Restricting the depth helps in controlling overfitting while still maintaining good classification accuracy.

The model was trained on the training dataset, and predictions were made on the test dataset. Accuracy was calculated to measure the proportion of correctly classified instances. Additionally, a classification report was generated, showing precision, recall, and F1-score for each class, offering deeper insights into the performance of the classifier beyond simple accuracy.

Visualization and Performance Evaluation

To enhance understanding, the trained decision tree was visualized using plot_tree(). This graphical representation displays the splits at each node, the decision rules, and the classification outcomes at the leaves. Visualizations are one of the strongest aspects of decision trees, as they provide clear interpretability compared to many other black-box models.

Furthermore, a confusion matrix was computed and visualized with a heatmap. The confusion matrix gives a breakdown of true positives, false positives, false negatives, and true negatives for each class. For a multi-class problem like this, it shows how often samples of each species were correctly classified versus misclassified as another species. The heatmap visualization makes these results more intuitive and highlights areas where the classifier might need improvement.

Conclusion

The Decision Tree Classifier implemented on the Iris dataset achieved a good balance of accuracy and interpretability. It successfully classified the flowers based on their morphological features, demonstrating the power of decision trees as a simple yet effective classification tool. This task not only illustrated the practical steps involved in machine learning model development—such as data preprocessing, model training, evaluation, and visualization—but also emphasized the importance of interpretability in model selection. The Iris dataset remains an excellent starting point for beginners in machine learning, and decision trees provide a clear and insightful way of approaching classification problems.

#output
<img width="622" height="697" alt="Image" src="https://github.com/user-attachments/assets/1078a4a2-0d59-4f63-8cec-e0f0ea9c5fae" />


