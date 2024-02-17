# dio_challenges_azure_ml_auto_ml
Project made during DIO's "Microsoft Azure AI Fundamentals" Bootcamp, under the section "Trabalhando com Machine Learning na Prática no Azure ML"

Steps followed to create the model are described in the following links:

- [Explore Azure AI Services](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html)
- [Explore Automated Machine Learning in Azure Machine Learning](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

## Followed step-by-step:

1. Creating a Machine Learning workspace at Azure Portal: selected "Create resource" then searched for "Azure Machine Learning" in the marketplace
2. Configuring the resource, indicating the subscription plan, the resource group, and the workspace details, and finally selecting "Review + create"
3. After creating resource, selecting "Go to resource" then "Launch studio"
4. Creating an Automated ML job by going to "Automated ML" option then selecting "New Automated ML job"
5. Filling fields "Job name", "New experiment name" and "Description" at Basic settings
6. Selecting task type as "Regression"
7. Creating new dataset under "Select dataset", by filling the fields "Name" and "Description", and selecting data type as "Tabular"
8. Selecting data source as "From web files"
9. Indicating the following URL: https://aka.ms/bike-rentals
10. Filling the required info in "Settings" and verifying data types in "Schema", and finally selecting "Create"
11. Selecting created dataset, and then indicating "Rentals" as target column
12. Configuring limits and selecting "Train-validation split" as validation type under "Validation and test"
13. Configuring the compute and then submiting the job; it starts automatically
14. After finishing training, creating model by going to "Job" and then "Overview", selecting the best model under "Algorithm name", selecting "Metrics" and then "residuals" and "predicted_true" charts if not already selected; select "Deploy" and select "Web service" to deploy the model
15. Waiting for the deploy status to change to "Succeeded"
16. Testing the deployed service by going to "Endpoints" and selecting the "Test" tab
17. Inputting the JSON shown in base_test.json; the returned result is indicated in result.json



