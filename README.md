# project
Machine learning with Apache Spark.

## Description

Use Apache Spark to explore and analyse a sample dataset for simple machine learning.

Below are your goals on this assignment.

1. Explore configuration options on SparkSession
2. Reading the data
3. Performing Tasks
    - Explore or transform the data with Spark SQL and/ or Spark DataFrame
    - Apply machine learning and compare models.
4. Present your findings to your audience with a brief presentation

**Your notebook** should contain your code, code output, and markdown text that briefly describes the code when necessary. Use headings, subheadings to organize your notebook. Remember, your notebook is your selling point of your project, anyone interested in your project should be able to:

- run the notebook and reproduce your outputs.
- when showing results, show only a few rows rather than printing entire dataset.
- should have headings, subheadings to understand which part we are reading.
- should have a conclusion.

**Your presentation** should be brief, less than 10 minutes, and each member of your group should involve in presenting. Your objective in presentation is below.

- briefly introduce your dataset
- show your exploratory data analysis results
- show your models, explain why you choose these models, and show comparison of the models.

While doing this, try showcasing below steps to complete your project. 

### EDA

- Read data as RDD.
- Read data as DataFrame.
- Convert RDD to Spark DataFrame.
- Convert Spark DataFrame to RDD.
- Convert Spark DataFrame to Pandas DataFrame.
- Create a plot on a categorical column.

### Transformations

- Do a groupby transformation on a column, show count or average.
- Select a column to do a replacement operation (`str.replace('a', '')`). Even if this doesn't fit your data, try examplifying it.
- Do at least one transformation with RDD.
- Transform a categorical column with OneHot Encoding.

### Use of Spark SQL

- Create a temp view of your dataset to be able to use Spark SQL.
- Group by and get max, min, count of a column in the dataset.
- Select distinct records by a column.

### Machine Learning

- Create `X` for features from your dataset, and `y` for labels if you have any.
- Apply 2 machine learning models on your dataset, and pick the best one as your model.
- Show appropriate statistics on your model.

## Hints

If using Google Colab, attach Google drive to Google Colab.

``` py
from google.colab import drive
drive.mount('/content/drive')
```

Create a temp table in Spark. 

``` py
spark_df.createOrReplaceTempView("some_table")
```

Use `.take()` or `.first()` instead of `.collect()`.

``` py
rdd.take(2)
```

## Dataset

Use any dataset that is *more than 1000 rows*, has **both categorical and numerical** values.

Some places you can find datasets from:

- [Data World](https://data.world/datasets/open-data)
- [Google Datasets](https://datasetsearch.research.google.com/)
- [UCI Machine Learning Library](https://archive.ics.uci.edu/ml/datasets.php)

## How to work on this Assignment?

1. Download this repository with `git clone https://github.com/spu-bigdataanalytics-211/project`.
2. [Create a virtual environment](https://github.com/spu-bigdataanalytics-211/class-materials#how-to-create-a-new-virtual-environment) and activate this environment everytime you need to use it.
3. Install [requirements.txt](requirements.txt) file using `pip install -r requirements.txt`.
4. Create a notebook.

## Questions

The repository should be self descriptive and it should guide you through assignment. Let me know if you have any questions.
