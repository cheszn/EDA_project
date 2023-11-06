# EDA Project
-Project related to the exploratory data analysis of King county property sales data from 2014 to 2015.

## Client detils and requirements:

Client Name: Nicole Johnson 
Role: Buyer
Requirements:
→ Neighborhood Preference: Nicole is looking for a neighborhood that is lively and centrally located within the city. She values the vibrancy and convenience of living in the heart of the city.
→ Price Range: Nicole is interested in properties that fall within the middle price range. She has a specific budget in mind and is seeking properties that align with her financial preferences.
→ Timing: Nicole is planning to make a purchase within the next year. It's crucial to find a property that meets her requirements within this timeframe.
Nicole's requirements are centered around finding a property in a lively and central neighborhood that fits her budget and aligns with her timeline for purchase. These criteria will guide the property search to ensure her needs and preferences are met.


## System Requirements

- pyenv
- python==3.11.3
- PostgreSQL:
      - HOST='your_host'
      - PORT=your port
      - DATABASE='postgres'
      - USER_DB='your_userdb_name'
      - PASSWORD='your_password'


#### Below in DB_STRING, replace "USER_DB" and "PASSWORD" with username and password used for Dbeaver setup (given by coaches)

DB_STRING = "postgresql://'your_userdb_name':'your_password'm@ds-sql-playground.c8g8r1deus2v.eu-central-1.rds.amazonaws.com:5432/postgres"

## Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you have to create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```Powershell
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*


### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

In order to install the environment you can use the following commands in Powershell:

```
python -m venv .venv
.venv\Scripts\Activate.ps1
.venv\Scripts\python.exe -m pip install --upgrade pip
pip install -r requirements.txt
Jupyter lab
'''
