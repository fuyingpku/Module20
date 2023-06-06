# Capstone Project: Final Report and Exploratory Data Analysis (EDA)
Github code:https://github.com/fuyingpku/Module20.git
### Overview of technology in this project:
(1) Project Organization · README file with a summary of findings and link to your Jupyter Notebook · Jupyter Notebook with headings and text appropriately formatted · Libraries are imported and aliased correctly · Code does not contain errors · No long strings of code output · Demonstrates competency with pandas · Demonstrates competency with seaborn · Variables are sensible

(2) Syntax and Code Quality · Libraries are imported and aliased correctly · Code does not contain errors · No long strings of code output · Demonstrates competency with pandas · Demonstrates competency with seaborn · Variables are sensible

(3) This criterion is linked to a Learning OutcomeVisualizations · Appropriate plots for categorical and continuous variables are utilized

(4) This criterion is linked to a Learning OutcomeModeling · Use of multiple regression or classification models Cross-validation of models · Grid Search hyperparameters

### Business Understanding
(1) Business Objectives: The research question you intend to answer (one sentence, if possible): Identification of key factors for HCC patent survival

(2) Background: the expected data source(s) (either a link to existing data or a sentence describing where you will source the data from): https://archive.ics.uci.edu/ml/datasets/HCC%2BSurvival (Links to an external site.)

(3) Business Success Criteria: The techniques you expect to use in your analysis: K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines

(4) The expected results: Identification of key factors for HCC patent survival Why this question is important: It is a very important prediction for patients and their family, it paves the biomarker method to identify patients who should explore or benefit investigational new drugs by FDA.
We will make use of the article accompanying the dataset here for more information on the data and features.

### Assess Situation
(1) Inventory of Resources: class chat and with mentor 1 on 1 meetings, python and modeling, and other previous trainings in this course.

(2) Requirements, Assumptions, and Constraints: this is a practice work due by the end of the course, no legal issue with data usage. The assumptions are good data collection in the public database. Due to the limiation of CPU power, a relatively small dateset was used.

(3) Risks and Contingencies terminology: The success may rely on good analysis skillset of the performer in this case.

(4) Costs and Benefits: It is a good business model which could be used for not only HCC but also other cancer types

### Determine Data Mining Goals
（1） Data Mining Goals：Predict the HCC patient survial based on their conditions and find the correlations between different features and surival status.

（2） Data Mining Success Criteria：plot the figure to cover all the features in the HCC dataset.

### Produce Project Plan
（1） Project Plan：the CRISP-DM standard protocol will be carried out, in total, 16 hrs for data understanding/preparation/modeling/evaluation/deployment

（2） Initial Assessment of Tools and Techniques：compare the performance of the Logistic Regression model to our KNN algorithm, Decision Tree, and SVM model and provide the best sample and best hyperparameters through Grid search.

### Evaluation
With some modeling accomplished, we aim to reflect on what we identify as a high quality model and what we are able to learn from this. We should review our business objective and explore how well we can provide meaningful insight on HCC patient status. 

We understand the challenges is that due to the limitation of avaiablity of the HCC patients, the dataset is only a small cohort, but we want to test the hypothesis to see how powerful the tool could be made or we can achieve in this case

Future directions: Ai based model could do a much better job than SVM which is the chosen best model in this analysis. 

Access of data mining results with respect to business success creteria:
In principle, a business is based on the consistency of the model, which is shown not overfitting in this case (Train accuracy at 0.64, test accuracy at 0.71), the model(s) build here provided the inital analysis of the price which address the business quesiton of predicting the HCC patient surviaval status with a limited input of small data base.

Business Objectives: The goal is build the model to predict the HCC patient survival status. Several groups of features were used and different hyperparameters were explored to optimize the model to achieve a test accuray at 0.71. 

Business Success Criteria is met: As a result of this model based analysis, the model should provide clear recommendations to the doctor who is evaluating the HCC patients status. In this case, highly relevant featuers were found: 'Alcohol', 'Cirrhosis : nominal', 'Hepatitis B Surface Antigen', 'Arterial Hypertension', 'Hepatitis C Virus Antibody', 'Smoking', 'Alanine transaminase ', 'Number of Nodules', 'Age at diagnosis'.

With this model, it is feasbile to put in any future features and give predicted status of the HCC patients. We can further use this program to train and obtain different models for different types of cancer. 

Review process: in summary, the whole process start with a small panel then overview of all the features in the dataset, remove outliers and Nan values, using graphic and correlation function to identify what are the key factors contribute/correlate the survival status of HCC patients. During the analysis, it is noticed the although the model and maker also could contribute a lot of the status of the HCC patients, it is feasible that improved accurary could be achieved/built with a much larger dataset. We used the correct attributes with correct model, but we admit there is still room to improve the result with a much larger dataset. 

Determing the next step: with the model built, we can suggest a deployment and give it a pressure test first.

### Deployment
Plan deployment: it is a general procedure used to identify and create the model in this case. all the parameters were fixed for any repeat analysis needed. The model itself is ready for deployment and for sure training and interface could be employed by the customers

Produce final report: In this project, we screened all the features, based on the avaiablity of the dataset, we narrow down factors: 'Alcohol', 'Cirrhosis : nominal', 'Hepatitis B Surface Antigen', 'Arterial Hypertension', 'Hepatitis C Virus Antibody', 'Smoking', 'Alanine transaminase ', 'Number of Nodules', 'Age at diagnosis'.

There are four techniques used in the analysis are K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines (SVM). In the end, SVM showed the best accuray. We also observed that Decision Trees tend to give the most overfitting in this case.

Review project: The initial analysis and data prep went well. However, the model (including all the four models and with new features and new hyperparameters) gives only accuracy at approximately 0.7, with a small database with less than 200 patients. That could be improved with better model e.g. AI based model and larger dataset with more features could be selected. A group discussion could be beneficial across the class and brainstorm an alternative strategy with deep learning as well.

​
