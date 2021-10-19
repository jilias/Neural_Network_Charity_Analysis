# Neural_Network_Charity_Analysis
## Overview of the analysis
The purpose of the using the neuron model for analysis is to see if where the foundation should successful make investments.

## Results
#### Data Preprocessing
- The IS_SUCCESSFUL column of the provided dataset was considered the target for this model.
- The EIN and NAME columns were removed from the dataset when compiliing, evaluating, and training the model since they did not information that could help with classification
- Other columns were used as features for the machine model
- "CLASSIFICATION" and "APPLICATION_TYPE" columns had identifiable unique values. Anything else was placed as "other"

#### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
The first and second layer are as followed
~~~
hidden_nodes_layer1 =  80
hidden_nodes_layer2 = 30
~~~
But did not bode well and yield the following accuracy
![image](https://user-images.githubusercontent.com/82242081/137848604-5e64fc78-05c7-47a4-a0e3-6994c5d97c71.png)
The next attempt, the neurons increased to
~~~
hidden_nodes_layer1 =  100
hidden_nodes_layer2 = 40
~~~
which then yielded the following
![image](https://user-images.githubusercontent.com/82242081/137848715-eba0da45-4e71-41cb-82bb-a40478c7e9de.png)

The next attempt the neurons increased and an additonal layer was added to the following
~~~
hidden_nodes_layer1 =  100
hidden_nodes_layer2 = 40
hidden_nodes_layer3 = 20
~~~
which led to the follwing
![image](https://user-images.githubusercontent.com/82242081/137848845-89bc4d25-7f71-4449-a3df-e3d403b7352d.png)

The next attempt
~~~
hidden_nodes_layer1 =  80
hidden_nodes_layer2 = 50
~~~
The neurons remained similar, but the third layer was removed only to decrease the accuracy.
![image](https://user-images.githubusercontent.com/82242081/137848960-7925e572-427a-4a73-a7f2-c5682874ea0a.png)

## Summary
The model is currently facing issues with possibly overfitting. There are too many variables in the datasets that cause too much noise. It would be best in the future to drop some of the columns that may not be useful for the process.
