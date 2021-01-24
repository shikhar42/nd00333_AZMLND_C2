
# Operationalizing Machine Learning

In this project, The Bank Marketing dataset was used. An AutoML experiment was created to find the best model and then the best model was deployed and consumed. Later, I also created, published and consumed a pipeline using the Azure SDK.

## Architectural Diagram
![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/flowchart.png?raw=true "Flowchart")


## Key Steps
### 1. AutoML Experiment

First, I uploaded the bank marketing dataset in azure.

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/2.%20datasets.PNG?raw=true "Dataset")

Next, we ran an AutoML Experiment. The screenshot below shows that the run was completed.

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/2.%20automl%20complete.PNG?raw=true "AutoML")

Finally in this step, we will find the best model and use it for our further analysis. Below is the screenshot of our best model.

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/2.%20Best%20Model.PNG?raw=true "Best Model")

### 2. Deploy

As it is clear from step 1 that the best model is Voting Ensemble, the next step would be to deploy this model.

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/3.%20Deploy1.PNG?raw=true "Deploy")

### 3. Enable Logging

Now, the next step is to enable logging. Here, we will enable the application insights of the deployed model so that it can be consumed. To enable application insights, I have added "service.update(enable_app_insights=True)" this statement to my code. 

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/4.%20Application%20Insights%202..PNG?raw=true "Insights")

Next, we can see that the url is available

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/4.%20Application%20Insights.PNG?raw=true "Enabled Insights")

Finally, we can also check the logs after running the logs.py

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/4.%20Application%20Insights%201.PNG?raw=true "logs.py")

### 4. Swagger Documentation

In this step, we will consume the deployed model using Swagger. First, we have to download the swagger.json file from the deployed model. Then we have to run serve.py script which serves our json using python script. Below are the screenshots of the documentation page including the get and post requests.

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/5.%20Main.PNG?raw=true "main screen")

#### Swagger Get Request
![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/5.%20Get.PNG?raw=true "Get.")

#### Swagger Post Request

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/5.%20Post%201.PNG?raw=true "post.")

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/5.%20Post%202.PNG?raw=true "post2.")

### 5. Consume Model Endpoint

Once the model is deployed, we use the endpoint.py script provided to interact with the trained model. Below is a screenshot of the response returned by the model

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/6%20consume.PNG?raw=true "endpoint")

### 6. Create, Publish and Consume a Pipeline

In this step, we will use jupyter notebook to create, publish and consume a pipeline.

From the below screenshot, we can confirm that the azure ML pipeline was completed in the experiments section:

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/7.%20Pipeline%20Created.PNG?raw=true "pipeline create")

#### Pipeline Endpoint

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/7.%20Pipeline%20Endpoint.PNG?raw=true "endpoint created")

#### Pipeline Run from RunDetails widget in Jupyter Notebook

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/7.%203.PNG?raw=true "run widget")

#### Completed Pipeline and Endpoint

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/7.%204.PNG?raw=true "status")

![Alt text](https://github.com/shikhar42/nd00333_AZMLND_C2/blob/master/rest%20endpoint.PNG?raw=true "status")

## Suggestions for Improvement

1) Deploy using AKS and compare the deployment time and cost.
2) We also noticed from the output that the data is biased towards one class. Hence, different sampling methods should be tried.


## Screen Recording

https://www.youtube.com/watch?v=-un1YJT1-HQ

