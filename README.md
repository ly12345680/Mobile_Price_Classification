# Mobile Price Classification

## Overview

This study describes the creation of a mobile phone pricing categorization model based on three machine learning methods: Support Vector Machine (SVM), Decision Tree, and Random Forest. 

## Requirements

List the requirements for running your project. This could include things like:

- Python 3.11
- Libraries: numpy, seaborn, matplotlib, sklearn, plotly, pandas

## Installation
- Carefully import train dataset directory
- Run step by step to gain results

## Dataset Description

- **Total Records**: 2000 mobile phones
- **Total Variables**: 21
  - **Categorical Variables**: 8 (n_cores, price_range, blue, dual_sim, four_g, three_g, touch_screen, wifi)
  - **Numeric Variables**: 13 (battery_power, clock_speed, fc, int_memory, m_dep, mobile_wt, pc, px_height, px_width, ram, talk_time, sc_h, sc_w)
- **Missing Values**: None

### Categorical Variables

- `n_cores`: Number of cores
- `price_range`: Price range (dependent variable)
- `blue`: Presence of Bluetooth (1 or 0)
- `dual_sim`: Presence of dual SIM (1 or 0)
- `four_g`: Supports 4G (1 or 0)
- `three_g`: Supports 3G (1 or 0)
- `touch_screen`: Touch screen (1 or 0)
- `wifi`: Supports WiFi (1 or 0)

### Numeric Variables

- `battery_power`: Battery power in mAh
- `clock_speed`: Clock speed in GHz
- `fc`: Front camera megapixels
- `int_memory`: Internal memory in GB
- `m_dep`: Mobile depth in cm
- `mobile_wt`: Weight of the mobile phone
- `pc`: Primary camera megapixels
- `px_height`: Pixel resolution height
- `px_width`: Pixel resolution width
- `ram`: RAM in MB
- `talk_time`: Talk time in hours
- `sc_h`: Screen height of the mobile in cm
- `sc_w`: Screen width of the mobile in cm

## Notebook Structure

The notebook includes the following sections:

1. **Open Data**: Loading and initial exploration of the dataset.
2. **Describe**: Detailed description and summary statistics of the dataset.
3. **Statistical Description of Categorical Variables**: Analysis and visualization of categorical variables.
4. **Statistical Description of Numeric Variables**: Analysis and visualization of numeric variables.
5. **Correlation Analysis**: Analyzing the correlation between different variables.
6. **Data Visualization**: Various plots and charts to visualize the dataset.
7. **Model Building**: Building and evaluating machine learning models based on the dataset.
8. **Model Evaluation**: Assessing the performance of the machine learning models.

## Models

The following machine learning models are used in this notebook:

- **Support Vector Machine (SVM)**
- **Decision Tree Classifier**
- **Random Forest Classifier**

Example code snippet for model building:

```python
from sklearn.svm import SVC
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier

# Example model instantiation
svm_model = SVC()
dt_model = DecisionTreeClassifier()
rf_model = RandomForestClassifier()

# Example model training
svm_model.fit(X_train, y_train)
dt_model.fit(X_train, y_train)
rf_model.fit(X_train, y_train)


## Contributing
Nguyễn Hoàng Lý - ITITIU20249
Trịnh Thị Như Quỳnh - ITITIU20201
Nguyễn Đỗ Tú Vy - ITITIU20125

