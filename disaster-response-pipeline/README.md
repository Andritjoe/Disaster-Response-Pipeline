# Disaster Response Pipeline Project

## Motivation
The main purpose of the project is to build a model that analyse and classifies disaster messages from Figure Eight to build a model using the web app (flask).

## Display of web apps

![](https://github.com/Andritjoe/Disaster-Response-Pipeline/blob/master/disaster-response-pipeline/Disasters%20(1).jpg)

### Install

This project requires Python version 3.6.5 and the following Python libraries installed:

- scikit-learn : http://scikit-learn.org/stable/ - A Python machine learning library
- pandas : http://pandas.pydata.org - A Python data analysis tool
- numpy : http://www.numpy.org - A package for scientific computing with Python
- Plotly : https://plotly.com - Visualization tool
- Nltk : https://www.nltk.org - Text processing libraries
- Flask : https://flask.palletsprojects.com - web framework
- Sqlalchemy : https://www.sqlalchemy.org - sql library
- Re : https://docs.python.org/2/library/re.html - regex


### Code file
process_data.py: The ETL pipeline used to process data in preparation for model building.
train_classifier.py: The Machine Learning pipeline which involves fitting, tuning, evaluating, and exporting the model.
templates folder: This folder contains all of the files necessary to run and render the web app.


### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
