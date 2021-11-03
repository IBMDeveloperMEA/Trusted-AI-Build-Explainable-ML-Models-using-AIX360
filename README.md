# Trusted AI: Build Explainable ML Models using AIX360

## Workshop Resources

- Login/Sign Up for IBM Cloud: https://ibm.biz/ExplainableAI
  
- Hands-On Guide: https://ibm.biz/ExplainableAi-HandsOn

- Slides: https://ibm.biz/ExplainableAI-Slides

- Workshop Replay: https://www.aisummit.io/

## Table of Contents
1. [About the Workshop](#About-the-workshop)
1. [Prerequisites](#Prerequisites)
1. [Architecture](#Architecture)  
1. [Steps to Follow](#Steps-to-Follow)

## About the Workshop

Imagine boarding the Titanic in 2021, and you have provided all your details as a passenger to the captain. There is are three people involved, the data scientist, captain, and the passenger. Imagine the company that has built Titanic, has created a machine ML model to predict the rate of survival of the passengers, in case of a disaster. The job of the data scientist is to make a model that is explainable to the passengers who are not technical, and that they get the answer about the reasons why they may not survive.

After pondering upon these questions, you will agree that It’s not enough to make predictions. Sometimes, you need to generate a deep understanding. Just because you model something doesn’t mean you really know how it works. 

There are multiple reasons why we need to understand the underlying mechanism of the Machine learning Models -

- Human Readability
- Bias Mitigation
- Justifiability
- Interpretability

![](https://github.com/IBM/unveiling-machine-fraud-prediction-decision-with-ai-explainability-360/blob/main/doc/source/images/AIX360_1.png)

 [**AI Explainability 360](http://aix360.mybluemix.net/), a comprehensive open source toolkit of state-of-the-art algorithms that support the interpretability and explainability of machine learning models.** 

This Code Pattern highlights the use of the AI explainability 360 toolkits to demystify the decisions taken by the machine learning model to gain better insights and explainability which not only help the policy-makers, data scientists to develop trusted explainable AI applications but also the general public for transparency and allowing them to gain insight into the machine’s decision-making process. Understanding behind the scenes is essential to fostering trust and confidence in AI systems.

To demonstrate the use of the AI Explainability 360 Toolkit, we are using the existing [Fraud Detection Code Pattern](https://developer.ibm.com/patterns/fraud-prediction-using-autoai/) showcasing, explaining, and also guide the practitioner on choosing an appropriate explanation method or algorithm depending upon the type of customer(Data Scientist, General Public, SME, Policy Maker) that needs an explanation of the model. 

This Code Pattern will also demonstrate the use of ART(Adversarial Robustness 360 Toolkit) to defend and evaluate Machine Learning models and applications against the adversarial threats of Evasion, Poisoning, Extraction, and Inference.

![https://www.ibm.com/blogs/research/wp-content/uploads/2019/08/Screen-Shot-2019-08-06-at-11.44.36-PM-1024x636.png](https://www.ibm.com/blogs/research/wp-content/uploads/2019/08/Screen-Shot-2019-08-06-at-11.44.36-PM-1024x636.png)

**No single approach to explaining algorithms**

Currently, AI explainability 360 toolkit provides eight state-of-the-art explainability algorithms that can add transparency throughout AI systems. Depending on the requirement and subjected to the problem statement you can choose them appropriately. The algorithms are explained in detail on this [link.](https://aix360.mybluemix.net/))

![](https://github.com/IBM/unveiling-machine-fraud-prediction-decision-with-ai-explainability-360/blob/main/doc/source/images/aix360_2.png)

In this Code Pattern, we will demonstrate the usage of AIX360 and how we can utilize different explainers to explain the decisions made by the machine learning model.

## Prerequisites
  
### **Sign-up/Login to IBM Cloud**

If you are an existing user please [login to IBM Cloud](https://cloud.ibm.com/registration/trial?utm_medium=Inpersondirected&utm_content=000039JL&utm_term=10010797&utm_id=Nov2021-trustedaibuildexplainablemlmodelsusingaix360-eventid-615c4ea14260e2561c73986f-global-devadvgrp--franchise-workshop-online)

And if you are not, don't worry! We have got you covered! There are 3 steps to create your account on [IBM Cloud](https://cloud.ibm.com/registration/trial?utm_medium=Inpersondirected&utm_content=000039JL&utm_term=10010797&utm_id=Nov2021-trustedaibuildexplainablemlmodelsusingaix360-eventid-615c4ea14260e2561c73986f-global-devadvgrp--franchise-workshop-online): <br>
1 - Put your email and password. <br>
2 - You get a verification link with the registered email to verify your account. <br>
3 - Fill the personal information fields. <br>
** Please make sure you select the country you are in when asked at any step of the registration process.
  
<img width="1188" alt="Screen Shot 2021-05-31 at 11 25 01 AM" src="https://user-images.githubusercontent.com/15332386/120156441-0769d980-c203-11eb-8cb3-29f4a8d5616a.png">


## Architecture 
  
![Architecture](/images/arch.png)

## Flow

1. Log in to Watson Studio powered by spark, initiate Cloud Object Storage, and  create a project.
2. Upload the .csv data file to Object Storage.
3. Load the Data File in Watson Studio Notebook.
4. Install AI Explainability 360 Toolkit in the Watson Studio Notebook.
5. Visualization for explainability and interpretability of AI Model for the three different types of Users.

## Included components

* [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio): Analyze data using RStudio, Jupyter, and Python in a configured, collaborative environment that includes IBM value-adds, such as managed Spark.

* [IBM AI Explainability 360 ](https://www.ibm.com/blogs/research/2019/08/ai-explainability-360/): The AI Explainability 360 toolkit is an open-source library that supports interpretability and explainability of datasets and machine learning models. The AI Explainability 360 Python package includes a comprehensive set of algorithms that cover different dimensions of explanations along with proxy explainability metrics.

* [IBM Cloud Object Storage](https://console.bluemix.net/catalog/services/cloud-object-storage): An IBM Cloud service that provides an unstructured cloud data store to build and deliver cost effective apps and services with high reliability and fast speed to market. This code pattern uses Cloud Object Storage.


## Featured technologies

* [Artificial Intelligence](https://developer.ibm.com/technologies/artificial-intelligence/): Any system which can mimic cognitive functions that humans associate with the human mind, such as learning and problem solving.
* [Data Science](https://developer.ibm.com/code/technologies/data-science/): Systems and scientific methods to analyze structured and unstructured data in order to extract knowledge and insights.
* [Analytics](https://developer.ibm.com/code/technologies/analytics/): Analytics delivers the value of data for the enterprise.
* [Python](https://www.python.org/): Python is a programming language that lets you work more quickly and integrate your systems more effectively.

## Steps to follow

### Step 1: Create an IBM Cloud account

Login to IBM Cloud and create an account using this link https://ibm.biz/ExplainableAI 

### Step 2: Create Watson Studio service

Go to your IBM Cloud Dashboard, type in search box "Watson studio" select the service, on the service page click create

<img width="540" alt="1" src="https://user-images.githubusercontent.com/16270682/130227865-a245e3e9-e1b4-46d5-8048-f8809d846446.PNG">

<img width="910" alt="2" src="https://user-images.githubusercontent.com/16270682/130227908-5a72177b-2fda-4a8f-8d70-fd4f8761c36a.PNG">

### Step 3. Create Cloud Object Storage

![gif 2](https://github.com/Anam-Mahmood/YPDL-Identify-Handwritten-Digits-using-CNN-with-TensorFlow/blob/main/images/ypdl%20gif.gif?raw=true)

1.	On the new project page, give your project a name. You will also need to associate an IBM Cloud Object Storage instance to store the data set.

2.	Under “Select Storage Service”, click on the “Add” button. This takes you to the IBM Cloud Object Store service page. Leave the service on the “Lite” tier and then click the “Create” button at the bottom of the page. You are prompted to name the service and choose the resource group. Once you give a name, click “Create”.

3.	Once the instance is created, you’re taken back to the project page. Click on “refresh” and you should see your newly created Cloud Object Storage instance under Storage.

4.	Click the “Create” button at the bottom right of the page to create your project.

### Step 4: Create a new Watson Studio project

Click on get started it will take you to a "Cloud Pak for Data" Dashboard. 

<img width="490" alt="3" src="https://user-images.githubusercontent.com/16270682/130227947-ead78d84-75e2-48ad-b489-18939abfdc46.PNG">

<img width="837" alt="4" src="https://user-images.githubusercontent.com/16270682/130227980-2aa2c5b4-65f7-4b39-b5a0-96fbd559536e.PNG">


Select create a project

<img width="580" alt="5" src="https://user-images.githubusercontent.com/16270682/130228261-90016159-e276-416c-af47-d3337baa4edb.PNG">

Click on create an empty project

<img width="916" alt="6" src="https://user-images.githubusercontent.com/16270682/130228274-2dcd1641-f504-43d6-aaee-ce62a942ab02.PNG">


Give your project a unique name and click on create 

<img width="930" alt="7" src="https://user-images.githubusercontent.com/16270682/130228284-6c2d3a6b-fe41-4d4a-abba-c2223443e233.PNG">

### Step 5: Create the notebook

From IBM Watson Dashboard click on "Add to project" and select "Notebook"

<img width="750" alt="10" src="https://user-images.githubusercontent.com/16270682/130228834-fb48f7fb-14f5-4cc5-9da6-15d770e9d16e.PNG">

<img width="548" alt="11" src="https://user-images.githubusercontent.com/16270682/130228859-7f3ad65d-1e87-4ee3-beaf-562ebf60bbda.PNG">

And then add the notebook using the URL using the steps below

<img width="750" alt="10" src="/images/notebook_url.png">

In the ```Add a Notebook``` section, select the ```From URL``` option, select the runtime as ```Default Python 3.7 XS (2 vCPU 8 GB RAM)```.

Add the following notebook URL in the ```Notebook URL``` field:
```
https://github.com/IBMDeveloperMEA/Trusted-AI-Build-Explainable-ML-Models-using-AIX360/blob/main/Titanic-aix360-v1.ipynb
```

### Step 5: Run the Notebook

The rest of of the concepts are explained in the notebook, let's go through them together! 

## Workshop Resources

- Login/Sign Up for IBM Cloud: https://ibm.biz/ExplainableAI
  
- Hands-On Guide: https://ibm.biz/ExplainableAi-HandsOn

- Slides: https://ibm.biz/ExplainableAI-Slides

- Workshop Replay: https://www.aisummit.io/

## Done with the workshop? Here are some things you can try further

Check out Adversarial Robustness 360 (ART): 
- https://github.com/IBM/adversarial-robustness-toolbox
- https://art-demo.mybluemix.net

Check out AI Fairness 360 (AIF360):
- https://github.com/IBM/AIF360
- https://aif360.mybluemix.net

Check out AI Factsheets 360 (AIFS360):
- https://aifs360.mybluemix.net

## Workshop Speakers

- (Fawaz Siddiqi)[https://linktr.ee/thefaz]
- (Qamar un Nisa)[https://www.linkedin.com/in/qamarnisa/]
