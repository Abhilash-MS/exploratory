# exploratory
Exploratory Data Analysis

## Description

This project explortory was created to perform Exploratory Data Analysis on any structured dataset. Dataset can have categorical or numerical data types. 
This project takes pandas dataframe and gives summary statistics and individual plots having categorical count for catagorical variables and PDF's, CDF's with mean, median and mode for numerical variables. The both the results are stored in PDF and CSV file in your current directory/path.  


## Installation:
Use the package manager [pip](https://pypi.org/project/exploratory/) to install exploratory
```bash
pip install exploratory
```
## Usage:

```python
from exploratory import EDA
EDA(df)
# df --> pandas dataframe
#Please input the DPI value, as DPI value increases runtime would increase. Default DPI value: 150
```
## Example Run:

![Exploratory Run](https://user-images.githubusercontent.com/114361354/207988464-669b7eec-5119-4ef3-88fe-bd094917ef16.gif)


## Expected Outputs:
* CSV File, DataFrame Containing 

| Column          | Description                                                         |
|-----------------|---------------------------------------------------------------------|
| Variable        | Variable Name in the dataset provided                               |
| Cardinality     | Number of levels/classes in each variable                           |
| total_count     | Count of total records (non null)                                   |
| unique_rate     | Cardinality / total_count, Unique Rate of 1 indicates a ID variable |
| percent_missing | Percentage of missing values across each column                     |
| mean            | Average of column (Ignores Object/String variables)                 |
| std             | Standard deviation of column (Ignores Object/String variables)      |
| min             | Minimum of column (Ignores Object/String variables)                 |
| 25%             | 25th percentile value of column (Ignores Object/String variables)   |
| median          | 50th percentile value of column (Ignores Object/String variables)   |
| 75%             | 75th percentile value of column (Ignores Object/String variables)   |
| max             | Maximum of column (Ignores Object/String variables)                 |
| data_types      | Data type of column (Int / Float / Object etc)                      |
| range           | Max Value - Min Value (Ignores Object/String variables)             |



* PDF with Statistical Summary and variable distribution graphs  (categorical & continous)


![Exported PDF](https://user-images.githubusercontent.com/114361354/207987618-ea144695-f18e-4f38-9bee-d7e313152bf6.gif)


## Contributing
Pull requests are welcome.For major changes, please open an issue first to discuss what you would like to change.
Please feel free to contact authors for any suggestions or issues,  Ram <kakarlaramcharan@gmail.com>, Abhilash <abhilashmaspalli1996@gmail.com> 
