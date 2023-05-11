# Education-Inequality
assessing educationa inequality through analysing socioeconomic factors and school performance, in terms of SAT and ACT scores

## DATA

The 2016 dataset containing SAT/ACT scores and socioeconomic characteristics for school districts comes from EdGap.org.
EdGap Data Source: https://www.edgap.org/#4/37.89/-97.00


Dataset providing basic information about each school, pulled from the National Center for Education Statistics.

NCES Data Source: https://nces.ed.gov/ccd/pubschuniv.asp

NCES Dataset: https://www.dropbox.com/s/lkl5nvcdmwyoban/ccd_sch_029_1617_w_1a_11212017.csv?dl=0

## Data Preparation

The data types for the school id for both datasets were changed to int64 so that they were able to be merged on that column later on. A subset of the data was taken, and all invalid act scores were dropped from the dataset. All invalid percentages for socioeconomic characteristics were replaced with NaN values. A train test split (keeping 20% of the data) was set up, and then all missing values from the training dataset were replaced with values from an iterative imputer.

The notebook with the data preparation can be found here in this repo: https://github.com/pintoanabel/Education-Inequality/blob/main/Pinto_Prep_DATA_3320_Education_Inequality_Data_Preparation.ipynb

The cleaned datafram can be found here in this repo: https://github.com/pintoanabel/Education-Inequality/blob/main/clean_education_inequality.csv

## Data Analysis

Regression plots were constructed for some of the individual predictors and ACT scores.
Prediction plot (regression) was utilized on the full model of all 9 predictors.
Best subset selection was utilized to determine the 8 predictor model was best.
Prediction plot using 8 predictors was constructed.
Heat map visualizations of different predictors and ACT scores by state were created and displayed.

Link to the notebook that performs the data analysis in this repository: https://github.com/pintoanabel/Education-Inequality/blob/main/Pinto_Analysis_DATA_3320_Education.ipynb

## Authors

The author of this repository and its contents is Anabel Pinto LinkedIn: https://www.linkedin.com/in/anabel-pinto/

## License

GNU GPLv3 (GNU General Public License v3.0)
