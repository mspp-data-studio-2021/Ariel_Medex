# Ariel_Medex
# Getting Started
You will first need to download and install [Python3](https://realpython.com/installing-python/).

Then clone this project repository, and open a command prompt/terminal window and navigate to the project directory.

To access your API key without risking it being published on GitHub this project uses the dotenv package. You need to edit the file .env_sample and add your key, then rename the file to .env.

Now you can create a virtual environment for python. On Mac OS you can use the following steps:

```
pip3 install virtualenv # if you don't already have this installed
virtualenv env
source env/bin/activate
which python # confirm you are using the virtual env
pip3 install -r requirements.txt
python -m ipykernel install --user --name=env
jupyter notebook
```

# Replicating the Analysis
To recreate all the results you will need to run all of the numbered scripts and notebooks in [`/code`](/code):

Below are the numbered datasets that correlate to the numbered notebooks for download. Make sure all downloaded csvs are in the base directory of your local copy of the repository:
* [`001usa_00003.csv`](https://www.dropbox.com/s/wuukgsjwrxzr89h/001usa_00003.csv?dl=0)
  * This downloads the raw, uncleaned data pulled from IPUMS USA. Use for Notebook 001
* [`002usa_00003.csv`](https://www.dropbox.com/s/qljngl9yrv0vuty/002usa_00003.csv?dl=0)
    * This is the first cleaned csv generated by Notebook 001 and should be used for Notebook beginning 002.
* [`003usa_00003.csv`](https://www.dropbox.com/s/he5nu1y9xedeuii/003usa_00003%20.csv?dl=0)
    * This is the second cleaned csv generated by Notebook 001 and should be used for Notebook beginning 003.
* [`004usa_00005.csv`](https://www.dropbox.com/s/sbr0j9j1t1algqt/004usa_00005.csv?dl=0)
    * This is the final csv needed to run Notebook beginning 004. It also raw data pulled from IPUMS USA of the entire NYC population.

## Accessing Shape File for Notebook 002
[Link to the shape file](https://www.dropbox.com/sh/92g1w7tjiity76b/AADPMvZh_j-afWW2tL9CbEjja?dl=0)
Download and unzip the file. Make sure the folder is in base directory of your local copy of the repository. 

## Note all map visualization gifs were made in Adobe Photoshop

## [Link to Medium Post](https://medium.com/@ajs701/investigating-the-economic-impacts-of-medicaid-expansion-in-new-york-city-3d20cbe1358e)

# Acknowledgements
All data from IPUMS USA:
    Steven Ruggles, Sarah Flood, Sophia Foster, Ronald Goeken, Jose Pacas, Megan Schouweiler and Matthew Sobek. IPUMS USA: Version 11.0 [dataset]. Minneapolis, MN: IPUMS, 2021. https://doi.org/10.18128/D010.V11.0


This project was created using ['GeoPandas'](https://towardsdatascience.com/mapping-with-matplotlib-pandas-geopandas-and-basemap-in-python-d11b57ab5dac) and ['weightedcalcs'](https://github.com/jsvine/weightedcalcs)