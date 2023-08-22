# JupyterLab_1

---

*A simple program in python, utilizing JupyterLab, to create a graph to display the name, age, and city*


---


1. **Download Python 3**: Make sure you have Python 3 installed. You can download it from [python.org](https://www.python.org/downloads/).

2. **Download and Run Jupyter Notebook**:
   - Download and install Python 3.
   - Open your terminal.
   - Enter the command `jupyter notebook` to launch Jupyter Notebook.
   
   Note: If you haven't installed Jupyter Notebook, you can do so by running `pip install jupyter` in your terminal.

---

### Cell 1: 
You load a dataset and display the first few rows to get an initial sense of the data.

### Cell 2: 
You preprocess the data, such as removing missing values, and display information about the number of rows before and after cleaning.

### Cell 3: 
You perform data analysis and visualization by creating a histogram of the 'age' column.
By breaking down your code into separate cells, you can focus on one task at a time, easily modify and re-run cells as needed, and keep your analysis organized and readable. Each cell's output is displayed below the cell, allowing you to see results and observations as you progress through your analysis.

---


#### Cell 1 - Data Loading and Exploration:

```
# Load necessary libraries
import pandas as pd

# Load a sample dataset (you can replace this with your own data)
data = pd.read_csv('sample_data.csv')

# Display the first few rows of the dataset
data.head()
```

* This cell starts by importing the pandas library, which is a powerful tool for data manipulation and analysis.
* It then uses the pd.read_csv() function to load a dataset from a CSV file named 'sample_data.csv'. You would replace this with the actual path to your dataset.
* The data.head() function is used to display the first few rows of the dataset. This helps you quickly get an overview of the data's structure and contents.



#### Cell 2 - Data Preprocessing:

```
# Perform data preprocessing
# For example, let's remove any rows with missing values
data_cleaned = data.dropna()

# Display the number of rows before and after cleaning
print("Rows before cleaning:", len(data))
print("Rows after cleaning:", len(data_cleaned))
```

* This cell focuses on data preprocessing. The line data_cleaned = data.dropna() removes any rows with missing values from the dataset. The result is stored in a new DataFrame called data_cleaned.
* The print() statements display the number of rows in the original dataset before cleaning and the number of rows in the cleaned dataset after removing missing values. This helps you understand the impact of the preprocessing step.



#### Cell 3 - Data Analysis and Visualization:

```
# Perform data analysis and visualization
# For example, let's plot a histogram of a numeric column
import matplotlib.pyplot as plt

plt.figure(figsize=(8, 6))
plt.hist(data_cleaned['age'], bins=20, color='blue', alpha=0.7)
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
```


* This cell focuses on data analysis and visualization. It begins by importing the matplotlib.pyplot library, which is used for creating visualizations.
* The code then creates a histogram of the 'age' column from the data_cleaned DataFrame. The plt.hist() function generates the histogram plot with specified bins, color, and transparency.
* The following lines set the title, x-label, y-label, and then use plt.show() to display the plot in the notebook.
