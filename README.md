# A Practise Project for matplotlib vs seaborn vs plotly

## Matplotlib
- Matplotlib is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications using general-purpose GUI toolkits like Tkinter, wxPython, Qt, or GTK.


## Seaborn
- Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.


## Plotly
- Plotly is a technical computing company headquartered in Montreal, Quebec, that develops online data analytics and visualization tools. Plotly provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python, R, MATLAB, Perl, Julia, Arduino, and REST.


### Installation
```bash
pip install matplotlib
pip install seaborn
pip install plotly
```

### Usage
```python
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
```

### Example
```python
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
    
# Matplotlib
plt.plot([1, 2, 3, 4])
plt.ylabel('some numbers')
plt.show()

# Seaborn
sns.set(style="whitegrid")
tips = sns.load_dataset("tips")
ax = sns.violinplot(x=tips["total_bill"])

# Plotly
df = px.data.iris()
fig = px.scatter(df, x="sepal_width", y="sepal_length", color="species")
fig.show()
```
