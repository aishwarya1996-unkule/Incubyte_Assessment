# Incubyte-assessment

## 🔹Overview:
This repository contains implementation of given [assessment](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/blob/main/Data%20Engineer%20Assignment%20-%20C-DAC.pdf). The working of data pipeline is demonstarted using tools listed below. Also, a dummy [database](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/tree/main/Data%20Files) has been created to demonstarte a simple data flow in different formats from server to the local system, using country-based row filteration.

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
- [```databaseConnector.py```](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/tree/main/Code/databaseConnector.py) python script, fetches database by establishing connection with Oracle server. (Note: Make sure the XAMMP server is running while executing the script)
- The retrieved data is fitted into pandas dataframe for further table manipulation.
- ```show_data()``` & ```getfile()``` functions are called to fetch the desired data rows and generating ```.csv``` and ```string``` file formats to specified path, accepting country names as parameters for filtering rows. 
- For example: ```get_file("IND")``` generates [```IND.csv```](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/tree/main/Data%20Files/IND.csv) to the specified local path. CLick [here](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/tree/main/Data%20Files) to see sample output files.


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

## 🔹Screenshots:
#### 🔸Jupytor console:
![alt tag](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/blob/main/Screenshots/Jupytor_Console.png)

#### 🔸Oracle console:
![alt tag](https://github.com/aishwarya1996-unkule/Incubyte_Assessment/blob/main/Screenshots/Oracle_Console.png)

