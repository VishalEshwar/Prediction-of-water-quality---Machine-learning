To predict water quality according to the classes defined by the Tamil Nadu Pollution Control Board (TNPCB) using 21 parameters.Here I have used supervised machine learning models such as logistic regression or a decision tree-based algorithm and Random forest.
Here's an overview of the steps involved:
1) Data Collection
2) Data Preprocessing
3) Split the Data
4) multi class classification
5) Model Evaluation
6) Conclusion
1) Data Collection: Obtained the dataset from the TNPCB website for the year 2018.The raw data consits of 26 water quality paramters with 12 sampling areas acrosss the Thamirabarani river.

2) Data Preprocessing:
•	The parameters which contained the missing values and the areas in which the samplings are not done were eliminated. Hence the preprocessed data contains about 21 parameters.
•	The missing values were handled
•	The label encoding was performed for the DBU (Designated Best Use) classes,using the LabelEncoder function provided by the scikit-learn library.
•	A - Drinking Water Source without conventional treatment but after disinfection
•	B - Outdoor bathing (organised)
•	C - Drinking water source after conventional treatment and disinfection
•	D- Propagation of wild life and fisheries
•	E -Irrigation, Industrial cooling,controlled waste disposal
•	Below  E Not meeting A,B,C,D & E Criteria

•	Z-score was performed to normalize the feature values.
•	The preprocessed paramters was visualized using .head(), .describe() and .info() functions.
•	Scatterplot is visualized to know about the PH and Conductivity of the data
•	Pairplot is visualized to know about the 4 following paramters subset = ['PH', 'conductivity', 'BOD', 'class']

3) Split the Data
In this problem statement the data is Splited as follows, 80% Training and 20% Testing.

4)Multi class classification
 For the parameters machine learning algorithms were performed to get result for multiclass classification
Logistic regression, Decision Tree and Random forest were performed.

5) Model evaluation:
The above mentioned ML algorithms were evaluated using the following performance metrices.
Precision, recall , f1 score, accuracy.

6) Conclusion:
With this ML model we come to the conclusion that the water quality has been predicted with the accuracy of about 93%.
