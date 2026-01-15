# Assignment2: Sampling by Prabhsimrat Singh (102317135)
EXPLANATIONS:
1. First of all view the visualisation of the dataset in a clean way using YData-Profiling
2. From this see if the Dataset is imbalanced by viewing the count of each class in the target/Class feature
3. Split the dataset into train,test. We apply sampling on only train data because test data is meant to be unseen and also because we want to improve the accuracy by adding meaningful rows into the train data to make it balanced. So we improve our training data by doing sampling.
4. We use 5 sampling techniques: Random Over Sampling, Random Under Sampling,SMOTE,Tomek, NearMiss
5. We use 5 Models: Logistic Regression, KNN, Random Forest, Decision Tree, SVM
6. Tomek gives high accuracy in SVM,Logisitc and KNN beacuse it removes those data points of the 2 classes that lie close to each other. This helps to seperate the 2 classes better at the decision boundary by reducing the noise near the area where the 2 classes overlap
7. Under Sampler gives low accuracy because it removes too much information from the majority class that the model becomes underfitting
8. Nearmiss is also an undersampling technique that's why it also performs badly
9. Oversampling makes the dataset balanced sufficiently balanced. However it causes overfitting beacuse same rows are repeated multiple times for the minority class
10. SMOTE gives mixed results and this shows that it overfits the data lesser as comapred to oversampling. this means that SMOTE provides better generalization on the training data using synthetic data points.
