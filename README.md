# deep-learning-challenge

### Overview of the analysis: Explain the purpose of this analysis.
The purpose of this activity was to predict if applicants will have the best success rate in their ventures if they are funded by Alphabet Soup. Our attempt was to create a deep learning machine using TensorFlow and Keras. They were used in the model to help predict the outcomes of the ventures through the accuracy and percision of the model.  

# Results
Results: Using bulleted lists and images to support your answers, address the following questions:

### Results of the optimized model

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/75f91d62-e88d-4cc3-acd4-b906d346310c)

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/852149dc-a174-4041-81c0-536d3e062ee6)

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/06040bf6-e97e-4d08-a85e-365029f18b00)


### Results of original model 

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/8d602c70-172e-46e0-a357-df17267a7cff)

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/ddf65bc2-7b88-4093-83ec-8d2f6840c48e)

![image](https://github.com/Artib03/deep-learning-challenge/assets/147446590/c7857e9e-3ec5-4b61-acad-0e3f7bbb70be)

# Data Preprocessing

What variable(s) are the target(s) for your model?
The target of my model is the column called IS_SUCCESSFUL because that was the best target to determine the the applicant's venture will be successful or not. 

What variable(s) are the features for your model?
The features of my model are all the columns of the dummies temporary dataframe except for the target which is the column IS_SUCCESSFUL. 

What variable(s) should be removed from the input data because they are neither targets nor features?
The cariables that should be removed from the input data should be AFFILIATION, CLASSIFICATION, USE_CASE, SPECIAL CONSIDERATIONS, ORGANIZATION (any column that is categorical). I believe these columns cannot help predict if the applicant's venture will be successifical and are more of identifiers for each APPLICATION_TYPE. 

### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

Were you able to achieve the target model performance?

What steps did you take in your attempts to increase model performance?

# Summary: 
---Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

The overall results of the deep learning model was an average accuracy rate of approximately 70% for both the original model and optimized model. When I tried optimizing my model, I tried different things 
before my third attempt such as using tanh and removing some more columns but I feel that a deep learning model would not be the most effective. I would recommend a supervised learning model or even make_blobs model because the answer we are looking for is a "yes" or "no" answer. We are looking for if the applicant will be successful or not so there is a target and desired output. Also there could be multiple factors that determine if the venture will be success or not, for instance in the csv we do not have data on the public opinion (if consumers would support the idea for the venture or not). So for that reason the accuracy of the model cannot be 100% and there is a pretty high percentage in losses (67% for the optimized one and 59% for the original). Also the training data created through pd.dummies seemed unfit to help predict the success of the ventures. 
