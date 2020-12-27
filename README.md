# Prediction of CO2 emissions from country-specific data
# A Machine Learning Project
### by Vladislav Todorov

***
## README

***

## Contents:
1. Project description
	- Context and goals
	- Project structure
2. Built with
3. Summary of all project stages
4. How to open
5. Dataset information
6. License information

***

## 1. Project description

### Context and goals
Predictive Machine Learning (ML) models and the big amount of available data can be very useful to analyze the development of climate change trends or relevant contributors. In theory, the country emissions of greenhouse gases such as CO2 over a year could depend on certain country-specific aspects. In this context, I have developed a ML project aiming to analyze and predict CO2 emissions from country-specific parameters such as economic indicators, population, energy use, land use, etc.

For this purpose, I have used the publicly available dataset provided by the World Bank Group, which includes parameters such as:
* country: the vast majority of countries worldwide
* year: ranging from 1990 to 2011
* emissions of greenhouse gases such as CO2, CH4, N2O, others
* population-specific parameters: population count, urban population, population growth, etc.
* country economic indicators: GDP, GNI, Foreign Direct Investment, etc.
* land-related parameters: cereal yield, agricultural land, Nationally terrestrial protected areas, etc.
* climate data: precipitations, national disasters, etc.
* energy use
* counts of certain types of medical personnel
* etc.


### Project structure

The project is divided into three stages:

* Stage 1: Data cleaning and preparation (file *1_data_preparation*)
* Stage 2: Data exploration and visualization (file *2_data_visualization*)
* Stage 3: Predictive analysis with the Random Forest machine learning algorithm (file *3_predictive_analysis_rf*)

Each of the stages is described in a separate Jupyter Notebook(.ipynb file) and a derived pdf file.

***

## 2. Built with

* **Programming language**
	- Python 3.7
* **Libraries**
	- **dataset handling**: pandas, numpy
	- **data visualization**: seaborn, matplotlib ( "Copyright (c) 2002-2009 John D. Hunter; All Rights Reserved")
	- **machine learning**: scikit-learn
* **Presentation**: 
	- Jupyter Notebook
	- derived identical HTML files

***

## 3. Summary of all project stages
The highlights of all project stages are briefly introduces in the following:

### Stage 1: Data cleaning and preparation

* Global data overview
* Definition of the initial project goals
* Data cleaning
    - dealing with missing values
    - transformation of the columns into a numerical data type
    - renaming of features
    - removing empty columns and rows
* Data frame transformation
    - melting of the data for each variable
    - integration of the data into a suitable data frame format
* Removal of missing values
    - detection of missing values
    - removal of missing values by filtering the columns and rows, so that minimal amount of features and rows are lost
* Export the clean data frame to a file

### Stage 2: Data exploration and visualization

* Feature/column abbreviations and units
* Definition of the hypothesis to be tested
* Feature engineering
    - features overview
    - derivation of additional important features
    - removal of unnecessary features
* Prepare the visualization
* Create plots
	- a global look onto all relationships and detailed plots of chosen dependencies
    - correlation matrix heatmaps
    - scatterplots, histograms
    - detection of outliers
    - discussion of dependencies and trends
* Conclusions

### Stage 3: Predictive analysis with the Random Forest machine learning algorithm

* Selection of dependent and independent variables
* Dataset splitting into training and test subsets
* Feature selection with recursive feature elimination and cross-validation
* Hyperparameter tuning of a random forest model with cross-validation
* Training and evaluation of the model with the best hyperparameters on the training data with cross-validation
* Validation of the model on the test subset (previously unseen data)
* Conclusions

***

## 4. How to open

* Just download and view the HTML files (exported from and identical with the Jupyter Notebooks) in an internet browser. These are located in the */HTML* folder

or

* download the Jupyter Notebooks (.ipynb files in the */Jupyter_Notebooks* folder), open Jupyter Notebooks, browse to the downloaded files and open them.

***

## 5. Dataset information

The dataset used is the Climate Change Data provided by the World Bank Group, which includes country-specific data on parameters such as CO2 emissions, energy use, population count, urban population, cereal yield, nationally terrestrial protected areas, GDP, GNI, etc.

The dataset is publicly available at https://datacatalog.worldbank.org/dataset/climate-change-data and licenced under the <a href="https://datacatalog.worldbank.org/public-licenses#cc-by">Creative Commons Attribution 4.0 International license</a>.

The downloaded original data file *"climate_change_download_0.xls"* has not been modified before its import to the Jupyter Notebooks and is located in the folder */original_data*. All operations applied to the data within the analyses are transparently documented in the Jupyter Notebooks and the corresponding HTML files.

***

## 6. License information and disclaimer notice
Copyright (c) 2020 Vladislav Todorov

When using any part of the source code, any part of the documentation or of
the results in any kind of publications, the present Software and the copyright holder should
be referenced in an appropriate way.

The current work/Software has been conducted in a private manner by using the tools and the data source listed in this README file. The current work, the Software and the obtained results have not been endorsed, ordered or sponsored by any party or entity whatsoever.

The detailed licence can be found in the *LICENCE.txt* file in the project root folder.



***