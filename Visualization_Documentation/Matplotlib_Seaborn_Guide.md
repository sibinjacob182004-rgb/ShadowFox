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

- Histogram
- Scatter Plot
- Pie Chart

---

## Seaborn

### Overview
Seaborn is a high-level visualization library built on top of Matplotlib. It provides attractive default styles and is mainly used for statistical data visualization.

### Common Graph Types in Seaborn
- Line Plot
- Bar Plot
- Count Plot
- Box Plot
- Heatmap

---

## Comparison: Matplotlib vs Seaborn

| Feature | Matplotlib | Seaborn |
|------|-----------|---------|
| Ease of Use | Moderate | Easy |
| Customization | High | Moderate |
| Default Styling | Basic | Attractive |
| Statistical Plots | Limited | Strong |
| Best Use Case | Detailed control | Quick analysis |
