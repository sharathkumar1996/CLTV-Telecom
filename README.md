## **Business Overview**

Customer Lifetime Value (CLTV) is a crucial metric that measures the total revenue a customer is expected to generate during their relationship with a company. CLTV is an important metric for telecom companies because it helps them understand the value of their customer base and make strategic decisions about customer acquisition and retention.

This Project is part of the "telecom data" cluster of projects, targeting the telecom industry. It is recommended to go through the ["Exploratory Data Analysis"](https://www.projectpro.io/data-science-use-cases/telecom-data-analysis-project) notebook before executing this project to understand the Data better. 

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

#### **Setting up a Python Virtual Environment on Mac**

* Open the Terminal by pressing `Command + Spacebar`, type `Terminal`, and press `Enter`.
* Navigate to the directory where you want to create the virtual environment.
* Install virtualenv by running the following command in the terminal `pip install virtualenv`
* Create a new virtual environment by running the following command `virtualenv env`
* This will create a new directory called `env`, containing the virtual environment.
* Activate the virtual environment by running the following command `source env/bin/activate`
* You can now install packages and work on your project within this virtual environment.
* To deactivate the virtual environment, simply run the following command `deactivate`

#### **Setting up a Python Virtual Environment on Linux**

* Open the Terminal by pressing `Ctrl + Alt + T`.
* Navigate to the directory where you want to create the virtual environment.
* Install `virtualenv` by running the following command in the terminal `sudo apt-get install python3-virtualenv`
* Create a new virtual environment by running the following command `virtualenv -p python3 env`
* This will create a new directory called `env`, containing the virtual environment.
* Activate the virtual environment by running the following command `source env/bin/activate`
* You can now install packages and work on your project within this virtual environment.
* To deactivate the virtual environment, simply run the following command `deactivate`

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
    

![CLTV-project structure.png](data:image/png;base64,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)



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

### **Database**
Most organizations store their data in databases such as MS SQL. Microsoft SQL Server (MS SQL) is a relational database management system developed by Microsoft. A BAK file in Microsoft SQL Server is a backup file that contains a copy of a SQL Server database at a specific point in time. It is essentially a binary representation of the database and includes all its data, tables, schema, indexes, stored procedures, and other objects.

#### **Installing MS SQL Management Studio**
To install Microsoft SQL Server Management Studio, you can follow these steps:

* Go to the Microsoft SQL Server Downloads page (https://www.microsoft.com/en-us/sql-server/sql-server-downloads) and click on the "Download now" button for the version of SQL Server Management Studio that you want to install.
* Follow the instructions on the screen to download the installation file to your computer.
* Once the download is complete, locate the installation file and double-click on it to start the installation process.


#### **Restore a BAK file in MS SQL**

* Open SQL Server Management Studio and connect to the SQL Server instance to which you want to upload the BAK file.
* Right-click on the Databases folder in the Object Explorer pane and select "Restore Database..." from the context menu.
* In the "Restore Database" dialog box, select the "Device" option under the "Source" section.
* Click on the "..." button to open the "Select backup devices" dialog box.
In the "Select backup devices" dialog box, click on the "Add" button to add the BAK file that you want to upload.
* In the "Locate Backup File" dialog box, browse to the location where the BAK file is stored in the Telecom Data Analysis Project to Improve Service Quality directory under the ‘data’ folder, select the file, and click on the "OK" button.
* Back in the "Select backup devices" dialog box, the BAK file you added should now be listed under "Backup media:".
* Click on the "OK" button to close the "Select backup devices" dialog box.
In the "Restore Database" dialog box, you should see the BAK file listed in the "Backup sets to restore" section.
* By default, the original database name and file locations from the BAK file will be used. If you want to restore the database with a different name or to a different location, you can modify the "To database" and "Restore as" options under the "General" section.
* Click the "Options" tab for additional restore options.
* If you want to overwrite an existing database with the same name, you can select the "Overwrite the existing database (WITH REPLACE)" option under the "Restore options" section.
* Click on the "OK" button to start the restore process.
* Once the restore process is complete, you should see a message indicating that the restore was successful.

#### **Read Data from DB to Python**
 The data can be accessed by secret credentials, which will be in the following format.
```
import pyodbc
import pandas as pd
connection = pyodbc.connect('DRIVER={ODBC Driver 17 for SQL Server};\
                       SERVER=server_name;\
                       PORT=1433;\
                       DATABASE=database_name;\
                       UID=admin;\
                       PWD=password')
```
#### **Steps to install ODBC driver**
* Go to the Microsoft Download Center page for the ODBC Driver 17 for SQL Server: https://www.microsoft.com/en-us/download/details.aspx?id=56567
* Select the download button that corresponds to the operating system you are using.
* Select the language you want to use for the installer, then click the download button.
* Once the download is complete, run the installer.
* Accept the license terms, then select the features you want to install.
Choose a location to install the driver, or use the default location.
* Complete the installation process by following the instructions provided by the installer.
* Once the installation is complete, you can use the ODBC Driver 17 for SQL Server to connect to SQL Server databases from applications that support ODBC connectivity.

#### **Query to read the data into Pandas**

```
query = '''select * from Processed_month_1_data
           UNION ALL
            select * from Processed_month_2_data
            UNION ALL
            select * from Processed_month_3_data
            UNION ALL
            select * from Processed_month_4_data
            UNION ALL
            select * from Processed_month_5_data
            UNION ALL
            select * from Processed_month_6_data
            UNION ALL
            select * from Processed_month_7_data
            UNION ALL
            select * from Processed_month_8_data
            UNION ALL
            select * from Processed_month_9_data
            UNION ALL
            select * from Processed_month_10_data
            UNION ALL
            select * from Processed_month_11_data
            UNION ALL
            select * from Processed_month_12_data
            UNION ALL
            select * from Processed_month_13_data
            UNION ALL
            select * from Processed_month_14_data'''
processed_data = pd.read_sql(query,connection)
processed_data.head()

```

	
