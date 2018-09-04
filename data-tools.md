# Data Tools

## Python-based Tools

- [Pandas](http://pandas.pydata.org/) - included with [Anaconda](https://www.continuum.io/downloads) distribution. Gold Standard for Data Analysis, Data Science. 
    + TODO [Pandas Tutorial]
    + TODO [Pandas Tips & Tricks]
    - [RealPython Article on Pandas Optimizations](https://realpython.com/fast-flexible-pandas/) - Good overview of how to thing about how to optimize your work in Pandas. 
- [Numba - The need for speed without bothering too much](https://nbviewer.jupyter.org/github/akittas/presentations/blob/master/pythess/numba/numba.ipynb?utm_source=newsletter_mailer&utm_medium=email&utm_campaign=weekly#The-need-for-speed-without-bothering-too-much:-An-introduction-to-numba) - These guys are genius. They basically made it super-simple to radically increase the speed of what you're doing in Pandas or Numpy arrays (which is what Pandas uses under the hood). Very excited about this. Basically if you tell it about a specific function or thing you're trying to do, it'll compile to low-level C-code. Some average improvements by adding **one line of code** are around **78 times faster.** Awesome. 
- [Dask](https://dask.pydata.org/en/latest/) - Rather than load your enormous Pandas Dataframe into memory, Dask takes kind of a streaming approach to process iteratively but more efficiently for large datasets. 

## Python Tutorials

- While we may compile our own list at some point, [this](https://nealcaren.github.io/python-tutorials/) is a fantastic compendium of available Python data-science tutorials.

## Optical Character Recognition (OCR)

- [Google Drive](https://support.google.com/drive/answer/176692) works quite well for basic applications.
- [Tesseract](https://github.com/tesseract-ocr/tesseract) - this is a !@#$$!@#$ and a half to get working, but it's incredibly powerful once you get it installed. Next time I'm going to try getting it working in a [Docker](devops.md) container and forget about it.
- TODO - Links to PyOCR, other Python tesseract libraries.
- [OCRopus](https://github.com/tmbdev/ocropy)

## Visualization Tools

We'll be migrating in some from this [list (Google Doc)](https://docs.google.com/spreadsheets/d/1zkDKbi144mrDl7NSPMTRKyjdX8qfiL8MSlUw2z_dEIE/edit?usp=drivesdk).

## Generic BI/Reporting Tools

- [Microsoft PowerBI](https://powerbi.microsoft.com) - For a Microsoft tool, this is surprisingly good, stable, extendable, and easy to use. I can't believe I just wrote that.
- [Tableau](https://www.tableau.com/) - Desktop version is free, as long as you publish your data/visualization.

### Python DataViz Tools

- [MatPlotLib](http://matplotlib.org/) - The original behemoth of DataViz tools. 
- [Seaborn](https://seaborn.pydata.org/) - Makes opinionated decisions for you on MatPlotLib settings, makes the MatPlotLib API much easier to use. 
- [Dash](https://plot.ly/products/dash/) - For easy, interactive visualizations. Very cool. 
- [Apache Superset](https://github.com/apache/incubator-superset) - Gorgeous-looking, open-source data visualization and dashboard tool. Uses Python library [SQLAlchemy](http://docs.sqlalchemy.org/en/rel_1_0/core/engines.html) under the hood, allowing it to connect to an enormous number of database engines. 


## ~~Robots~~ Machine Learning

- [TensorFlow](https://www.tensorflow.org/) - When robots take over the world, this will be the core of their DNA. TensorFlow is the principal Google Artificial Intelligence / Machine Learning library. They open-sourced it a few years ago. It's generally considered the most powerful in the world. There are APIs for Python and tons of other languages now.
- [Keras](https://keras.io/) - An overall neural network API, but basically it makes interacting with TensorFlow way easier. See this nice [DataCamp Tutorial](https://www.datacamp.com/community/tutorials/deep-learning-python).

## Data Mapping

- [YWorks](https://www.yworks.com/products/yed)
- [The Brain](http://www.thebrain.com/)
- [Orange](https://orange.biolab.si/)

## Data Quality Tools

- [Open Refine](http://openrefine.org/) - Great data cleanup platform.
- [Talend Data Preparation (Free Desktop Edition)](https://www.talend.com/products/data-preparation/) - Good GUI tool to analyze and clean data.


## General

- [Transformy](https://www.transformy.io/#/)
- [Datazar](https://www.datazar.com)
- [Diggernaut](https://www.diggernaut.com/) - Web scraping service.

## Text / Document Manipulation Tools

- [Pandoc](http://www.pandoc.org) - Amazing command line tool for converting documents between many different formats. For example, if you want to change a Word doc to a markdown file, you would run `pandoc -f docx -t markdown -o outputmarkdownfile.md sourcedocument.docx`.
- [Tabula](https://tabula.technology/) - Amazing tool for extracting tabular data out of PDFs. Works like a charm, pretty much every time. 