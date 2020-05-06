Sepsis Prediction Methodology
==============================
This repository contains a rewritten version of the code for our submission (Team Name: Can I get your Signature?) to the PhysioNet 2019 challenge. 


Getting Started
---------------
Once the repo has been cloned locally, setup a python environment with ``python==3.7`` and run ``pip install -r requirements.txt``.

Create a folder `/data/raw`, the `data/` folder should be made a symlink if you wish to store the large data files elsewhere. 

Run the following:
    1. ``python src/data/get_data/download.py`` To download the raw .psv files to `/data/raw`
    2. ``python src/data/get_data/convert_data.py`` To convert the downloaded data into a pandas dataframe (for easy analysis) and a TimeSeriesDataset (for fast operations).
    
You are then ready to go! Check `/notebooks/examples/prediction.ipynb` for an intro to the basic prediction methods and the functions used to generate the features. 
