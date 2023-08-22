# JupyterLab_1
name, age, city data plotting

Cell 1 - Data Loading and Exploration:

python
Copy code
# Load necessary libraries
import pandas as pd

# Load a sample dataset (you can replace this with your own data)
data = pd.read_csv('sample_data.csv')

# Display the first few rows of the dataset
data.head()
Cell 2 - Data Preprocessing:

python
Copy code
# Perform data preprocessing
# For example, let's remove any rows with missing values
data_cleaned = data.dropna()

# Display the number of rows before and after cleaning
print("Rows before cleaning:", len(data))
print("Rows after cleaning:", len(data_cleaned))
Cell 3 - Data Analysis and Visualization:

python
Copy code
# Perform data analysis and visualization
# For example, let's plot a histogram of a numeric column
import matplotlib.pyplot as plt

plt.figure(figsize=(8, 6))
plt.hist(data_cleaned['age'], bins=20, color='blue', alpha=0.7)
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
In this example:

Cell 1: You load a dataset and display the first few rows to get an initial sense of the data.
Cell 2: You preprocess the data, such as removing missing values, and display information about the number of rows before and after cleaning.
Cell 3: You perform data analysis and visualization by creating a histogram of the 'age' column.
By breaking down your code into separate cells, you can focus on one task at a time, easily modify and re-run cells as needed, and keep your analysis organized and readable. Each cell's output is displayed below the cell, allowing you to see results and observations as you progress through your analysis.
