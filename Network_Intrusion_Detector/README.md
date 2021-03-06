# group-project-group-f
group-project-group-f created by GitHub Classroom

Team Members:

Rifat Ahmed Khan - 45847827
Tahsina Tamanna - 45710449
Cal Vin Khor - 44551401

Project on Network Intrusion Detection

Tasks Performed:

1) The datasets downloaded were huge and more than 100MB each. Thus they had to be compressed in order to be uploaded to GitHub.
2) In order to run the code, the compressed files need to be extracted first. 
3) The final dataset was created by combining the 4 datasets into a single .csv file using code in the python file.
4) The NUSW-NB15_features.csv file contains the names of the features and were used for the column names in the final dataset.
5) After the dataset was complete, it was checked for null values and filled with appropriate values.
6) Empty spaces in the 'ct_ftp_cmd' column were found and removed as the research paper of the data listed it as a numerical feature.
7) Further cross-checking were performed.
8) The binary columns containing values more than 1 were changed to 1.
9) '-' values found in 'service' column were changed to 'None'.
10) 'backdoors' values in 'attack_cat' column were change to 'backdoor' to remove redundancy.
11) Feature selection was performed by finding out the correlation between the features. The columns with correlation more than 0.95 were dropped to reduce redundancy.
12) Categorical Encoding was performed to convert the text data ('proto', 'state', 'service' columns) to numerical data.
14) The label encoding were changed so that +1 would mean normal data and -1 would represent attack data.
15) The dataset was then split into features and labels and the features were standardized so that all columns would contain values between 0 and 1.
16) The dataset was then split into testing and training sets. 30% of the whole dataset was set aside for testing.
17) 4 different classifers were vuilt and the data was tested on each of them and their performance metrics were calculated and recorded to determine the best performing classifier for NIDS.
18) The classifiers used were- Decision Tree, Logistic Regression, Gaussian Naive Bayes and Random Forest.
19) Anomaly detection was performed on the dataset by two different methods, Isolation Forest and Local Outlier Factor. 
20) Hyperparameter tuning of the algorithms for anomaly detection were performed and represented usng graphs. Their perfromance metrics were measured and recorded.
21) Finally the research task was added to the python notebook as a requirement for the second task of the group project.