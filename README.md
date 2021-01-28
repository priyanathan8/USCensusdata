# USCensusdata

Executive Summary
 This report discusses the use of artificial neural network algorithms and Keras Classifier
in order to accurately predict whether an individual has an income over $50,000 per year
in the US. The first step involved understanding the given data by generating a series of
plots. Followed by, exploratory data analysis which was conducted to examine the
quantitative variables and assess their significance. The categorical data were
transformed into sets of dummy variables which created a binary variable representing
each of the possible categories. After the data was explored, pre-processed, and split
between training and validation sets using a 60%-40% proportion, it was used to fit the
neural network. The initial ANN was trained on 28 predictors and it was found that the
network could accurately predict the target variable around 85% of the time. Further, this
model was tweaked based on its performance on the validation set; the best model
included only the significant predictors which led to an increase in model accuracy to
around 86%, while the false positive rate was minimized (0.0893) which is deemed
important for the process of granting personal loans to individuals by assessing their
income levels.
Part One: Training Data Set
Data Preprocessing
 Due to the model definition, all input and output variables should be numeric values
from 0 to 1. Therefore, we converted all numeric variables using a min-max scaler, and
created dummy variables for all categorical variables.
Neural Network
 Using the quantitative and qualitative predictors, a sequential neural network was
developed to predict the income of individuals based upon their attributes. Shown in
figure below, is the network topology. The quantitative predictors (blue nodes) and
qualitative predictors (orange nodes) represent the input layer. Next, two hidden layers
were constructed with nodes, and finally an output layer contained a single node. The
connections between the various layers represented the weights, and as the model
reiterated through back-propagation, the weights were adjusted until they eventually
reached a global minimum; resulting in the lowest squared error between the predicted
output and actual (test/validation) output.
