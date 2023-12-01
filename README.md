## **Project Overview**

Customer Lifetime Value (CLTV) is a crucial metric that measures the total revenue a customer is expected to generate during their relationship with a company. CLTV is an important metric for telecom companies because it helps them understand the value of their customer base and make strategic decisions about customer acquisition and retention.

CLTV analysis enables companies to identify high-value customers, develop personalized retention strategies, and allocate marketing resources accordingly. It also helps companies optimize their sales and pricing strategies, improve customer satisfaction, and reduce churn rate.

It enables companies to identify high-value customers and focus their marketing and sales efforts on retaining these customers. This, in turn, leads to a reduction in customer churn rate and an increase in customer loyalty.
CLTV analysis helps companies optimize their pricing strategies by identifying which services are most valuable to customers. Companies can then adjust their pricing strategies accordingly to maximize revenue and profitability.
It also helps companies improve their overall customer satisfaction levels by identifying the factors that are most important to customers. Companies can then focus on improving these areas to ensure customer satisfaction and loyalty.

![image.png](https://images.unsplash.com/photo-1559526324-4b87b5e36e44?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1171&q=80)

CLTV can be perceived differently for revenue, customer churn, loyalty and retention. Each approach provides a different perspective on customer value and helps companies understand the different factors that impact customer lifetime.

In this project, we will be exploring different CLTV calculation methods, and analyzing feature importance to determine the most influential factors on CLTV.
We will also be identifying high-value customers based on their CLTV scores, analyzing their characteristics and behavior, and providing suggestions for targeted marketing and retention strategies.

## **Approach**

* Introduction
    * Brief overview of the project

* Data Processing

* Exploratory data analysis (EDA)
  * ARPU Analysis
  * Customer Lifetime Analysis
    
* Customer Lifetime Value
    * Overview of different CLTV calculation methods (e.g., historical, predictive, probabilistic, etc)
    * CLTV Calculation: Historical Data
    * Rule Based Customer Segmentation
    * Analyzing customers for each perspective, i.e. customer churn, loyalty, and retention
  
* Feature Importance
    * Identification of important services affecting CLTV
    * Correlation analysis to measure the impact of various factors on CLTV
    
* High-Value Customer Identification 
    * Identification of high-value customers based on CLTV scores
    * Analysis of their characteristics and behavior
    * Suggestions for targeted marketing, retention strategies
    


* Project Summary



## **Execution Instructions**



### **Installation and Setup for IPYNB**

For the best experience, please stay connected to the internet while executing this Project

#### **Running an IPYNB on Google Colab**:

* Open the [Google Colab website](https://colab.research.google.com/).
* Click on the "New Notebook" button.
* Click the "File" menu in the new notebook and choose "Upload notebook."
* Select the IPYNB file(notebooks/telco_data_analysis.ipynb) you want to upload.
* Once the file is uploaded, click on the "Runtime" menu and choose "Run all" to execute all the cells in the notebook.
* Alternatively, you can execute each cell individually by clicking the "Play" button next to the cell OR by pressing `"shift” + "enter"`.
* The Default version of Python that Colab uses currently is 3.8

#### **Python setup steps for Local Machine**:
* If you're using a local machine and do not have Python installed, follow these steps to set up Python:
* Download and install the latest version of Python from the official Python website: https://www.python.org/downloads/.
* Once the installation is complete, open a command prompt/terminal and type the following command to check if Python is installed `python –-version`
* If Python is installed, the version number will be displayed.
* This Project has been created using **Python version 3.8.10**

#### **Setting up a Python Virtual Environment on Windows**

* Open a command prompt by pressing `Windows Key + R`, type `cmd`, and press `Enter`.
* Navigate to the directory where you want to create the virtual environment.
* Install virtualenv by running the command in the command prompt `pip install virtualenv`
* Create a new virtual environment by running the command `virtualenv env`
* This will create a new directory called `env`, containing the virtual environment.
* Activate the virtual environment by running the command `env\Scripts\activate`
* You can now install packages and work on your project within this virtual environment.
* To deactivate the virtual environment, simply run the command `deactivate`

#### **Installing Jupyter with pip**
If pip is installed on your local machine, you can install Jupyter. 

Here are the steps:
* Open the command prompt (Windows) or terminal (Mac/Linux).
* Install Jupyter with pip by running the following command `pip install jupyter`
* Launch Jupyter Notebook by running the following command `jupyter notebook`

#### **Installing Jupyter with Conda**

* Download and install Anaconda from the official website: https://www.anaconda.com/products/individual.
* Open the Anaconda Navigator App and launch Jupyter Notebook 
* Running IPYNB in Jupyter Notebook
* Open Terminal / Command Prompt and Navigate to the notebooks directory using cd
* Launch Jupyter Notebook by running the following command jupyter notebook
* This will open a browser window displaying the Jupyter interface.
* Click on the IPYNB file you want to open.
* To execute all the cells in the notebook, click on the "Cell" menu and choose "Run all".
* Alternatively, you can execute each cell individually by clicking on the "Play" button next to the cell.



# Executing the project via Modular Code
1. Install the dependencies using the command, navigate to the **ML Project for Customer Lifetime Value Prediction in Telecom** directory where the requirements.txt file exists, and run ***pip install -r requirements.txt*** in the terminal/CMD.
2. Run the jupyter notebook "CLTV.ipynb" present in the notebooks folder.

3. Note: As this is a data analysis project, the analysis work is primarily done in the Jupyter notebook. Therefore, we have not created separate modular source codes for this project. Please use the project structure to run the codes in the Jupyter notebook accordingly.


## **Data Reading from Different Sources**



### **Files**

In many cases, the data is stored in the local system. To read the data from the local system, specify the correct path and filename.

### **CSV Format**
Comma-separated values, also known as CSV, is a specific way to store data in a table structure format. The data used in this project is stored in a CSV file. Download the data for the project.


Use following code to read data from csv file using pandas. 
```
import pandas as pd
csv_file_path= "D:/ProjectPro/ML Project for Customer Lifetime Value Prediction in Telecom/data/Telecom_Data.csv"
df = pd.read_csv(csv_file_path)
```
With appropriate csv_file_path, pd.read_csv() function will read the data and store it in df variable.
 
If you get *FileNotFoundError or No such file or directory*, try checking the path provided in the function. It's possible that python is not able to find the file or directory at a given location.


### **Colab - CSV Format**

```
# mount the google drive
from google.colab import drive
drive.mount('/content/drive')
csv_file_path= '/content/drive/MyDrive/project_pro/ML Project for Customer Lifetime Value Prediction in Telecom/Telecom_Data.csv'
df = pd.read_csv(csv_file_path)
```

### **AWS S3 - CSV**
Use the S3 public link to read the CSV file directly into a pandas DataFrame
```
s3_link = 'https://s3.amazonaws.com/projex.dezyre.com/customer-lifetime-value-prediction-in-telecommunications/materials/Telecom_Data.csv'
df = pd.read_csv(s3_link)
```
