
# Bank Marketing Project

## Overview
This project is part of the Udacity Nanodegree programme. In this project, I trained my model using autoML in the Azure Studio for the Bank Marketing dataset. After that, I have used deployed the best model from the autoML run. For the best model, I enabled the application insights logging and I used swagger API to interact with the swagger instance using the HTTP GET and POST requests. Then, I used the endpoint.py file to interact with my consumed model in order to get some outputs. Finally, I used the python SDK to create/consume and publish the best model using the aml-pipelines-with-automated-machine-learning-step.ipynb.

## Architectural Diagram

The steps followed throughout this project are shown below in the Architectural Diagram. 
![Architectural Steps Diagram](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Architectural%20Steps%20Diagram.PNG?raw=True "Title")

## Key Steps

#Note: All the pictures can be found in this GIT repository Starter_files/Pictures. 
Step 1: I skipped this step as I used the Udacity Lab and as such I was not authorized to create a principal security.
Step 2: Pictures Step 2-1, 2-2, 2-3 are applicable for this step. In picture Step 2-1, it can be seen the registered dataset in AzureML studio which is the bank marketing dataset. The picture Step 2-2 show that the AutoML run is completed. Finally, picture 2-3 show the best model which is the Voting Ensemble. 
Step 3: Picture Step 3 show that the deployed best model was completed.
Step 4: Picture Step 4-1 show that the Application Insights are enabled and Step 4-2 show that the logs.py file is running and reports logs back.
Step 5: Picture Step 5 show that the API swagger localhost page for the consumed best autoML model.
Step 6: Picture Step 6 show the output from the run of the endpoint.py file. Benchmark was an optional step which I didnt complete.
Step 7: Pictures Step 7-1, 7-2, 7-3, 7-4, 7-5, 7-5b, 7-6 show the outputs from running the aml-pipelines-with-automated-machine-learning-step.ipynd notebook file. It is apparent that running through the cells of the jupyter notebook, I created/consumed and published the best model for the bank marketing dataset using AutoML with Python SDK. 

## Screen Recording

Recording is available in Box folder in the following link:
https://app.box.com/s/ppa7kiit05tmve9pry7mfdb39epwfcvq

 ![fd](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%202-1.PNG)
 
