# Data-Cleaning-with-Pandas-and-Numpy
This project involves a detailed data cleaning process, documented in a Jupyter notebook. 
The Jupyter notebook contains detailed steps and methodologies used to transform the raw data into a more usable form.

### Data Source
The dataset used in this project is the [FIFA 21 Messy Raw Dataset](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring?select=fifa21+raw+data+v2.csv) gottenfrom Kaggle. It includes various player attributes and performance metrics from the popular video game FIFA 21.

### Objectives
The main objectives of the data cleaning process include:

* Handling missing values
* Correcting data types
* Data transformation for better analysis

### Methodology
The Jupyter notebook details the following steps:

- Initial Data Exploration:
 * Basic exploration to understand the structure and issues in the dataset.
- Data Cleaning:
 * Data type corrections: Converting data into appropriate types.
     * A function was defined to convert various string representations of measurements and values into their numerical equivalents.
     * This function was used to handle conversions for units like centimeters ('cm'), feet and inches ('ft'in"), kilograms ('kg'), pounds ('lbs'), as well as monetary values in thousands ('K') and millions ('M'), and ratings indicated by stars ('★'). It's designed to parse and transform these diverse formats into a consistent float or integer format for easier data processing and analysis.
 * Data Transformation: Methods used for transforming data into a more analyzable format.
     * The 'Joined' column, which is in the format 'Month day, year', was transformed into a pandas datetime object, handling any parsing errors.
     * Three new columns: 'Joined_Year', 'Joined_Month', and 'Joined_Day' were created, extracting the respective year, month, and day from the converted datetime. This enhances the dataset by breaking down the joining date into separate, more analyzable components."
 * Handling missing values: Strategies used to fill or remove missing data.
     * Drop the redundant columns and rows with missing values

### Libraries Used
* Pandas: For data manipulation and analysis.
* NumPy: For numerical operations.

### How to Use
* Clone this repository.
* Ensure you have Jupyter Notebook installed.
* Open the notebook FIFA_21_Data_Cleaning.ipynb.
* Install required libraries
* Run the notebook to view the data cleaning process.

### Contributions and Feedback
Feel free to fork this project, submit pull requests, or send suggestions to improve the data cleaning process.
