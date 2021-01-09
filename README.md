
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



## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
