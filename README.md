# Neural_Network_Charity_Analysis

## Overview
Using Tensorflow to experiment with Deep Learning - specifically when applied to binary classification.

## Results

### Data Preprocessing
**- What variable is considered the target for your model?** IS_SUCCESSFUL - We are attemping to predict how likely a charity project is to succeed.  

**- What variables are considered to be the features for your model?** Everything except for IS_SUCCESSFUL, EIN, and NAME columns.

**- What variables are neither targets nor features, and should be removed from the input data?** EIN and NAME columns.  


### Compling, Training, and Evaluating the Model
**- How many neurons, layers, and activation functions did you select for your neural network model, and why?** I chose to take the number of inputs (38) and triple it amongst three hidden layers for a total of 114 neurons. For activation layers they were assigned in the following order relu -> sigmoid -> relu -> sigmoid. This was finalized this way as even with experimenting with all sorts of different combinations of activation layers the accuracy would not improve past 74%.  

**- Were you able to achieve the target model performance?** No, the final results after attempting more than 3 times was an accuracy score of 72.5%.  

**- What steps did you take to try and increase model performance?** First, I attempted just increasing the number of neurons in the existing two hidden layers. Second, I increased the number of hidden layers to 3 and had a descending number of neurons in each layer. Third, I attempted to bin the data in a more general manner to reduce the spread of the data. After this I generally experiemented with changing activation methods, loss methods, and the number of neurons in each hidden layer before concluding on the above.  



## Summary
Overall the results of this deep learning model resulted in a final accuracy of approximately 72.5%. If I were to keep working on this problem I would take a deeper dive into finding a better way to preprocess the data going into the model. If we were to use machine learing with a different model altogether I would choose to use a logistic regression, as it works well with binary classification.
