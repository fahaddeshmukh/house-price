
## House price prediction using Machine learning



### Overview

The aim of the project  centers around the utilization of machine learning techniques for the accurate prediction of housing prices. The precise estimation of property sale prices holds immense significance within real estate markets, serving various purposes such as aiding investment choices, determining property values, and facilitating market analysis. Leveraging machine learning algorithms and a dataset replete with pertinent housing features, the objective is to craft a predictive model capable of estimating housing prices with a high degree of accuracy.

The approach is systematic, commencing with data preprocessing, followed by exploratory data analysis (EDA), feature selection, and feature engineering. Subsequently, an assortment of machine learning algorithms is employed to train and evaluate predictive models using the processed dataset.

## Installation

To use this script, you need to have Python installed on your system (3.8 or higher). You also need to install the required dependencies by running the following command:

```
pip install -r requirements.txt
```
## Directories

The project is structured as follows:

- **bin**: This directory contains the source code files required to run the analysis.
  - `house.py`: This Python script is the main entry point for running the project. It contains the code that reads the dataset and performs various data processing, visualization and modelling tasks.
 
  - `house.ipynb`: This Jupyter Notebook file provides an alternative interface for running the analysis interactively. It contains the same code as `house.py` but provides easy accessablity along with a narrative.

- **data**: This directory contains the dataset used for the analysis.
  - `train.csv`: The CSV file that contains the data on the sale price of various properties. The file is required for running the analysis. Please ensure that it is located in this directory.

- **modules**: This directory contains the modules used project.
- `modules.py`: The modules.py script contains utility functions used by the house.py script to preprocess data and evaluate models.
- **plots**: This directory contains the EDA plots used for the analysis.
## Usage

The script requires two input files: house.py and train.csv. Place these files in the data directory of your project. Then, run the following command to execute the preprocessing script:

```
python bin/house.py data/train.csv
```

The script will perform the following steps:

1. Data Preprocessing: The script performs data preprocessing, including handling missing values and transforming numerical features.
2. Data Visualization: It generates histograms and box plots to visualize the data distribution and relationships between variables.
3. Model Evaluation: The script evaluates multiple machine learning models (Linear Regression, Random Forest, and LGBM) and provides Mean Squared Error (MSE) and R-squared scores.
4. Results: The evaluation results are saved in the results/ directory, including yPred_yTrue_table_{model_name}.txt files.




## Requirements

The script requires the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- lightgbm
- scipy

You can install these packages by running the command mentioned in the "Installation" section.

## Functions

The modules.py script contains utility functions used by the house.py script to preprocess data and evaluate models:
<ul>
    <li><b>count_null_data</b>: Counts and prints the number of missing values in each column of the dataset.</li>
    <li><b>delete_columns_with_zero_data</b>: Removes columns with a high number of zero values from the dataset.</li>
    <li><b>separate_categorical_numerical</b>: Separates categorical and numerical columns in the dataset.</li>
    <li><b>drop_columns_with_zero_threshold</b>: Drops columns with a high number of zero values based on the specified threshold.</li>
    <li><b>plot_categorical_columns</b>: Plots bar charts for categorical columns to visualize value counts.</li>
    <li><b>apply_1_plus_log_transformation</b>: Applies the 1 plus log transformation to specified numerical columns.</li>
    <li><b>model_evaluation</b>: Evaluates machine learning models and returns the Mean Squared Error (MSE) and R-squared scores.</li>
</ul>


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.md) file for details.

## Contact Information
For any questions, suggestions, or issues, please feel free to contact:

- Name: Fahad Deshmukh
- Email: deshmukh@uni-potsdam.de


