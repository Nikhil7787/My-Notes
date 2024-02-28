# Seaborn

## Types of plots in Seaborn Library that are commonly used. 

### 1. Scatter Plot:

**Purpose**: To visualize the relationship between two continuous variables. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot scatter plot
sns.scatterplot(x='sepal_length', y='sepal_width', data=df)
plt.title('Scatter Plot')
plt.xlabel('Sepal Length')
plt.ylabel('Sepal Width')
plt.show()
```

### 2. Line Plot

**Purpose:** To visualize the trend of a continuous variable over a continuous or categorical variable. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot line plot
sns.lineplot(x='petal_length', y='petal_width', data=df)
plt.title('Line Plot')
plt.xlabel('Petal Length')
plt.ylabel('Petal Width')
plt.show()
```

### 3. Histogram

**Purpose:** To visualize the distribution of a single continuous variable. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot histogram
sns.histplot(x='sepal_length', data=df, kde=True)
plt.title('Histogram')
plt.xlabel('Sepal Length')
plt.show()
```
### 4. Bar Plot:

**Purpose:** To visualize the distribution of a categorical variable or to compare values across different categories. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot bar plot
sns.barplot(x='species', y='sepal_width', data=df)
plt.title('Bar Plot')
plt.xlabel('Species')
plt.ylabel('Sepal Width')
plt.show()
```

### 5. Box Plot:

**Purpose:** To visualize the distribution of a continuous variable across different categories and identify outliers. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot box plot
sns.boxplot(x='species', y='petal_length', data=df)
plt.title('Box Plot')
plt.xlabel('Species')
plt.ylabel('Petal Length')
plt.show()
```

### 6. Violin Plot:

**Purpose:** To visualize the distribution of a continuous variable or the comparison of distributions across different categories. It combines features of box plots and kernel density estimation. </br>
**Steps to Plot:**


```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot violin plot
sns.violinplot(x='species', y='petal_width', data=df)
plt.title('Violin Plot')
plt.xlabel('Species')
plt.ylabel('Petal Width')
plt.show()
```


### 7. Pair Plot

**Purpose:** To visualize the pairwise relationships between multiple variables in a dataset. </br>
**Steps to Plot:**

```
import seaborn as sns

# Load data
df = sns.load_dataset('iris')

# Plot pair plot
sns.pairplot(df, hue='species')
plt.title('Pair Plot')
plt.show()
```

### 8. Heatmap:

**Purpose:** To visualize the correlation between variables in a dataset or to represent a 2D dataset. </br>
**Steps to Plot:**

```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Compute correlation matrix
corr = df.corr()

# Plot heatmap
sns.heatmap(corr, annot=True, cmap='coolwarm')
plt.title('Heatmap')
plt.show()
```

### 9. Joint Plot:

**Purpose:** To visualize the relationship between two variables along with their individual distributions. </br>
**Steps to Plot:**

```
import seaborn as sns

# Load data
df = sns.load_dataset('iris')

# Plot joint plot
sns.jointplot(x='sepal_length', y='sepal_width', data=df, kind='scatter')
plt.title('Joint Plot')
plt.show()
```

### 10. KDE Plot:

**Purpose:** To visualize the distribution of a single variable or the comparison of distributions across different categories using kernel density estimation. </br>
**Steps to Plot:**
```
import seaborn as sns
import matplotlib.pyplot as plt

# Load data
df = sns.load_dataset('iris')

# Plot KDE plot
sns.kdeplot(data=df['petal_length'], shade=True)
plt.title('KDE Plot')
plt.xlabel('Petal Length')
plt.show()
```
<br>
<br>
<br>
<br>

## Interview Questions 

### 1.	What is Seaborn?</br>
▶️ Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics. </br>


### 2.	How do you install Seaborn?</br>
▶️ You can install Seaborn using pip: pip install seaborn.</br>


### 3.	What kind of plots can Seaborn generate? </br>
▶️ Seaborn can generate various types of plots including scatter plots, line plots, bar plots, histograms, box plots, violin plots, heatmap, etc. </br>


### 4.	How do you import Seaborn? </br>
▶️ You can import Seaborn using: import seaborn as sns. </br>


### 5.	How do you create a scatter plot using Seaborn? </br>
▶️ You can create a scatter plot using the sns.scatterplot() function. </br>


### 6.	What is the purpose of the hue parameter in Seaborn plots?</br>
▶️ The hue parameter allows you to color the plot elements based on a categorical variable, adding an extra dimension to the visualization. </br>


### 7.	How do you create a bar plot in Seaborn? </br>
▶️ You can create a bar plot using the sns.barplot() function. </br>


### 8.	What is the difference between a bar plot and a count plot in Seaborn? </br>
▶️ A bar plot displays the mean of a numeric variable for each category, while a count plot shows the count of observations in each category. </br>


### 9.	How do you create a box plot in Seaborn? </br>
▶️ You can create a box plot using the sns.boxplot() function. </br>


### 10.	How can you customize the color palette in Seaborn? </br>
▶️ You can customize the color palette using the sns.set_palette() function or by specifying the palette parameter in individual plotting functions. </br>


### 11.	What is a violin plot in Seaborn? </br>
▶️ A violin plot is similar to a box plot but also shows the probability density of the data at different values. </br> 


### 12.	How do you create a heatmap in Seaborn?  </br>
▶️ You can create a heatmap using the sns.heatmap() function. </br>


### 13.	What does the annot parameter do in Seaborn's heatmap? </br>
▶️ The annot parameter in Seaborn's heatmap controls whether to annotate each cell with the numeric value or not. </br>


### 14.	How do you create a pair plot in Seaborn? </br>
▶️ You can create a pair plot using the sns.pairplot() function. </br>


### 15.	What is the purpose of the hue parameter in a pair plot? </br>
▶️ The hue parameter in a pair plot allows you to color the scatter plot points based on a categorical variable. </br>


### 16.	How do you create a joint plot in Seaborn? </br>
▶️ You can create a joint plot using the sns.jointplot() function. </br>


### 17.	What types of joint plots are available in Seaborn? </br>
▶️ Seaborn provides scatter plots (kind='scatter'), hexbin plots (kind='hex'), and kernel density estimation plots (kind='kde') for joint plots. </br>


### 18.	How do you customize the size of plots in Seaborn? </br>
▶️ You can customize the size of plots using the plt.figure(figsize=(width, height)) function from matplotlib before creating the plot. </br>


### 19.	What is the purpose of the size parameter in Seaborn's plotting functions? </br>
▶️ The size parameter allows you to adjust the size of elements in the plot, such as markers or lines. </br>


### 20.	How do you save a Seaborn plot as an image file? </br>
▶️ You can save a Seaborn plot as an image file using the plt.savefig('filename.png') function from matplotlib. </br>


### 21.	How do you create a facet grid in Seaborn? </br>
▶️ You can create a facet grid using the sns.FacetGrid() function. </br>


### 22.	What is the purpose of the col and row parameters in a facet grid? </br>
▶️ The col and row parameters allow you to create subplots based on the values of categorical variables. </br>


### 23.	How do you create a line plot in Seaborn?</br>
▶️ You can create a line plot using the sns.lineplot() function. </br>


### 24.	What is the purpose of the style parameter in Seaborn's plotting functions? </br>
▶️ The style parameter allows you to control the style of the plot elements, such as markers or lines. </br>


### 25.	How do you create a regression plot in Seaborn? </br>
▶️ You can create a regression plot using the sns.regplot() function. </br>


### 26.	What is the purpose of the ci parameter in Seaborn's regression plot? </br>
▶️ The ci parameter controls the size of the confidence interval to be drawn around the regression line. </br>


### 27.	How do you create a KDE plot in Seaborn? </br>
▶️ You can create a KDE plot using the sns.kdeplot() function. </br>


### 28.	What is the purpose of the shade parameter in Seaborn's KDE plot? </br>
▶️ The shade parameter controls whether to shade the area under the KDE curve. </br>


### 29.	How do you create a swarm plot in Seaborn? </br>
▶️ You can create a swarm plot using the sns.swarmplot() function. </br>


### 30.	What is the purpose of the dodge parameter in Seaborn's swarm plot? </br>
▶️ The dodge parameter allows you to separate the points for different categorical variables along the categorical axis. 

