
# Project: Business predictions with analysis 
This is a Business storage, sells based predictions and anylysis project. <br> 
This notebook uses Raw Pandas on tabular data with statistics and makes data science predictions. 
All works in this project falls into one of two types: 
* Business analysis and data analysis
* Business prediction and data science

# Works: 
This project worked with multiple sheets under the same csv file.<br>
List of all works for reference: <br>
* which product was sold the least amount? 
* which product was sold the most amount? 
* yearly how many amount of product are left in stock after sell? 
* Predict the amount of product are left in stock for Next year. 
* Predict the amount of money to inverst for Next year. 
* Find profit yearly.
* Predict profit for next year.
* Find profit of product of every brands sequentially.
* Find which product from every brands sold the most sequentially.
* Make sell prediction per day.

## Business analysis and data analysis:
* yearly how many amount of product are left in stock after sell?

`groupby()` Transaction Type (`TransType`) from dataset (Buy transaction Type, Sell transaction Type).<br>
`groupby(year)` from `sub-dataframe`. <br>
For every year 2018, 2019, 2020, 2021 calculated cumulative buy quantity, sell quantity. Afterwards comparison will give total remaining in stock. <br>
Resources used: `pandas`



## Business prediction and data science:

* Predict the amount of product are left in stock for Next year.

Aforementioned engineering also gives previous years data history. Use this data as `training data`.<br>
Apply `regression` for prediction.<br>
Resources used:  `scikit-learn`, `LinearRegression()`



## Business analysis and prediction: 

* Make sell prediction per day.
  

_use satatistical method, visualization:_ <br>
apply `histogram()` on daily `Qty`(sell quantity) data.<br>
use `mean()` addition to standard deviation `std()` to clean data.<br>
pick percentage from histogram to pick per day sell prediction without `outlier`.<br>
Resources used: <br>  `histogram`, `matplotlib`, `standard deviation`
<br>

_use predictive method:_ <br>
clean `Qty`(sell quantity) data removing `outliers`. 
apply different regressors. benchmark models. <br>
`DecisionTreeRegressor()` performs best. Improve model by using ensemble `RandomForestRegressor()` which gives the highest result.<br>
Resources used:  <br>`histogram`, `matplotlib`, `standard deviation`, `DecisionTreeRegressor()`, `RandomForestRegressor()`



## Business prediction and data science: 

* Predict money amount to invest for Next year.

`groupby()` to find money invested each year. this creates `training data` of previous years.<br>
Apply `regression` for prediction.<br>
Resources used: <br>`scikit-learn`, support vector regressor `SVR()`, `DecisionTreeRegressor()`, `RandomForestRegressor()`



## Business analysis and data analysis:
First Strategically calculated:<br>
cumulative Brand-wise sells amount and earning <br>
cumulative Item-wise sells amount and earning<br>
then answer:<br>
* which product was sold the least and most? 
* which product was sold the most?
from multiple dimensions:
* In terms of money
* In terms of Quantity
* Brand-wise
* Item-wise

Resources used: `pandas`



## Business analysis and data analysis:

* Find profit yearly. 

`groupby()` Transaction Type and then year.<br>
for every year 2018, 2019, 2020, 2021 calculated cumulative buy money and sell earning to further figure out profit.

<br>

and more:
* Predict profit for next year.
* Find profit of product of every brands sequentially.
* Find which product from every brands sold the most sequentially.

P.s. this specific dataset will not be shared without permission as request of dataset author.<br>

libraries used: `sklearn`, `pandas`, `matplotlib`, `numpy`<br>

Techniques used: histogram, standard deviation, outlier processing, yearly data find, LinearRegression, DecisionTreeRegressor, SVR, linear_model.Lasso, RandomForestRegressor <br> 

<br>

using the repository:
1. Download the repository on your pc using the following command.
```bash
git clone https://github.com/tanvir-ishraq/business-predictions-project-and-analysis.git
```
2. Activate the virtual environment
On Windows:
```bash
virtualenv venv
venv\Scripts\activate
```
On Mac/Linux:
```bash
virtualenv --no-site-packages  venv
source venv/bin/activate
```
3. Install Dependencies
```bash
pip install -r requirements.txt
```
4. Use jupyter notebook, VSCode or google colaboratory as your choice. <br>
e.g. Open jupyter notebook by running the following command in the terminal
```bash
jupyter notebook
```
5. Navigate codes, read git documentation and run the cells. Further information are given in the comments of notebook.

