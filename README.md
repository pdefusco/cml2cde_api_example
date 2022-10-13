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
The "sql.py" script is already provided to you when you clone this project.

The "run_spark_job" method in the last cell executes a small Spark SQL script in CDE.
This shouldn't affect your data or any other jobs running in your CDE VC.

In addition:
* There are no requirements.txt files to install
* There are no CML Project Environment Variables to set. Your CDP User and Password are automatically tracked by CML.
* There is no need to preupload data to Cloud Storage. All data is created by the PySpark Script.
