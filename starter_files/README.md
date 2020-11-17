# Operationalizing Machine Learning
In this project, I used Microsoft Azure to configure a cloud-based machine learning production model, deploy it, and consume it. I also created, published and consumed a pipeline using the Azure SDK.

## Architectural Diagram
![Design](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/Architectural%20Design.png)

## Key Steps
1. Create an experiment using AutoML, attach a database, configure a compute cluster, and use that cluster to run the experiment. The experiment returns the best model.
![Registered Dataset](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/2_registered_dataset.png)
![Completed Experiment](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/2_completed_experiment.png)
![Best Model Summary](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/2_best_model_summary.png)
![Best Model Details](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/2_best_model_details.png)
2. Deploy the model.
3. Enable Application Insights.
![Application Insights Enabled In Deployed Model](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/4_application_insights_enabled.png)
![Logs In Portal](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/4_logs.png)
![Logs In Bash](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/4_logs_bash.png)
4. Consume the deployed model using Swagger.
![Swagger API Documentation](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/5_swagger_docs.png)
![Swagger APIS 1](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/5_swagger_apis_1.png)
![Swagger APIS 2](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/5_swagger_apis_2.png)
![Swagger APIS 3](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/5_swagger_apis_3.png)
5. Consume the model endpoints and show benchmarks for the endpoint.
![Endpoing Output](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/6_endpoint_output.png)
![Benchmarks 1](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/6_benchmark_1.png)
![Benchmarks 2](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/6_benchmark_2.png)
6. Use Jupyter Notebook to create, publish and consume a pipeline.
![Dataset](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_dataset.png)
![Published Pipeline Overview](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_published_pipeline_overview.png)
![Run Details](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_run_details.png)
![Scheduled Run](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_scheduled_run.png)
![Pipeline Created](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_pipeline_created.png)
![Pipeline Endpoint](https://github.com/SLane35/nd00333_AZMLND_C2/blob/master/7_pipeline_endpoint.png)


## Screen Recording
https://drive.google.com/file/d/1po8V5YdENGH6uFTg2Meo101XdgR-Whl1/view?usp=sharing

## Suggestions For Improvement
A future project could deploy the model using different settings and types of authentications to see how that affects the deployment.



