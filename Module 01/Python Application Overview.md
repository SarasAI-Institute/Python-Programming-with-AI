### Before Running any Codes

**Please run the following commands in your IDE (preferably in separate cells) and restart the session if necessary:**

```python
!pip install pandas-profiling
```
```python
!pip install spacy
```
```python
!python -m spacy download en_core_web_sm
```
```python
!pip install opencv-python
```

## 1. Python's Applications in Data Science, Data Analytics, ML, and AI

### Data Science

#### Data Manipulation and Cleaning
```python
import pandas as pd
import numpy as np

# Creating a sample DataFrame
data = {'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Eve'],
        'Age': [24, 27, 22, 32, 29],
        'Salary': [70000, 80000, 65000, 90000, 85000]}
df = pd.DataFrame(data)

# Cleaning data: Handling missing values
df['Salary'].fillna(df['Salary'].mean(), inplace=True)

# Data manipulation: Adding a new column
df['Salary_increase'] = df['Salary'] * 0.1
print(df)
```

#### Data Visualization

```python
import matplotlib.pyplot as plt
import seaborn as sns

# Sample data
tips = sns.load_dataset("tips")

# Matplotlib example
plt.figure(figsize=(8, 6))
plt.hist(tips['total_bill'], bins=20, color='skyblue')
plt.title('Distribution of Total Bill')
plt.xlabel('Total Bill')
plt.ylabel('Frequency')
plt.show()

# Seaborn example
plt.figure(figsize=(8, 6))
sns.boxplot(x='day', y='total_bill', data=tips)
plt.title('Total Bill Distribution by Day')
plt.show()
```

#### Statistical Analysis
```python
import statsmodels.api as sm
import numpy as np

# Generating sample data
np.random.seed(0)
X = np.random.rand(100)
Y = 2 * X + np.random.normal(0, 0.1, 100)

# Adding constant term to predictor
X = sm.add_constant(X)

# Fitting the regression model
model = sm.OLS(Y, X).fit()
predictions = model.predict(X)

# Model summary
print(model.summary())

```

### Data Analytics

#### Exploratory Data Analysis (EDA)
```python

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the sample dataset
df = pd.read_csv('https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv')

# Display basic information about the dataset
print(df.info())
print(df.describe(include='all'))

# Handle categorical variables using one-hot encoding
df_encoded = pd.get_dummies(df, drop_first=True)

# Correlation matrix
correlation_matrix = df_encoded.corr()

# Plotting the heatmap for the correlation matrix
plt.figure(figsize=(12, 8))
sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm')
plt.title('Correlation Matrix Heatmap')
plt.show()

# Pairplot to visualize relationships
sns.pairplot(df, hue='sex')
plt.show()

# Boxplot to visualize the distribution of total_bill across different days
plt.figure(figsize=(10, 6))
sns.boxplot(x='day', y='total_bill', data=df)
plt.title('Total Bill Distribution by Day')
plt.show()

# Histogram to visualize the distribution of total_bill
plt.figure(figsize=(10, 6))
sns.histplot(df['total_bill'], bins=20, kde=True)
plt.title('Distribution of Total Bill')
plt.xlabel('Total Bill')
plt.ylabel('Frequency')
plt.show()


```

#### Data Reporting and Dashboards

```python
import dash
import dash_core_components as dcc
import dash_html_components as html
import plotly.express as px
import pandas as pd

# Sample data
df = pd.read_csv('https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv')

# Creating a Dash app
app = dash.Dash(__name__)

# Plotly figure
fig = px.scatter(df, x='total_bill', y='tip', color='sex')

app.layout = html.Div(children=[
    html.H1(children='Tips Dashboard'),
    dcc.Graph(
        id='example-graph',
        figure=fig
    )
])

if __name__ == '__main__':
    app.run_server(debug=True)

```

### Machine Learning (ML)
#### Model Development

```python
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

# Loading the dataset
iris = load_iris()
X, y = iris.data, iris.target

# Splitting the dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)

# Training the model
clf = RandomForestClassifier(n_estimators=100)
clf.fit(X_train, y_train)

# Making predictions
y_pred = clf.predict(X_test)

# Evaluating the model
accuracy = accuracy_score(y_test, y_pred)
print(f'Accuracy: {accuracy}')

```

### Artificial Intelligence (AI)
#### Deep Learning

```python
import tensorflow as tf
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense
import numpy as np

# Generating sample data
X = np.random.rand(1000, 10)
y = np.random.randint(2, size=(1000, 1))

# Defining the model
model = Sequential([
    Dense(32, activation='relu', input_shape=(10,)),
    Dense(32, activation='relu'),
    Dense(1, activation='sigmoid')
])

# Compiling the model
model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])

# Training the model
model.fit(X, y, epochs=10, batch_size=32)

# Evaluating the model
loss, accuracy = model.evaluate(X, y)
print(f'Accuracy: {accuracy}')

```

#### Natural Language Processing (NLP)

```python
import spacy

# Loading the English model
nlp = spacy.load('en_core_web_sm')

# Processing a text
doc = nlp("Apple is looking at buying U.K. startup for $1 billion.")

# Extracting entities
entities = [(ent.text, ent.label_) for ent in doc.ents]
if entities:
    for entity in entities:
        print(entity[0], entity[1])
else:
    print("No entities found")

```

#### Computer Vision

```python

import cv2
import matplotlib.pyplot as plt
import urllib.request
import numpy as np

# URL of the image
url = 'https://upload.wikimedia.org/wikipedia/commons/4/47/PNG_transparency_demonstration_1.png'

# Download the image
resp = urllib.request.urlopen(url)
image = np.asarray(bytearray(resp.read()), dtype="uint8")
img = cv2.imdecode(image, cv2.IMREAD_COLOR)

# Check if the image is loaded
if img is None:
    print("Error: Could not load image.")
else:
    # Converting to grayscale
    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

    # Detecting edges
    edges = cv2.Canny(gray, 100, 200)

    # Displaying the image using matplotlib
    plt.figure(figsize=(10, 5))

    plt.subplot(1, 2, 1)
    plt.title('Grayscale Image')
    plt.imshow(gray, cmap='gray')

    plt.subplot(1, 2, 2)
    plt.title('Edges Detected')
    plt.imshow(edges, cmap='gray')

    plt.show()


```
