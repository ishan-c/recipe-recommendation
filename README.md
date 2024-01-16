# Recipe Recommendations from Food.com Data

## Project Overview
This project aims to create a recipe recommendation system using the extensive Food.com Recipes and Interactions dataset available on Kaggle. The goal is to develop a system that suggests recipes to users based on a set of their input ingredients or by analyzing their past favorite recipes. I selected this project to explore, learn, and practice advanced data processing, visualization, and machine learning techniques.

Initial stages have involved extensive exploratory data analysis (EDA) using Pandas and Seaborn to understand the dataset's characteristics and potential features for the recommendation system.

Future development includes implementing the recommendation logic using scikit-learn and PyTorch and eventually deploying and endpoint using AWS to make the system accessible for real-time user interaction. This system will ideally provide personalized culinary recommendations, helping users discover recipes aligned with their tastes and ingredient preferences.

### Status
This project is currently an early work-in-progress. First pass EDA is complete. Feature engineering and initial model selection is in progress.

## Data Source
The dataset used in this project is the "Food.com Recipes and Interactions" dataset, available on Kaggle. This dataset includes over 180K recipes and 700K user interactions collected from Food.com.

You can access the dataset on Kaggle here: [Food.com Recipes and Interactions Dataset](https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions).

Credits for compiling this dataset go to Shuyang Li and Bodhisattwa Prasad Majumder, who are listed as collaborators on Kaggle. Additionally, the dataset is used in [this paper](https://aclanthology.org/D19-1613/) by Shuyang Li, Bodhisattwa Prasad Majumder, Jianmo Ni, and Julian McAuley from the University of California, San Diego.

## Technology Stack
Please see the environment.yml file for the current, complete set of dependencies.
- **Language**: python, Jupyter Notebook
- **Data Processing and Visualization**: Pandas, Seaborn
- **Modeling** (Planned): PyTorch, scikit-learn
- **Deployment** (Planned): AWS

## Data Storage and Loading

### Data Organization
- **Raw Data**: Located in `/data/raw`, this directory contains the original dataset files as downloaded from Kaggle. It includes the author-provided subdirectory `pre-process` which contains the pre-processed data files used in the journal paper.
- **Processed Data**: After conducting Exploratory Data Analysis (EDA), the processed data is saved in the `/data/preprocess` directory in Parquet format for efficient storage and access.

### Data Processing Pipeline (Current)
- **Raw Data Ingestion**: The project initially ingests the two raw data files from the `/data/raw` without using the author-preprocessed data into the EDA notebook.
- **EDA and Preprocessing**: The EDA process involves cleaning and transforming the raw data. Key insights and transformations from this phase are documented in the corresponding Jupyter notebook.
- **Storage of Processed Data**: Post-EDA, the data is stored in Parquet format and exported to `/data/preprocess`. This format is chosen for its fidelity and efficiency in storing large datasets as well as its compatibility with Pandas.

#### Future Considerations
- As the project evolves, additional data processing steps may be introduced. At the very least, pre-processing will be de-coupled from EDA at some point and the equivalent transforms will be available as part of a pipeline. There will also be significant further transformations introduced as part of feature engineering.
- The method of data handling and storage will be adapted as needed to accommodate changes and ensure efficient data management throughout the project lifecycle.

## Methodology


## Completed Work


## Future Work

