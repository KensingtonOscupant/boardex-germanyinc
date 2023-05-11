# BoardEx for Germany Inc

This GitHub repository contains Python code that helps in the analysis of board members for companies in the German market. It focuses on using BoardEx data to distinguish between board members with the same name.

## Purpose

The purpose of this repository is to provide researchers with a set of tools to analyze and differentiate between board members with similar names. The BoardEx database contains detailed information on board members of different companies, including their names, positions, and seniority levels. However, the database has some limitations when it comes to disambiguating board members with the same name. 

The code in this repository helps to overcome these limitations by leveraging SQL queries to retrieve data from the BoardEx database and Pandas data frames to manipulate and analyze the data.

## Contents

The repository contains a Python script named `boardex_sample_script.ipynb` that includes several functions to retrieve and analyze board members' data. 

The script uses the following libraries:

- wrds: A Python package that provides an interface to the Wharton Research Data Services (WRDS) platform.
- pandas: A Python library used for data manipulation and analysis.

The functions included in the `boardex_analysis.py` script are:

1. `query_boardex_data()`: This function connects to the WRDS database and retrieves data from the `boardex_eur.eur_wrds_org_composition` table. It returns a Pandas data frame with the selected data.

2. `get_directors_with_multiple_ids()`: This function groups the data frame by director name and counts the number of unique director IDs for each name. It returns a Pandas data frame with the names of the directors who have multiple IDs.

3. `query_director_data()`: This function queries the `boardex_eur.eur_wrds_org_composition` table for a specific director's name and returns a Pandas data frame with the selected data.

The `boardex_analysis.py` script also includes an example of how to use the functions to analyze board members' data.

## Usage

To use this repository, you will need to have access to the BoardEx database through the WRDS platform. You will also need to install the `wrds` and `pandas` libraries.

Additionally, this code is intended to be run on JupyterHub, a web-based platform for interactive computing. To use this code on JupyterHub, follow these steps:

1. Log in to your JupyterHub account.
2. Open a terminal and navigate to the directory where you want to clone the repository.
3. Clone the repository to your local machine using the following command:

'''git@github.com:KensingtonOscupant/boardex-germanyinc.git'''


4. Launch JupyterLab or Jupyter Notebook from the JupyterHub interface.
5. Open the `boardex_sample_script.ipynb` notebook from the cloned repository directory.
6. Follow the instructions in the notebook to use the functions to retrieve and analyze data from the BoardEx database.

The example code included in the notebook demonstrates how to use the functions to retrieve and analyze data from the BoardEx database.


