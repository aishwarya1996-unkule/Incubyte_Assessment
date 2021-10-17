# Incubyte-assessment

## 🔹Overview:
This repository contains implementation of given [assessment](https://github.com/gauravpore/Incubyte-assessment/blob/main/Data_Engineer_Assessment.pdf). The working of data pipeline is demonstarted using tools listed below. Also, a dummy [database](https://github.com/gauravpore/Incubyte-assessment/tree/main/data) has been created to demonstarte a simple data flow in different formats from server to the local system, using country-based row filteration.

🔸**Concepts:**
- Oracle Connection 
- ETL

🔸**Tools & Technologies:**
- Python 
- cx_Oracle
- Oracle Server
- [Pandas](https://pandas.pydata.org/docs/)
- [Conda Environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#activating-an-environment)
- [Oracle connector](https://www.oracle.com/database/technologies/appdev/python/quickstartpythononprem.html)

## 🔹Working:
- Firstly Oracle database has been created with specified schema.
- [```databaseConnector.py```](https://github.com/gauravpore/Incubyte-assessment/blob/main/connector.py) python script, fetches database by establishing connection with MySQL server. (Note: Make sure the XAMMP server is running while executing the script)
- The retrieved data is fitted into pandas dataframe for further table manipulation.
- ```show_data()``` & ```getfile()``` functions are called to fetch the desired data rows and generating ```.csv``` and ```string``` file formats to specified path, accepting country names as parameters for filtering rows. 
- For example: ```get_file("IND")``` generates [```IND.csv```](https://github.com/gauravpore/Incubyteassessment/blob/main/data/sample_data/IND.csv) to the specified local path. CLick [here](https://github.com/gauravpore/Incubyte-assessment/tree/main/data/sample_data) to see sample output files.


####  📌*Note: This submission is sujected to further improvements.*
  
  >🔸Installation Guide:
- To install ```cx_Oracle```:
```
pip install cx_Oracle
```
- To install pandas:
```
pip install pandas
```
## 🔹References:
- [Oracle Connector Python](https://www.oracle.com/database/technologies/appdev/python/quickstartpythononprem.html)
- [Pandas docs](https://pandas.pydata.org/docs/)

## 🔹Contribution:
Contributions are always welcomed.
Make sure you read the [Contribution info](https://github.com/gauravpore/Weather-Forecaster-App/blob/main/contribution.md)

## 🔹Screenshots:
#### 🔸PyCharm console:
![alt tag](https://user-images.githubusercontent.com/67472558/122553078-c53ef580-d054-11eb-97a6-1b756ebc5c6b.png)

#### 🔸Oracle console:
![alt tag](https://user-images.githubusercontent.com/67472558/122553074-c3753200-d054-11eb-92b0-cc868750e5cd.png)

