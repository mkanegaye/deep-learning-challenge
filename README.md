**Deep Learning Challenge Report**

**Overview:**
The purpose of this analysis was to create a tool that can help the nonprofit foundation Alphabet Soup to select the applicants to fund that have the best chance of success. Using the provided dataset, we created a binary classifiier that can predict the success of applicants.

**Results:**

Data Preprocessing
* "IS_SUCCESSFUL" was the target variable for the model
* Features for the model include the following variables: application type, affiliiation (affiliated sector of industry), classification (government organization classification), use case (for funding), organization type, status, income amount classification, any special considerations, and the ask amount (i.e., the funding amount requested)
* The EIN andd Name variables were removed from the input data because they were neither targets nor features
  
Compiling, Training, and Evaluating the Model
* In my attempts I selected the following specifications for my nueral network model, which resulted in the listed accuracies:
    *Model Attempt 1
2 layers:
layer1_nodes = 10
layer2_nodes = 8
Accuracy: 0.728

  *Model Attempt 2
4 layers
layer1_nodes = 40
layer2_nodes = 30
layer3_nodess = 20
layer4_nodes = 10
Accuracy: 0.727

  *Model Attempt 3
3 layers
layer1_nodes = 80
layer2_nodes = 50
layer3_nodes = 30
Accuracy: 0.728

*In my first attempt I utlized an amount of layers and nodes which we had used in class activities. As that attempt did not yield the desired 75% accuracy, I then chose to increase both the number of layers and the nodes within, which resulted in 72% accuracy, again below the target. For my third and final attempt I chose to see what would happen if I decreased the number of layers by one, but increased the number of nodes by a decent amount. This attempt did marginally better than Attempt 2, but still resulted in ~72% accuracy.

**Summary: **
None of my 3 attempts of optimizing the model provided the desired result of at least 75% accuracy. A different classifer, like a random forest, could provide improved results. A random forest will implement many decision trees to come to a classification.
