# Course Outline: Intermediate Python for Accounting

### Course Learning Objectives (from Track Proposal):
  By the end of this course, students will be able to...
  - Execute and present Python code with Jupyter Notebooks
  - Create, read, copy, and update data in Pandas DataFrames and Series objects
  - Clean, manipulate and summarize data in Pandas by merging, grouping, filtering, and generating pivot tables

## Chapter 1: Organizing and Presenting Code with Jupyter Notebooks
### Lesson 1.1: Setting Up
- Learner will be able to create a Jupyter Notebook and organize it with various cell types and basic markdown formatting
- Learner will be able to navigate through a Jupyter Notebook using edit and command mode and shortcuts as well as an understanding of Kernels
### Lesson 1.2: Running Code
- Learner will be able to connect a Jupyter Notebook to libraries, code snippets, and their own computer through notebook imports, magic commands, and terminal commands
### Lesson 1.3: Presenting
- Learner will be able to prepare presentable HTML slides from Jupyter Notebook cells, including images and styling

## Chapter 2: Introduction to Working with Data in Pandas
### Lesson 2.1: Pandas Data Structures
- Learner will be able to create Pandas Series and DataFrames and describe thier contents using utility methods and attributes
- Some functions introduced/used: .head(), .shape(), .info(), .describe()
### Lesson 2.2: Data Selection
- Learner will be able to select and filter data with data slicing and Boolean indexing
- Some functions introduced/used: .loc(), .iloc()
### Lesson 2.3: Addressing Missing Data
- Learner will be able to identify and evaluate missing data to recommend an appropriate way to deal with it
- Some functions introduced/used: .isnull(), .dropna(), .fillna(), .replace()
### Lesson 2.4: Arranging Data
- Learner will be able to order and categorize data according to their needs
- Some functions introduced/used: .groupby(), .sort_values(), .agg()

## Chapter 3: Summarizing and Manipulating Data in Pandas
### Lesson 3.1: Summary Methods
- Learner will be able to summarize data using Pandas summary functions
- Some functions introduced/used: .sum(), .mean(), .count(), .std(), .apply()
### Lesson 3.2: Vectorized Operations
- Learner will be able to manipulate data using vectorized functions
### Lesson 3.3: Cleaning Data
- Learner will be able to improve data quality using techniques such as data type conversion, re-indexing, and dropping and renaming columns
- Some functions introduced/used: .to_numeric(), .astype()

## Chapter 4: Combining Data in Pandas
### Lesson 4.1: Concatenating
- Learner will be able to add data along a given axis in Pandas
- Some functions introduced/used: .concat()
### Lesson 4.2: Merging and Joining
- Learner will be able to relate and combine multiple DataFrames based on their indexes or a shared value.
- Some functions introduced/used: .join(), .merge()
### Lesson 4.3: Reshaping and Pivot Tables
- Learner will be able to rearrange data using reshaping and pivot table functionality in Pandas
- Some functions introduced/used: .reshape(), .stack(), .pivot_table()
