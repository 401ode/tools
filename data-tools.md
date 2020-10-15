# Data Tools

## General Resources

- [Quartz Guide to Bad Data](https://github.com/Quartz/bad-data-guide) - The title says it all, but it also provides intellectual guidance on how to resolve common data problems.
- [PolicyViz](https://policyviz.com/) - "Helping you do a better job processing, analyzing, sharing, and presenting your data." There's a podcast, and tons of guides on visualization, presentation, etc.

## Python-based Tools

- [Pandas](http://pandas.pydata.org/) - included with [Anaconda](https://www.continuum.io/downloads) distribution. Gold Standard for Data Analysis, Data Science.
- [Learn Pandas by Studying COVID-19 Data](https://www.fullstackpython.com/blog/learn-pandas-basic-commands-explore-covid-19-data.html) - Pretty self-explanatory, but a very nice walkthrough using an important datasource.
- [Pandas Crosstab Explained](http://pbpython.com/pandas-crosstab.html) - A great reference article from [Practical Business Python](http://pbpython.com/) (an EXCELLENT site) on Panda's [Crosstab](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.crosstab.html) functionality. Basically if you want to take element A, and then find how many time instances of element B show up with it, Crosstab is perfect. Just one simple command. Really useful.
- [Great list of Pandas Examples by Solution](http://www.pythonprogramming.in/pandas-examples.html) - Too many to list, really, but I'll try:

```
- Creating a Series using List and Dictionary
- Create series using NumPy functions
- Get index and values of a series
- Specify an Index at Series creation
- Get Length Size and Shape of a Series
- Slicing a Series into subsets
- Example of Heads, Tails and Takes
- Create and Print DataFrame
- Set Index and Columns of DataFrame
- Rename DataFrame Columns
- select rows from a DataFrame using operator
- Filter DataFrame rows using isin
- Example of iterrows and itertuples
- Drop DataFrame Column(s) by Name or Index
- Add new column to DataFrame
- Get list of the column headers
- Generate DataFrame with random values
- Select multiple columns from DataFrame
- Convert Dictionary into DataFrame
- DataFrame slicing using loc
- DataFrame is empty
- Specify Index and Column for DataFrame
- DataFrame slicing using iloc
- loc vs iloc slicing in DataFrame
- Empty DataFrame with Date Index
- Reindex DataFrame columns
- Determine DataFrame columns data type
- Change DataFrame column data type from Int64 to String
- Change DataFrame column data-type from UnixTime to DateTime
- Alter DataFrame column data type from Float64 to Int32
- Alter DataFrame column data type from Object to Datetime64
- Appending two DataFrame objects
- Add row at end
- Add row with specific index name
- Append rows using a for loop
- Add a row at top
- Dynamically Add Rows to DataFrame
- Insert a row at an arbitrary position
- Adding row to DataFrame with time stamp index
- Adding rows with different column names
- Example of append, concat and combine_first
- Get mean(average) of rows and columns
- Calculate sum across rows and columns
- Join two columns
- Filter rows which contain specific keyword
- Filtering DataFrame Index
- Filtering DataFrame with an AND operator
- Find all rows contain a Sub-string
- Example of where()
- Count number of rows per group
- Example of using any()
- Get Unique row values
- Count Distinct Values
- Remove duplicate rows
- Remove duplicate rows based on two columns
- Get value of a specific cell
- Get scalar value of a cell using conditional indexing
- Remove duplicate rows
- Get list of cell value conditionally
- Replace values in column with a dictionary
- Count distinct equivalent
- Handle missing data
- Delete missing data rows
- Drop columns with missing data
- Sort Index in descending order
- Sort Column in descending order
- Determine Rank of DataFrame values
- Multiple Indexing
- Determine Period Index and Column for DataFrame
- Determine Period Range with Frequency
- Import CSV with specific Index
- Writing DataFrame to CSV file
- Read specific columns from CSV
- Get list of CSV columns
- Find row where values for column is maximum
- Complex filter data using query method
- Check if one or more columns all exist
- Locating the n-smallest and n-largest values
- Finding minimum and maximum values
- Find index position of minimum and maximum values
- Calculation of a cumulative product and sum
- Summary statistics of DataFrame
- Find Mean, Median and Mode
- Measure Variance and Standard Deviation
- Calculating Co-variance
- Calculating correlation between two DataFrame
- Calculating the percent change at each cell of a DataFrame
- Forward and backward filling of missing values
- Stacking using non-hierarchical indexes
- Unstacking using hierarchical indexes
```

- [RealPython Article on Pandas Optimizations](https://realpython.com/fast-flexible-pandas/) - Good overview of how to thing about how to optimize your work in Pandas.
- [PythonSpeed Article on Using SQLite and Pandas Indices for Efficient Querying and Filtering](https://pythonspeed.com/articles/indexing-pandas-sqlite/) - TL;DR: SQLite is FAST and kind of awesome. In this instance, 50x faster than reading/querying a CSV that's too big to fit in memory.
- [MessyTables - "All Your Rows Are Belong To Us"](https://messytables.readthedocs.io/en/latest/) - "Tabular data as published on the web is often not well formatted and structured. Messytables tries to detect and fix errors in the data. Typical examples include: Finding the header of a table when there are explanations and text fragments in the first few rows of the table; Guessing the type of columns in CSV data; Guessing the format of a byte stream. This library provides data structures and some heuristics to fix these problems and read a wide number of different tabular abominations." **Pretty cool.**
- [Article on 'Tidy Data' in Python](http://www.jeannicholashould.com/tidy-data-in-python.html) - Interesting thoughts on how to clean and structure data.
- [Numba - The need for speed without bothering too much](https://nbviewer.jupyter.org/github/akittas/presentations/blob/master/pythess/numba/numba.ipynb?utm_source=newsletter_mailer&utm_medium=email&utm_campaign=weekly#The-need-for-speed-without-bothering-too-much:-An-introduction-to-numba) - These guys are genius. They basically made it super-simple to radically increase the speed of what you're doing in Pandas or Numpy arrays (which is what Pandas uses under the hood). Very excited about this. Basically if you tell it about a specific function or thing you're trying to do, it'll compile to low-level C-code. Some average improvements by adding **one line of code** are around **78 times faster.** Awesome.
- [Cookiecuttter Data Science](https://drivendata.github.io/cookiecutter-data-science/) - Uses [Cookiecutter](http://cookiecutter.readthedocs.org/en/latest/installation.html) to set up a nice, version-controlled data analysis directory for tracking your whole project.
- [Kedro](https://github.com/quantumblacklabs/kedro) - Another cookiecutter data science setup that is getting a lot of buzz. Apparently great at setting up reusable data pipelines. Particularly cool is its ability to generate graphical diagrams of said pipelines.
- [Dask](https://dask.pydata.org/en/latest/) - Rather than load your enormous Pandas Dataframe into memory, Dask takes kind of a streaming approach to process iteratively but more efficiently for large datasets.
- [RapidFuzz](https://github.com/rhasspy/rapidfuzz) - Extremely fast Python package for comparing text similarity in various capacities. The classic example is comparing "BOS Celtics v. LA Lakers" and "Los Angeles Lakers and Boston Celtics"

## Python Tutorials

- While we may compile our own list at some point, [this](https://nealcaren.github.io/python-tutorials/) is a fantastic compendium of available Python data-science tutorials.

## Optical Character Recognition (OCR)

- [Google Drive](https://support.google.com/drive/answer/176692) works quite well for basic applications.
- [Tesseract](https://github.com/tesseract-ocr/tesseract) - this is a !@#$$!@#$ and a half to get working, but it's incredibly powerful once you get it installed. Next time I'm going to try getting it working in a [Docker](devops.md) container and forget about it.
- TODO - Links to PyOCR, other Python tesseract libraries.
- [OCRopus](https://github.com/tmbdev/ocropy)

## Visualization Tools

We'll be migrating in some from this [list (Google Doc)](https://docs.google.com/spreadsheets/d/1zkDKbi144mrDl7NSPMTRKyjdX8qfiL8MSlUw2z_dEIE/edit?usp=drivesdk).

- [FLourish](https://flourish.studio/) - Web-based data visualization tool that makes it easy to do things like [bar chart races](https://flourish.studio/visualisations/bar-chart-race/?utm_source=showcase&utm_campaign=visualisation/3835611). 

## Generic BI/Reporting Tools

- [Microsoft PowerBI](https://powerbi.microsoft.com) - For a Microsoft tool, this is surprisingly good, stable, extendable, and easy to use. I can't believe I just wrote that.
- [Tableau](https://www.tableau.com/) - Desktop version is free, as long as you publish your data/visualization.

### Python DataViz Tools

- [MatPlotLib](http://matplotlib.org/) - The original behemoth of DataViz tools.
- [Seaborn](https://seaborn.pydata.org/) - Makes opinionated decisions for you on MatPlotLib settings, makes the MatPlotLib API much easier to use.
- [Dash](https://plot.ly/products/dash/) - For easy, interactive visualizations. Very cool.
- [Apache Superset](https://github.com/apache/incubator-superset) - Gorgeous-looking, open-source data visualization and dashboard tool. Uses Python library [SQLAlchemy](http://docs.sqlalchemy.org/en/rel_1_0/core/engines.html) under the hood, allowing it to connect to an enormous number of database engines.
- [University of Potsdam Summer Class on Information Visualization Using Python](https://infovis.fh-potsdam.de/tutorials/) - Well, that about says it. But it looks like a great, comprehensive course. Also, it's *free*.

## ~~Robots~~ Machine Learning

- [TensorFlow](https://www.tensorflow.org/) - When robots take over the world, this will be the core of their DNA. TensorFlow is the principal Google Artificial Intelligence / Machine Learning library. They open-sourced it a few years ago. It's generally considered the most powerful in the world. There are APIs for Python and tons of other languages now.
- [Keras](https://keras.io/) - An overall neural network API, but basically it makes interacting with TensorFlow way easier. See this nice [DataCamp Tutorial](https://www.datacamp.com/community/tutorials/deep-learning-python).
- [Setting up Python for Machine Learning on Windows](https://realpython.com/python-windows-machine-learning-setup/) - a great [RealPython](https://realpython.com/) article that is exactly what the title describes.
- [fastText - Facebook's Text Classification and Representation Learning](https://fasttext.cc/) - "The goal of text classification is to assign documents (such as emails, posts, text messages, product reviews, etc...) to one or multiple categories. Such categories can be review scores, spam v.s. non-spam, or the language in which the document was typed. Nowadays, the dominant approach to build such classifiers is machine learning, that is learning classification rules from examples. In order to build such classifiers, we need labeled data, which consists of documents and their corresponding categories (or tags, or labels)."
- [Prophet - Time Series Prediction from Facebook](https://facebook.github.io/prophet/) - "Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well." It's dead interesting and pretty easy to use. [PBP](https://pbpython.com/) has an [interesting overview article](https://pbpython.com/prophet-overview.html), along with an [update looking at the accuracy of the predictions](https://pbpython.com/prophet-accuracy.html).

## Data Mapping

- [YWorks](https://www.yworks.com/products/yed)
- [The Brain](http://www.thebrain.com/) - Like a Dumbledorean Pensieve, but digital.
- [Orange](https://orange.biolab.si/)
- [KNIME](https://www.knime.com/) - An open-source-based GUI for fairly sophisticated data manipulation, processing, and visualization. And it's even approved for production usage by State security staff.

## Data Quality Tools

- [Open Refine](http://openrefine.org/) - Great data cleanup platform.
- [Talend Data Preparation (Free Desktop Edition)](https://www.talend.com/products/data-preparation/) - Good GUI tool to analyze and clean data.
- [Dora](https://github.com/NathanEpstein/Dora) - "Dora is a Python library designed to automate the painful parts of exploratory data analysis. The library contains convenience functions for data cleaning, feature selection & extraction, visualization, partitioning data for model validation, and versioning transformations of data."
- [Scrubadub](https://scrubadub.readthedocs.io/en/stable/index.html) - Automatically removes sensitive data (PII, etc.) from datasets.

## General

- [Transformy](https://www.transformy.io/#/)
- [Datazar](https://www.datazar.com)
- [Diggernaut](https://www.diggernaut.com/) - Web scraping service.

## Text / Document Manipulation Tools

- [Pandoc](http://www.pandoc.org) - Amazing command line tool for converting documents between many different formats. For example, if you want to change a Word doc to a markdown file, you would run `pandoc -f docx -t markdown -o outputmarkdownfile.md sourcedocument.docx`.
- [Camelot](https://github.com/socialcopsdev/camelot) - A Python-based PDF table extraction tool. Pretty slick!
- [Excalibur] - A web interface for Camelot.
- [Tabula](https://tabula.technology/) - Amazing tool for extracting tabular data out of PDFs. Works like a charm, pretty much every time.

## Version Controlled Data

- [Dolt](https://www.dolthub.com/) - Git for Data
- [qri](https://qri.io/) - qri (“query”) is versioned, scriptable, exportable, collaborative datasets


## Database Viewers
- [Hedi](https://www.heidisql.com/)
- [Postico](https://eggerapps.at/postico/)
- [TablePlus](https://tableplus.com/)

