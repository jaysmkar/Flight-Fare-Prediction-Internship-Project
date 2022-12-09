
# Flight Fare Prediction Internship project

This README file gives you detailed description and the flow of the project.




## Problem Statement
Travelling through flights has become an integral part of today’s lifestyle as more and more people are opting for faster travelling options. The flight ticket prices increase or decrease every now and then depending on various factors like timing of the flights,
destination, and duration of flights various occasions such as vacations or festive season. Therefore, having some basic idea of the flight fares before planning the trip will surely help many people save money and time. The main goal is to predict the fares of the flights based on different factors available in the provided dataset.



## Dataset
This Dataset is openly available on kaggle
```bash
  https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh
```
## Tech Stack

**Programming Languages:** Python

**Libraries:** Numpy, Pandas, Matplotlib, Seaborn, Sklearn

**Frontend:** HTML

**Backend:** Flask

**Deployment:** Putty, Puttygen, WinSCP, AWS

**Tools:** VSCode, Jupyternotebook, Anaconda


## Data Preprocessing
It includes loading the dataset into the required format that .csv to the pandas dataframe, clearning the dataset into required format which includese the removal of missing values, one hot encoding, standard scaling of the model and some other techinques. This process is the very important process because it cleans the data which play a very important role in the model building process. More cleaner data you give to the model more the accuraccy of the model will be.
## Model Building
This is the regression problem statement so we have tried many regression ML algorithms like linear regression, support vector regressor and some of the others as well. We have found out that the Random Forest fits the best with an accuracy of 89.40% with the training dataset and 83.30% with the testing dateset. Based on this figures we have finalised Random Forest as the main model for this project.
## Pickling the model
After building the model we have to create the pickle file for this model because our machine will understand only and pickle file is the binary file. We have loaded the entire model into the pickle file for the prediction. The command used to convert the model into the binary file is as follows:
```bash
import pickle
file = open('flight_fare_prediction.pkl', 'wb')
pickle.dump(random_forest_regresor, file)
```
## Backend Flask Application
The backend of this entire project is written in the flask which is the micro-web framework written in python. It is used as an intermediater to send and recieve information to our main model form the HTML template.
## Frontend
The frontend of this application is written in the HTML which will be receving the information from the user.
## Deployment

This project is deployed on AWS which is the cloud platform by amazon.


```bash
Steps to deploy the application on AWS:
• Create an AWS account
• Create an EC2 instance
• Edit security group
• Download the keygen (.pem file)
• Download and install Putty and WinSCP
• Install packages on EC2 using putty
• Finally run app.py command

```

## Demo
http://ec2-3-133-86-150.us-east-2.compute.amazonaws.com:8080/

## Authors

- [@Jayesh Mandavkar](https://github.com/jaysmkar/Flight-Fare-Prediction-Internship-Project)


## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jayesh-mandavkar-746b2b207/)

