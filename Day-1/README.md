[![Static Badge](https://img.shields.io/badge/Agenda-1f7a78?style=flat&logoSize=auto)
](https://github.com/paletterz/7days)

### 🔹 Day1: Introduction to Platter (Navigation & Core Concepts)
In this first day of the 7-day learning plan, we will focus on getting you familiar with Platter, a powerful tool for data analysis and visualization. We will cover the installation process,navigate through the Platter interface, and introduce you to the core concepts that will help you get started with Platter.

#### 1. Install Platter and Set Up Your Environment

To begin, you need to install Platter on your computer. Follow the instructions provided in the official Platter documentation to download and install the software. Once you have Platter installed, set up your environment by creating a new project and organizing your files. This will help you keep your work organized and make it easier to manage your datasets and visualizations as you progress through the learning plan. Make sure to also install any necessary dependencies or libraries that Platter may require for your data analysis tasks.

#### 2. Explore the Platter Interface

Take some time to familiarize yourself with the Platter interface. Explore the different panels, menus, and tools available. Pay attention to the layout and how you can access various features. This will help you navigate efficiently as you work on your data analysis projects.
#### 3. Understand Core Concepts
Platter is built on several core concepts that are essential for effective data analysis. These include:
- **Datasets**: Platter allows you to work with various datasets. Learn how to import and manage your datasets within Platter.
- **Visualizations**: Platter provides a wide range of visualization options. Explore how to create different types of visualizations to represent your data effectively.  
- **Transformations**: Platter offers powerful data transformation capabilities. Understand how to manipulate and transform your data to gain insights.
- **Workflows**: Platter enables you to create workflows to automate your data analysis processes. Learn how to set up and manage workflows to streamline your analysis.
#### 4. Hands-On Practice

To solidify your understanding of Platter, try working on a simple data analysis project. Import a dataset, create some visualizations, and apply transformations to explore the data. This hands-on practice will help you become more comfortable with the Platter interface and its core concepts.   
By the end of Day 1, you should have a good understanding of how to navigate Platter and be familiar with its core concepts. This foundation will set you up for success as you continue to explore more advanced features in the coming days.

#### 5. Hand-On Exercise

To reinforce your learning, try the following exercise:
- Import a sample dataset (e.g., a CSV file containing sales data).
- Create a bar chart to visualize the total sales by product category.
- Apply a transformation to calculate the average sales per month.
- Set up a workflow to automate the process of importing the dataset, creating the visualization, and applying the transformation.  
This exercise will help you practice the skills you've learned and give you a practical understanding of how to use Platter for data analysis.

#### 6. Hands-on Exercise Solution

Here is a step-by-step solution to the exercise:
1. Import the dataset:
```python
import pandas as pd
data = pd.read_csv('sales_data.csv')
```
2. Create a bar chart:
```python
import matplotlib.pyplot as plt
sales_by_category = data.groupby('product_category')['sales'].sum()
sales_by_category.plot(kind='bar')
plt.title('Total Sales by Product Category')
plt.xlabel('Product Category')
plt.ylabel('Total Sales')
plt.show()
```
3. Calculate average sales per month:
```python
data['month'] = pd.to_datetime(data['date']).dt.month
average_sales_per_month = data.groupby('month')['sales'].mean()
print(average_sales_per_month)
```
4. Set up a workflow:
```python
def import_data(file_path):
    return pd.read_csv(file_path)
def create_bar_chart(data):
    sales_by_category = data.groupby('product_category')['sales'].sum()
    sales_by_category.plot(kind='bar')
    plt.title('Total Sales by Product Category')
    plt.xlabel('Product Category')
    plt.ylabel('Total Sales')
    plt.show()
def calculate_average_sales(data):
    data['month'] = pd.to_datetime(data['date']).dt.month
    average_sales_per_month = data.groupby('month')['sales'].mean()
    print(average_sales_per_month)

# Workflow execution
data = import_data('sales_data.csv')
create_bar_chart(data)
calculate_average_sales(data)
```
By following these steps, you will have successfully completed the exercise and gained practical experience with Platter's features. Keep practicing and exploring to further enhance your skills!

#### 7. Hands-on Exercise Solution Explanation

In the solution provided, we first import the necessary libraries and read the dataset using `pandas`. We then create a bar chart to visualize total sales by product category using `matplotlib`. Next, we calculate the average sales per month by extracting the month from the date and grouping the data accordingly. Finally, we set up a workflow by defining functions for each step of the process and executing them in sequence. This structured approach allows us to automate the data analysis process and ensures that we can easily repeat the analysis in the future with different datasets. By practicing these steps, you will become more proficient in using Platter for your data analysis projects.

#### 8.Hands-on Exercise Solution using the Platter interface

To complete the exercise using the Platter interface, follow these steps:
1. Import the dataset:
- Open Platter and navigate to the "Datasets" panel.
- Click on "Import Dataset" and select your CSV file containing the sales data.
2. Create a bar chart:
- Go to the "Visualizations" panel and select "Bar Chart".
- Drag and drop the "product_category" field to the x-axis and the "sales" field to the y-axis.
- Customize the chart by adding titles and labels as needed.
3. Calculate average sales per month:
- In the "Transformations" panel, create a new transformation to extract the month from the date field.
- Group the data by month and calculate the average sales using the transformation tools provided by Platter.
4. Set up a workflow:
- Navigate to the "Workflows" panel and create a new workflow.
- Add steps to import the dataset, create the bar chart, and calculate the average sales per month.
- Save and execute the workflow to automate the entire process.
By following these steps within the Platter interface, you will have successfully completed the exercise and gained practical experience using Platter's features without writing code. This hands-on practice will help you become more comfortable with the Platter interface and its capabilities for data analysis and visualization. Keep exploring and experimenting with different datasets and visualizations to further enhance your skills!

#### 9. Conclusion

Congratulations on completing Day 1 of the Platter learning plan! You have successfully installed Platter
and familiarized yourself with its interface and core concepts. This foundation will be crucial as you continue to explore more advanced features and techniques in the coming days. Remember to practice regularly and experiment with different datasets and visualizations to deepen your understanding of Platter. Happy learning!