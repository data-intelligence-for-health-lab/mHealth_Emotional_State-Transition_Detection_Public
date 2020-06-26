# mHealth_Emotion_detection

Summary of the project: The main objective of this project is to study the feasibility of detecting emotional states and transitions in small intervals leveraging machine learning algorithms applied and contextual data acquired by smartphone and wearable sensors. Our study includes all three dimensions of emotional states (pleasure, arousal, and dominance) and the variability of interpersonal data as well. 

Dataset: Download the dataset from	http://extrasensory.ucsd.edu/
Dataset reference: Vaizman, Y., Ellis, K., and Lanckriet, G. "Recognizing Detailed Human Context In-the-Wild from Smartphones and Smartwatches". IEEE Pervasive Computing, vol. 16, no. 4, October-December 2017, pp. 62-74. doi:10.1109/MPRV.2017.3971131

Python codes: This repository contains 11 Jupyter notebook files for data processing, hyperparameter tuning, machine learning, and imbalance handling. All intermediate and processed data are included in the 'data' folder. ALl codes are written in python using scikitlearn, imblearn, xgboost, and catboost libraries. 

Notation: D1-D7: Data preparation, ES.General and ES.Indiv: Emotional state detection and imbalance handling using ML algorithms, and ET.General and ET.Indiv: Emotional transition detection and imbalance handling using ML algorithms.

Steps to run the project succesfully
1. Download the following datasets from	http://extrasensory.ucsd.edu/
  a. Primary data - features and labels
  b. Mood labels
  c. Absolute location coordinates
2. Unzip data and store them in 'data' folder or in your desired directory
3. Run files D1-D7 to read, merge, preprocess, and re-sample data 
4. Run files ES.General and ES.Indiv to tune hyperparameters (GridSearch) of ML algorithms for emotional state detection. This includes running the models with the best parameters for each classifier with an optional step of using imbalance handling techniques: SMOTE and SVMSMOTE
5. Run files ET.General and ET.Indiv to tune hyperparameters (GridSearch) of ML algorithms for emotional transition detection. This includes running the models with the best parameters for each classifier with an optional step of using imbalance handling techniques: SMOTE and SVMSMOTE
