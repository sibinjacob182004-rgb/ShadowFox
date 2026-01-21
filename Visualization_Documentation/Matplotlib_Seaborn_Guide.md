# Visualization Library Documentation
## Matplotlib and Seaborn

### Introduction
Data visualization is an essential part of data science. It helps in understanding patterns, trends, and insights from data using graphical representations.

In this documentation, we explore two popular Python visualization libraries:
- Matplotlib
- Seaborn

---

## Matplotlib

### Overview
Matplotlib is a widely used Python library for creating static, animated, and interactive visualizations. It provides complete control over plots and is suitable for both simple and complex visualizations.

### Common Graph Types in Matplotlib
### Line Plot (Matplotlib)

**Description:**  
A line plot is used to show trends over time or continuous data.

**Use Case:**  
Tracking sales growth, temperature changes, or performance trends.

**Code Example:**
```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

plt.plot(x, y)
plt.xlabel("X values")
plt.ylabel("Y values")
plt.title("Simple Line Plot")
plt.show()
```

  
### Bar Chart (Matplotlib)

**Description:**  
A bar chart represents data using rectangular bars where the height of each bar corresponds to its value.

**Use Case:**  
Comparing quantities such as sales across different products or marks scored by students.

**Code Example:**
```python
import matplotlib.pyplot as plt

categories = ["A", "B", "C", "D"]
values = [10, 15, 7, 12]

plt.bar(categories, values)
plt.xlabel("Categories")
plt.ylabel("Values")
plt.title("Simple Bar Chart")
plt.show()
```

- Histogram
  ### Histogram (Matplotlib)

**Description:**  
A histogram shows the distribution of numerical data by grouping values into bins.

**Use Case:**  
Understanding data distribution such as exam scores, ages, or income ranges.

**Code Example:**
```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.randn(100)

plt.hist(data, bins=10)
plt.xlabel("Value")
plt.ylabel("Frequency")
plt.title("Simple Histogram")
plt.show()
```

- Scatter Plot
  ### Scatter Plot (Matplotlib)

**Description:**  
A scatter plot displays the relationship between two numerical variables using points.

**Use Case:**  
Analyzing relationships such as height vs weight or hours studied vs marks scored.

**Code Example:**
```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [5, 7, 4, 8, 6]

plt.scatter(x, y)
plt.xlabel("X values")
plt.ylabel("Y values")
plt.title("Simple Scatter Plot")
plt.show()
```

- Pie Chart
### Pie Chart (Matplotlib)

**Description:**  
A pie chart represents data as portions of a whole, showing percentage distribution.

**Use Case:**  
Displaying market share, budget allocation, or time spent on activities.

**Code Example:**
```python
import matplotlib.pyplot as plt

labels = ["Python", "Java", "C++", "Others"]
sizes = [40, 30, 20, 10]

plt.pie(sizes, labels=labels, autopct="%1.1f%%")
plt.title("Programming Language Usage")
plt.show()
```

## Seaborn
### Overview
Seaborn is a Python data visualization library built on top of Matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.

Seaborn works seamlessly with Pandas DataFrames and is widely used for exploratory data analysis due to its clean syntax and default styling.

### Common Graph Types in Seaborn
- Line Plot
  ### Line Plot (Seaborn)

**Description:**  
A Seaborn line plot is used to visualize trends over time or ordered data with better default styling than Matplotlib.

**Use Case:**  
Analyzing trends such as monthly sales or temperature changes.

**Code Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [5, 10, 15, 20, 25]

sns.lineplot(x=x, y=y)
plt.title("Simple Line Plot using Seaborn")
plt.show()
```
- Bar Plot
  ### Bar Plot (Seaborn)

**Description:**  
A bar plot in Seaborn shows the relationship between a categorical variable and a numerical variable.

**Use Case:**  
Comparing average values such as average marks per subject or average sales per category.

**Code Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt

categories = ["A", "B", "C", "D"]
values = [10, 15, 7, 12]

sns.barplot(x=categories, y=values)
plt.title("Simple Bar Plot using Seaborn")
plt.show()
```

- Count Plot
  ### Count Plot (Seaborn)

**Description:**  
A count plot displays the number of occurrences of each categorical value in a dataset.

**Use Case:**  
Counting the number of students in each department or number of items in each category.

**Code Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt

data = ["A", "B", "A", "C", "B", "A", "D", "C"]

sns.countplot(x=data)
plt.xlabel("Category")
plt.ylabel("Count")
plt.title("Simple Count Plot using Seaborn")
plt.show()
```

- Box Plot
  ### Box Plot (Seaborn)

**Description:**  
A box plot displays the distribution of numerical data using quartiles and highlights outliers.

**Use Case:**  
Analyzing exam scores, salary distributions, or comparing numerical values across categories.

**Code Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt

data = [45, 50, 55, 60, 65, 70, 80, 90, 100]

sns.boxplot(y=data)
plt.ylabel("Values")
plt.title("Simple Box Plot using Seaborn")
plt.show()
```

- Heatmap
### Heatmap (Seaborn)

**Description:**  
A heatmap visualizes data in a matrix format where colors represent the magnitude of values.

**Use Case:**  
Identifying correlations between numerical variables or visualizing patterns in tabular data.

**Code Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np

data = np.random.rand(5, 5)

sns.heatmap(data, annot=True)
plt.title("Simple Heatmap using Seaborn")
plt.show()
```

---

## Comparison: Matplotlib vs Seaborn

## Comparison: Matplotlib vs Seaborn

| Feature | Matplotlib | Seaborn |
|--------|------------|---------|
| Ease of Use | Moderate – requires more code | Easy – concise syntax |
| Customization | Very high | Moderate |
| Default Styling | Basic | Clean and attractive |
| Statistical Plots | Limited | Strong support |
| Data Handling | Works with NumPy & Pandas | Excellent Pandas integration |
| Best Use Case | Fine-grained control over plots | Exploratory Data Analysis |
