```markdown
# In-Class Exploratory Data Analysis (EDA)

This repository is part of the **SPU-F1-2026 GitHub Classroom** and is designed to provide hands-on practice with **Exploratory Data Analysis (EDA)** and data visualization using Python.

GitHub Classroom Organization:  
https://github.com/SPU-F1-2026

Repository:  
https://github.com/SPU-F1-2026/In-Class-EDA.git

---

## Table of Contents

- [Description](#description)
- [Learning Objectives](#learning-objectives)
- [Datasets](#datasets)
- [Visualization Libraries](#visualization-libraries)
- [How to Work on This Repository](#how-to-work-on-this-repository)
- [Presentation Expectations](#presentation-expectations)
- [Questions](#questions)

---

## Description

In this in-class exercise, you will practice **Exploratory Data Analysis (EDA)** using Python.

The objective is to examine datasets through descriptive statistics and visualizations in order to identify:

- Patterns and trends
- Relationships between variables
- Distributions
- Correlations
- Outliers
- Potential anomalies
- Meaningful insights that may not be immediately visible from the raw data

You should use Python visualization techniques to communicate your findings clearly and professionally.

Select **any three datasets** available through `plotly.data` and perform exploratory analysis on each dataset.

Your notebook should be organized, reproducible, and self-explanatory.

---

## Learning Objectives

By completing this exercise, you should be able to:

- Load and inspect datasets using Python
- Understand dataset structure, dimensions, and data types
- Perform basic descriptive statistical analysis
- Identify missing values and potential data-quality issues
- Analyze numerical and categorical variables
- Explore relationships between multiple features
- Create appropriate statistical and analytical visualizations
- Interpret patterns, distributions, correlations, and outliers
- Communicate analytical findings through a well-structured Jupyter Notebook

---

## Datasets

You do **not** need to manually download the datasets.

Plotly provides several built-in datasets that can be loaded directly from Python.

```python
from plotly import data

iris = data.iris()
carshare = data.carshare()
election = data.election()
tips = data.tips()
gapminder = data.gapminder()
wind = data.wind()
```

You may inspect the available datasets before selecting the three you would like to analyze.

For example:

```python
from plotly import data

df = data.iris()

df.head()
```

You should also examine the structure of your selected datasets using commands such as:

```python
df.shape
df.columns
df.info()
df.describe()
df.isnull().sum()
```

---

## Visualization Libraries

You may use any appropriate Python visualization library, including:

- `matplotlib`
- `seaborn`
- `plotly`
- `bokeh`

You are encouraged to use more than one visualization technique when appropriate.

Examples may include:

- Histograms
- Bar charts
- Scatter plots
- Box plots
- Violin plots
- Line charts
- Correlation heatmaps
- Pair plots
- Interactive Plotly visualizations

Your choice of visualization should support the analytical question you are investigating.

---

## How to Work on This Repository

### 1. Clone the Repository

Open your terminal, Git Bash, or the integrated terminal in Visual Studio Code and run:

```bash
git clone https://github.com/SPU-F1-2026/In-Class-EDA.git
```

Navigate into the repository:

```bash
cd In-Class-EDA
```

---

### 2. Create a Python Virtual Environment

Creating a dedicated virtual environment is strongly recommended.

Using Python:

```bash
python -m venv .venv
```

Activate the environment.

#### Windows

```bash
.venv\Scripts\activate
```

#### macOS / Linux

```bash
source .venv/bin/activate
```

If you are using Anaconda or Miniconda, you may instead create a Conda environment:

```bash
conda create -n eda python=3.11 -y
conda activate eda
```

---

### 3. Install the Required Packages

If the repository contains a `requirements.txt` file, install the dependencies using:

```bash
pip install -r requirements.txt
```

If necessary, the core packages may also be installed manually:

```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

---

### 4. Open the Jupyter Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Alternatively, you may work directly inside **Visual Studio Code** using the Jupyter extension.

Open the notebook included in the repository and complete the required EDA exercises.

---

### 5. Perform Exploratory Data Analysis

For each of your three selected datasets, your analysis should include appropriate exploration of the following areas:

- Dataset dimensions
- Column names
- Data types
- Missing values
- Descriptive statistics
- Numerical-variable distributions
- Categorical-variable distributions
- Relationships between variables
- Correlations where appropriate
- Outliers or unusual observations
- Relevant visualizations
- Interpretation of findings

Do not simply generate charts.

Each important visualization should be accompanied by a brief explanation of **what the visualization reveals about the data**.

---

### 6. Save and Commit Your Work

Save your notebook and verify that all cells execute successfully.

Check your repository status:

```bash
git status
```

Stage your changes:

```bash
git add .
```

Create a meaningful commit:

```bash
git commit -m "Complete in-class exploratory data analysis"
```

If your repository is connected to GitHub, push your work:

```bash
git push
```

---

## Presentation Expectations

You should be prepared to briefly present your notebook during class.

The presentation should be approximately **5–10 minutes** and should focus on:

1. The datasets you selected
2. The analytical questions you explored
3. The visualizations you created
4. The most important patterns or relationships you discovered
5. Your overall conclusions

The objective is not merely to display charts, but to explain the **story revealed by the data**.

---

## Repository Quality Expectations

Your repository and notebook should be:

- Clearly organized
- Professionally presented
- Reproducible
- Properly documented
- Free of unnecessary code
- Free of unresolved execution errors
- Easy for another person to follow

Before completing the exercise, restart the notebook kernel and run all cells from beginning to end to verify that the notebook executes successfully.

---

## Questions

The repository and notebook instructions should guide you through the exercise.

If you encounter technical problems involving:

- Git or GitHub
- Python environments
- Jupyter Notebook
- Package installation
- Plotting libraries
- Dataset loading

document the error message and bring it to class for troubleshooting.

**Best of luck, and focus on explaining what the data is telling you.**
```