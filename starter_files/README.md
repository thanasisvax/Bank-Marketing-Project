
# Bank Marketing Project

## Table of Contents

<ol>
<li>Overview</li>
<li>Architectural Diagram</li>
<li>Key Steps</li>
<li>Improvements</li>
</ol> 

## Overview
This project is part of the Udacity Nanodegree programme. In this project, I trained my model using autoML in the Azure Studio for the Bank Marketing dataset. After that, I have deployed the best model from the autoML run. For the best model, I enabled the application insights logging and I used swagger API to interact with the swagger instance using the HTTP GET and POST requests. By deploying the model in Azure Machine Learning as a web service creates a REST API endpoint. Then, I used the endpoint.py file to interact with the API endpoing for my consumed model in order to send some requests and get some responses from my model. Finally, I used the python SDK to create/consume and publish the best model using the aml-pipelines-with-automated-machine-learning-step.ipynb.

## Architectural Diagram

The steps followed throughout this project are shown below in the Architectural Diagram. 
![](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Architectural%20Steps%20Diagram.PNG)

## Key Steps

### Step 1: 
<p>I skipped this step as I used the Udacity Lab and as such I was not authorized to create a principal security.</p>

### Step 2:

In picture Step 2-1 it can be seen the registered dataset in AzureML studio which is the bank marketing dataset.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%202-1.PNG)</p>


The picture Step 2-2 show that the AutoML run is completed.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%202-2.PNG)</p>

Finally, picture 2-3 show the best model which is the Voting Ensemble.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%202-3.PNG)</p>

### Step 3: 

Picture Step 3 show that the deployed best model was completed.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%203.PNG)</p>

### Step 4: 

Picture Step 4-1 show that the Application Insights are enabled.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%204-1.PNG)</p>

Picture Step 4-2 show that the logs.py file is running and reports logs back.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%204-2.PNG)</p>

### Step 5: 

Picture Step 5 show that the API swagger localhost page for the consumed best autoML model.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%205.PNG)</p>

### Step 6: 

Picture Step 6 show the output from the run of the endpoint.py file. Benchmark was an optional step which I didnt complete.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%206.PNG)</p>

### Step 7: 

<p>Pictures Step 7-1, 7-2, 7-3, 7-4, 7-5, 7-5b, 7-6 below show the outputs from running the aml-pipelines-with-automated-machine-learning-step.ipynd notebook file. It is apparent that running through the cells of the jupyter notebook, I created/consumed and published the best model for the bank marketing dataset using AutoML with Python SDK.</p>

Picture Step 7-1 shows that Pipeline has been created.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-1.PNG)</p>

Picture Step 7-2 shows the Pipeline endpoints.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-2.PNG)</p>

Picture Step 7-3 shows the bank marketing dataset to be fed into the AutoML run.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-3.PNG)</p>

Picture Step 7-4 shows the REST endpoint and the status to be Active.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-4.PNG)</p>

Picture Step 7-5 and 7-5b show the Run Details from the AutoML run from the notebook.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-5.PNG)</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-5b.PNG)</p>

Picture Step 7-6 show the scheduled run from the pipeline rest endpoint which is running.</p>
![alt](https://github.com/thanasisvax/MLops-Operations/blob/master/starter_files/Pictures/Step%207-6.PNG)</p>

## Screen Recording

Recording is available in the Box folder in the following link:</p>
https://app.box.com/s/ppa7kiit05tmve9pry7mfdb39epwfcvq</p>
**Note:** The file can be downloaded from the Box link above.

 ## Improvements
The dataset looks to be biased towards the no answer on the 'y' column. So, one of the improvements on the notebook will be to try to split the data to training/cross validation/testing datasets in order to try to improve the overfitting of the model.</p> Also, we can try to create our own classification model instead of using the AutoML config machine in order to identify the best model. This will give us the opportunity to optimize our model using the hyperparameter functions.</p> Another suggestion is to enable the deep learning for the classification task in order to check if the accuracy is improved.</p> Finally, I would suggest to play more with the endpoint.py file in order to interact more with our deployed model.
