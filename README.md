# Starbucks-Project
Capstone project of Udacity data scientist nanodegree.

## Table of Contents
1. [Installation](https://github.com/Rawan-Alharbi/Starbucks-Project#Installation)
2. [Project Motivation](https://github.com/Rawan-Alharbi/Starbucks-Project#Project-Motivation)
3. [File Descriptions](https://github.com/Rawan-Alharbi/Starbucks-Project#File-Descriptions)
4. [Analysis Summary](https://github.com/Rawan-Alharbi/Starbucks-Project#Analysis-Summary)

## Installation
This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/installing.html)
- [scikit-learn](http://scikit-learn.org/stable/)
- [Jupyter-Notbook](https://jupyter.org/install.html)

Or you could install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all 
of the necessary libraries and software for this project.

## Project Motivation
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, 
Starbucks sends out an offer to users of the mobile app. Using this dataset I have built a model that predict whether customers will respond to 
offers or not.

## File Descriptions

The data is contained in three files:
* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.).
* profile.json - demographic data for each customer.
* transcript.json - records for transactions, offers received, offers viewed, and offers completed.

Here is the schema and explanation of each variable in the files:

### portfolio.json
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

### profile.json
* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

### transcript.json
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Analysis Summary
Analysis summary is available [here](https://medium.com/@RawanAlharbi1/starbucks-offer-analysis-6ed8641779bc)
