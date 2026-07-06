
# 📊 Python Data Visualization Roadmap

<div align="center">

# Learn • Practice • Visualize • Build

### 🚀 A Complete Learning Repository for **Matplotlib**, **Seaborn**, **Plotly** & **Cufflinks**

From **Beginner ➜ Advanced** with Notes, Jupyter Notebooks, Examples, Exercises, Real Datasets, Interview Questions, and Projects.

---

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-blue?style=for-the-badge)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-success?style=for-the-badge)
![Cufflinks](https://img.shields.io/badge/Cufflinks-Pandas-important?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)
![GitHub](https://img.shields.io/badge/Made%20with-GitHub-black?style=for-the-badge&logo=github)

⭐ If you find this repository useful, don't forget to **Star** it!

</div>

---

# 📖 About Repository

This repository contains everything required to master Python Data Visualization from scratch.

Whether you're preparing for:

- 📊 Data Analyst Interviews
- 🤖 Data Science Interviews
- 📈 Machine Learning Projects
- 📚 College Practicals
- 💼 Industry Projects
- 🎯 Exploratory Data Analysis (EDA)

this repository will guide you step-by-step.

The content is organized from **Beginner ➜ Intermediate ➜ Advanced**, making it easy to follow without prior visualization experience.

---

# 🎯 Repository Objectives

✔ Learn Data Visualization from Scratch

✔ Understand Every Plot with Examples

✔ Perform Exploratory Data Analysis (EDA)

✔ Create Interactive Dashboards

✔ Practice with Real-World Datasets

✔ Improve Data Storytelling Skills

✔ Prepare for Technical Interviews

✔ Build an Impressive GitHub Portfolio

---

# 🚀 Libraries Covered

| Library | Purpose |
|---------|----------|
| 📊 Matplotlib | Fundamental Plotting Library |
| 🎨 Seaborn | Statistical Data Visualization |
| ⚡ Plotly | Interactive Charts & Dashboards |
| 📈 Cufflinks | Plotly + Pandas Integration |

---

# 📦 Installation

Install all required libraries.

```bash
pip install matplotlib seaborn plotly cufflinks pandas numpy jupyter notebook
```

or

```bash
pip install -r requirements.txt
```

---

# 📥 Import Libraries

```python
import numpy as np
import pandas as pd

# Matplotlib
import matplotlib.pyplot as plt

# Seaborn
import seaborn as sns

# Plotly
import plotly.express as px
import plotly.graph_objects as go

# Cufflinks
import cufflinks as cf
from plotly.offline import init_notebook_mode

# Enable Offline Mode
init_notebook_mode(connected=True)
cf.go_offline()
```

---

# 📂 Repository Structure

```
Python-Data-Visualization/
│
├── 01_Matplotlib/
│      ├── 01_Introduction.ipynb
│      ├── 02_Line_Plot.ipynb
│      ├── 03_Bar_Plot.ipynb
│      ├── 04_Scatter_Plot.ipynb
│      ├── 05_Histogram.ipynb
│      ├── 06_Pie_Chart.ipynb
│      ├── ...
│
├── 02_Seaborn/
│      ├── 01_Introduction.ipynb
│      ├── 02_Distribution.ipynb
│      ├── 03_Categorical.ipynb
│      ├── ...
│
├── 03_Plotly/
│      ├── 01_Basics.ipynb
│      ├── 02_Interactive.ipynb
│      ├── ...
│
├── 04_Cufflinks/
│      ├── 01_Basics.ipynb
│      ├── ...
│
├── Datasets/
├── Projects/
├── Images/
├── requirements.txt
└── README.md
```

---

# 📈 Quick Matplotlib Example

```python
import matplotlib.pyplot as plt

x = [1,2,3,4,5]
y = [3,5,2,8,6]

plt.figure(figsize=(8,5))

plt.plot(
    x,
    y,
    color="blue",
    marker="o",
    linewidth=2
)

plt.title("Simple Line Plot")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.grid(True)

plt.show()
```

---

# 🌊 Quick Seaborn Example

```python
import seaborn as sns
import matplotlib.pyplot as plt

tips = sns.load_dataset("tips")

sns.scatterplot(
    data=tips,
    x="total_bill",
    y="tip",
    hue="sex"
)

plt.show()
```

---

# ⚡ Quick Plotly Example

```python
import plotly.express as px

df = px.data.iris()

fig = px.scatter(
    df,
    x="sepal_length",
    y="petal_length",
    color="species",
    title="Interactive Scatter Plot"
)

fig.show()
```

---

# 📊 Quick Cufflinks Example

```python
import pandas as pd
import cufflinks as cf

cf.go_offline()

df = pd.DataFrame({
    "Sales":[12,18,25,32,28],
    "Profit":[2,4,8,9,6]
})

df.iplot(
    kind="line",
    title="Sales Dashboard"
)
```

---

# 📚 Complete Learning Roadmap

## 📊 Module 1 — Matplotlib

### Basics

- Introduction
- Installation
- pyplot
- Figure
- Axes
- Figure vs Axes
- Plot Workflow

### Basic Charts

- Line Plot
- Scatter Plot
- Bar Plot
- Horizontal Bar Plot
- Histogram
- Pie Chart
- Area Plot
- Stem Plot
- Step Plot

### Plot Customization

- Colors
- Line Styles
- Markers
- Marker Size
- Marker Color
- Legends
- Titles
- Labels
- Grid
- Axis Limits
- Tick Formatting
- Fonts
- Themes

### Multiple Plots

- subplot()
- subplots()
- Shared Axes
- Layouts

### Advanced

- Twin Axis
- Log Scale
- Polar Charts
- Error Bars
- Contour Plot
- Heatmaps
- Box Plot
- Violin Plot
- Stack Plot
- Fill Between
- 3D Plotting
- Animation
- Saving Figures

---

## 🎨 Module 2 — Seaborn

### Basics

- Introduction
- Themes
- Color Palettes

### Relational Plots

- lineplot()
- scatterplot()
- relplot()

### Distribution Plots

- histplot()
- kdeplot()
- displot()
- rugplot()
- ecdfplot()

### Categorical Plots

- countplot()
- barplot()
- pointplot()
- boxplot()
- violinplot()
- stripplot()
- swarmplot()
- catplot()

### Matrix Plots

- Heatmap
- Correlation Matrix
- Clustermap

### Regression

- regplot()
- lmplot()

### Pairwise

- pairplot()
- PairGrid()

### Faceting

- JointPlot
- JointGrid
- FacetGrid

### Styling

- Themes
- Fonts
- Context
- Colors
- Legends

---

## ⚡ Module 3 — Plotly

### Plotly Express

- Line Chart
- Scatter Plot
- Pie Chart
- Histogram
- Box Plot
- Violin Plot
- Area Chart

### Graph Objects

- Figure
- Layout
- Traces

### Advanced

- Sunburst
- Treemap
- Funnel Chart
- Sankey Diagram
- Choropleth Maps
- 3D Scatter
- 3D Surface
- Animations
- Interactive Dashboards

---

## 📈 Module 4 — Cufflinks

- Installation
- Offline Mode
- Pandas Integration
- Line Charts
- Scatter Charts
- Histograms
- Bubble Charts
- Heatmaps
- Financial Charts
- Exploratory Data Analysis

---

# 📊 Datasets Used

- Iris
- Titanic
- Tips
- Flights
- Penguins
- Diamonds
- Netflix
- Spotify
- FIFA
- IPL
- Amazon Sales
- Superstore
- COVID-19
- House Prices
- Employee Attrition

---

# 💼 Mini Projects

- Netflix Dashboard
- Sales Dashboard
- IPL Analysis
- HR Analytics Dashboard
- Spotify Dashboard
- COVID Dashboard
- Superstore Dashboard
- Employee Attrition Dashboard
- Housing Price Visualization
- Financial Dashboard

---

# 🎯 Skills You'll Gain

✅ Exploratory Data Analysis

✅ Statistical Visualization

✅ Data Storytelling

✅ Interactive Dashboards

✅ Publication Quality Figures

✅ Business Reports

✅ Presentation Ready Charts

✅ Interview Preparation

✅ Portfolio Projects

---

# 📸 Repository Preview

```
Images/
│
├── line_plot.png
├── scatter_plot.png
├── histogram.png
├── heatmap.png
├── pairplot.png
├── dashboard.png
└── plotly_chart.png
```

You can display screenshots like:

```markdown
## Repository Preview

| Matplotlib | Seaborn |
|------------|----------|
| ![](Images/line_plot.png) | ![](Images/heatmap.png) |

| Plotly | Cufflinks |
|---------|------------|
| ![](Images/dashboard.png) | ![](Images/plotly_chart.png) |
```

---

# 📚 Recommended Learning Order

```
Python
      ↓
NumPy
      ↓
Pandas
      ↓
Matplotlib
      ↓
Seaborn
      ↓
Plotly
      ↓
Cufflinks
      ↓
Real Datasets
      ↓
Mini Projects
```

---

# 💻 Best Practices

- Write clean, readable notebooks.
- Add comments to every important section.
- Practice with multiple datasets.
- Compare different chart types.
- Focus on storytelling rather than just plotting.
- Recreate dashboards from real-world applications.

---

# 🤝 Contributions

Contributions are always welcome!

If you'd like to improve this repository:

- Fork the repository
- Create a new branch
- Commit your changes
- Submit a Pull Request

You can also open an Issue for bugs, suggestions, or new visualization ideas.

---

# ⭐ Support

If this repository helped you in your learning journey:

⭐ Star this repository

🍴 Fork it

📢 Share it with others

---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use it for learning, teaching, and personal projects.

---

<div align="center">

## 🚀 Happy Learning & Happy Coding!

### Made with ❤️ for the Python & Data Science Community

**"A picture is worth a thousand numbers."**

⭐ Star the repository if you found it useful.

</div>

