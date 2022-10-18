# Using the CML2CDE Module

## Objective

The example notebook "cml2cde_api_example.ipynb" shows an example of using the cml2cde api to submit a PySpark script from the CML project folder to CDE

## Requirements

The following are required to run the notebook:
* A CML Workspace (Azure, AWS or Private Cloud)
* A CDE Virtual Cluster (Azure, AWS or Private Cloud)

## Instructions

1. Clone this GitHub Repository as a CML Project.

2. In the CDE Virtual Cluster Service page copy the JOBS API URL value for your Virtual Cluster.

3. Launch a CML Session with Jupyter Lab editor, open the "cml2cde_api_example.ipynb" notebook and enter the JOBS API URL value in the third cell.

No other code changes are required for the remaining cells. You can execute each in sequence.
Optionally, you can change values for CDE_RESOURCE_NAME and CDE_JOB_NAME as needed.
The "sql.py" script is already provided and placed in the correct path for you upon cloning this GitHub repository.

The "run_spark_job" method in the last cell executes a small Spark SQL script in CDE.
This shouldn't affect your data or any other jobs running in your CDE VC.

In addition:
* There are no requirements.txt files to install
* There are no CML Project Environment Variables to set. Your CDP User and Password are automatically tracked by CML.
* There is no need to preupload data to Cloud Storage. All data is created by the PySpark Script.

## Conclusions

Cloudera Machine Learning (CML) is Cloudera’s cloud-native machine learning platform built for CDP. Cloudera Machine Learning unifies self-service data science and data engineering in a single, portable service as part of an enterprise data cloud for multi-function analytics on data anywhere.

It empowers organizations to build and deploy machine learning and AI capabilities for business at scale, efficiently and securely, anywhere they want. It’s built for the agility and power of cloud computing, but isn’t limited to any one cloud provider or data source.

* CML Analytic Applications give data scientists a way to create ML web applications/dashboards and easily share them with other business stakeholders. Applications can range from single visualizations embedded in reports, to rich dashboard solutions such as Tableau. They can be interactive or non-interactive.

* CML exposes a REST API that you can use to perform operations related to projects, jobs, and runs. You can use API commands to integrate CML with third-party workflow tools or to control CML from the command line.

If you have any questions about CML or would like to see a demo, please reach out to your Cloudera Account Team or send a message [through this portal](https://www.cloudera.com/contact-sales.html) and we will be in contact with you soon.
