## Lesson 8: Advanced Plotting Techniques with Matplotlib

In this lesson, we will explore advanced plotting techniques in Matplotlib, including creating subplots and complex figures, as well as using Matplotlib in conjunction with Pandas for data manipulation and visualization.

### Creating Subplots and Complex Figures

Subplots allow you to display multiple plots in a single figure, making it easier to compare different datasets or visualizations side by side.

#### 1. Creating Subplots

You can create subplots using the `subplot()` function or the `subplots()` function. Here’s how to do it:

- **Step 1**: Use the `subplots()` function to create a grid of subplots. Specify the number of rows and columns:

```python
import matplotlib.pyplot as plt

# Create a 2x2 grid of subplots
fig, axs = plt.subplots(2, 2, figsize=(10, 8))

# Sample data
x = [1, 2, 3, 4, 5]
y1 = [2, 3, 5, 7, 11]
y2 = [1, 4, 6, 8, 10]

# Plot on the first subplot
axs[0, 0].plot(x, y1, color='blue')
axs[0, 0].set_title('Line Plot 1')
axs[0, 0].set_xlabel('X-axis')
axs[0, 0].set_ylabel('Y-axis')

# Plot on the second subplot
axs[0, 1].scatter(x, y2, color='red')
axs[0, 1].set_title('Scatter Plot')
axs[0, 1].set_xlabel('X-axis')
axs[0, 1].set_ylabel('Y-axis')

# Plot on the third subplot
axs[1, 0].bar(x, y1, color='green')
axs[1, 0].set_title('Bar Chart')
axs[1, 0].set_xlabel('X-axis')
axs[1, 0].set_ylabel('Y-axis')

# Plot on the fourth subplot
axs[1, 1].hist(y2, bins=5, color='purple', alpha=0.7)
axs[1, 1].set_title('Histogram')
axs[1, 1].set_xlabel('Value')
axs[1, 1].set_ylabel('Frequency')

# Adjust layout
plt.tight_layout()
plt.show()
```

In this example, we created a 2x2 grid of subplots, each displaying a different type of plot.

#### 2. Creating Complex Figures

Complex figures can include multiple elements such as annotations, legends, and customized layouts. You can enhance your plots by adding these elements.

- **Step 1**: Create a plot with annotations and legends:

```python
# Sample data
x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

plt.figure(figsize=(8, 5))
plt.plot(x, y, marker='o', color='blue', label='Data Series')

# Adding annotations
for i, v in enumerate(y):
    plt.text(x[i], v + 0.5, str(v), ha='center', color='black')

plt.title('Complex Figure with Annotations')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.legend()
plt.grid(True)
plt.show()
```

In this example, we added annotations to each data point to display their values.

### Using Matplotlib with Pandas for Data Manipulation and Visualization

Pandas is a powerful data manipulation library that works seamlessly with Matplotlib. You can use Pandas to handle data and create visualizations easily.

#### 1. Setting Up Pandas

First, ensure you have Pandas installed. You can install it using pip:

```bash
pip install pandas
```

#### 2. Creating a DataFrame

You can create a Pandas DataFrame to hold your data. Here’s an example:

```python
import pandas as pd

# Sample data
data = {
    'Year': [2018, 2019, 2020, 2021, 2022],
    'Sales': [150, 200, 250, 300, 350],
    'Profit': [50, 80, 100, 120, 150]
}

df = pd.DataFrame(data)
```

#### 3. Plotting with Pandas

Pandas provides a convenient way to plot data directly from a DataFrame using the `plot()` method.

- **Step 1**: Create a line plot of Sales and Profit over the years:

```python
# Plotting Sales and Profit
df.plot(x='Year', y=['Sales', 'Profit'], kind='line', marker='o', figsize=(10, 6))
plt.title('Sales and Profit Over Years')
plt.xlabel('Year')
plt.ylabel('Amount')
plt.grid(True)
plt.show()
```

In this example, we created a line plot that displays both Sales and Profit over the years using a single DataFrame.

#### 4. Creating a Bar Plot

You can also create bar plots easily with Pandas:

```python
# Creating a bar plot for Sales
df.plot(x='Year', y='Sales', kind='bar', color='skyblue', figsize=(10, 6))
plt.title('Sales by Year')
plt.xlabel('Year')
plt.ylabel('Sales Amount')
plt.xticks(rotation=0)  # Rotate x-axis labels for better readability
plt.grid(axis='y')
plt.show()
```

In this example, we created a bar plot to visualize Sales by Year.

### Conclusion

In this lesson, you learned how to create subplots and complex figures in Matplotlib, enhancing your visualizations with multiple plots and annotations. You also explored how to use Matplotlib in conjunction with Pandas for data manipulation and visualization, making it easier to analyze and present your data effectively. These advanced techniques will empower you to create more sophisticated visualizations as you continue your journey with Matplotlib.