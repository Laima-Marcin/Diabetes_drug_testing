# Diabetes_drug_testing
Patient Selection for Diabetes Drug Testing

EHR data is becoming a key source of real-world evidence (RWE) for the pharmaceutical industry and regulators to make decisions on clinical trials. 

OUR PROJECT:

Unicorn Healthcare startup company has created a groundbreaking diabetes drug that is ready for clinical trial testing. It is a very unique and sensitive drug that requires administering the drug over at least 5-7 days of time in the hospital with frequent monitoring/testing and patient medication adherence training with a mobile application. 
For this project we have been provided a patient dataset from a client partner and we were tasked with building a predictive model that can identify which type of patients the company should focus their efforts testing this drug on. Target patients are people that are likely to be in the hospital for this duration of time and will not incur significant additional costs for administering this drug to the patient and monitoring.

In order to achieve our goal we must first build a **regression model** that can predict the estimated hospitalization time for a patient and also provide an uncertainty estimate range for that prediction so that we can rank the predictions based off of the uncertainty range.

*Expected Hospitalization Time Regression and Uncertainty Estimation Model*: Utilizing a synthetic dataset(upsampled, denormalized, with line level augmentation) built off of the UCI Diabetes readmission dataset, we have built a regression model that predicts the expected days of hospitalization time and an uncertainty range estimation.

This project demonstrates the importance of building the right data representation at the encounter level, with appropriate filtering and preprocessing/feature engineering of key medical code sets. In this project we analyzed and interpreted our model for biases across key demographic groups. 
Lastly, we utilized the TF probability library to provide uncertainty range estimates in the regression output predictions to prioritize and triage prediction uncertainty levels.

In the end we created a demographic bias analysis to detect if our model has any bias which we know can be a huge issue in working with healthcare data!
