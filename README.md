# Machine-Learning-in-Health-Care

  Causal inferences are used to draw causal (cause and effect) conclusions from data. They have applications in different fields from economics to health care. 

This project has two parts. The first part is testing SuperLearner framework which is a flexible ensemble of machine learning models. The second part is using SuperLearner to develop a doubly robust method for estimation of causal parameters called TMLE (Targeted Maximum Likelihood Estimation). We tested TMLE on different datasets and compared the results with traditional methods.

## Super (Machine) Learning  
The super learner provides a flexible but robust procedure for estimating an ensemble prediction model. By incorporating a rich collection of algorithms that vary in bias and degree of data-fitting, the cross-validation within the super learning prevents overfitting and it also prevents selecting a fit that is too biased. 

![image](https://github.com/user-attachments/assets/990de748-3733-43c7-a77f-62585d80ea7f)

## Simulation

To test the performance of super learner we did a simulation on four different types of functions defined by

<img width="760" height="720" alt="image" src="https://github.com/user-attachments/assets/9dd7976c-3e4b-480b-986e-b76a3bdbec14" />

### Set of Algorithms for Super Learner
The set of algorithms in the collection should be a diverse set to adapt to different types of data generating models. Here we have regression, regression trees, random forest and neural networks.

<img width="660" height="435" alt="image" src="https://github.com/user-attachments/assets/dc3688b4-2de2-4cfe-ac31-fad094a2ac31" />

### Results

For each simulation we produced a scatterplot. The true curve for the simulation is represented by the solid black line. The red dots represent the simulated data and blue dots represent the predictions from super learner fit. With the given collection of algorithms (except for simulation 4 which requires additional algorithms), the super learner is able to adapt to the underlying structure of the data-generating function and has a risk close to the best algorithm.

In summary, The super learner provides a flexible but robust procedure for estimating an ensemble prediction model. It allows the researcher to evaluate a large library of prediction algorithms, but controls over-fitting with cross-validation. 

<img width="960" height="720" alt="test" src="https://github.com/user-attachments/assets/e5c5149b-b569-4e20-8052-cfa06a75d70f" />

## TMLE method for Causal Inferences
Targeted Learning integrates causal inference, machine learning and statistical theory. TMLE provides doubly robust estimation for complex observations, particularly high dimensional data. The estimate is accompanied with confidence interval and p-value.

![image](https://github.com/user-attachments/assets/2c39dd32-c069-4d7a-bf41-1dc0ceee1971)



