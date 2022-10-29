# Tanzania Tourism Prediction: ML Project
The main goal of this project was about to create a ML model to predict how much money a tourist will spend when visiting Tanzania.

The data used for this is: [data](https://zindi.africa/competitions/tanzania-tourism-prediction/data).

Hypothesis: Tourists are likely to spent more money depending on their age.

To impove our hypothesis we trained a regression model to predict the total cost a tourist can spend.
Contribution features are:
- In what age group is a tourist
- The country a tourist coming from
- Which packages a tourist have
- Number of tourists

## Exploratory Data Analysis (EDA)

## Data Cleaning and Feature Engineering
## Model Building and Evaluation

# Requirements and Environment

Requirements:

- pyenv with Python: 3.9.8

Requirements:
- pyenv with Python: 3.9.8

Environment: 

For installing the virtual environment you can either use the Makefile and run `make setup` or install it manually with the following commands: 

```Bash
pyenv local 3.9.8
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Usage

In order to train the model and store test data in the data folder and the model in models run:

```bash
#activate env
source .venv/bin/activate

python example_files/train.py  
```

In order to test that predict works on a test set you created run:

```bash
python example_files/predict.py models/linear_regression_model.sav data/X_test.csv data/y_test.csv
```

## Limitations

Development libraries are part of the production environment, normally these would be separate as the production code should be as slim as possible.
