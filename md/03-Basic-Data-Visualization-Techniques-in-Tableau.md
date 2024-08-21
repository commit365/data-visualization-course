## Lesson 3: Basic Data Visualization Techniques in Tableau

### Creating Simple Charts

Tableau provides a user-friendly interface for creating various types of visualizations. In this section, we will cover how to create three common types of charts: bar charts, line charts, and pie charts.

#### 1. Creating a Bar Chart

Bar charts are useful for comparing quantities across different categories. Here’s how to create a bar chart in Tableau:

- **Step 1**: Open Tableau and connect to your data source. For this example, you can use the Sample Superstore dataset that comes with Tableau.
  
- **Step 2**: Drag a dimension (e.g., "Category") to the Rows shelf. This will create a row for each category in your data.
  
- **Step 3**: Drag a measure (e.g., "Sales") to the Columns shelf. Tableau will automatically generate a bar chart displaying the sales for each category.

- **Step 4**: Customize your bar chart by clicking on the "Show Me" panel and selecting different styles or colors. You can also sort the bars by clicking on the axis labels.

#### 2. Creating a Line Chart

Line charts are ideal for showing trends over time. Follow these steps to create a line chart:

- **Step 1**: Start with your dataset open in Tableau.

- **Step 2**: Drag a date dimension (e.g., "Order Date") to the Columns shelf. Tableau will automatically aggregate the dates.

- **Step 3**: Drag a measure (e.g., "Sales") to the Rows shelf. Tableau will create a line chart that shows sales over time.

- **Step 4**: To enhance the line chart, you can add more detail by dragging another dimension (e.g., "Category") to the Color shelf in the Marks card. This will create separate lines for each category.

#### 3. Creating a Pie Chart

Pie charts are useful for showing the proportion of categories within a whole. Here’s how to create a pie chart:

- **Step 1**: Open your dataset in Tableau.

- **Step 2**: Drag a dimension (e.g., "Category") to the Rows shelf.

- **Step 3**: Drag a measure (e.g., "Sales") to the Columns shelf. Tableau will create a bar chart.

- **Step 4**: Click on the "Show Me" panel and select the pie chart option. Tableau will convert your bar chart into a pie chart.

- **Step 5**: To add labels, drag the measure (e.g., "Sales") to the Label shelf in the Marks card. This will display sales values on the pie chart.

### Using Filters and Sorting to Manipulate Data Views

Filters and sorting are essential tools in Tableau that allow you to refine your data visualizations and focus on specific insights.

#### 1. Using Filters

Filters help you limit the data displayed in your visualizations. Here’s how to apply filters:

- **Step 1**: Select the visualization you want to filter.

- **Step 2**: Drag a field (e.g., "Region") to the Filters shelf. A filter dialog box will appear.

- **Step 3**: Choose the values you want to include or exclude from your visualization. You can select specific regions or use conditions to filter the data.

- **Step 4**: Click "OK" to apply the filter. The visualization will update to reflect the filtered data.

- **Step 5**: To show the filter control on the dashboard, right-click on the field in the Filters shelf and select "Show Filter." This allows viewers to interact with the filter directly.

#### 2. Using Sorting

Sorting helps you arrange your data in a meaningful order. Here’s how to sort your visualizations:

- **Step 1**: Click on the axis of the visualization you want to sort (e.g., the sales axis in a bar chart).

- **Step 2**: Click the sort icon (ascending or descending) in the toolbar. Tableau will automatically rearrange the data based on your selection.

- **Step 3**: For more advanced sorting, right-click on the field in the Rows or Columns shelf and select "Sort." You can choose to sort by field values, manual order, or a calculated field.

### Conclusion

In this lesson, you learned how to create basic charts in Tableau, including bar charts, line charts, and pie charts. You also explored how to use filters and sorting to manipulate your data views effectively. These foundational skills will enable you to visualize data clearly and derive meaningful insights as you continue your journey in data visualization with Tableau.