# IEBC DATA SCRAPPING SCRIPTS

## Setting up the project.
You need to have python preinstalled in your system and a stable network connection as a prerequesite.

Run the following commands promptly to get started.
1. python3 -m venv iebc_env to set up a virtual environment
2. source iebc_env/bin/activate to activate the virtual environment.
3. pip install -r requirements.txt to install the required packages.
4. jupyter-lab This will launch jupyterlab where you'll run the main.ipynb file.

When everything goes as expected, you'll have the following files created on your working directory:
constituencies.csv
counties.csv
polling_stations.csv
registration_officers.csv
wards.csv
iebcrecords.db
iebc_records.xlsx

In dbms for the db is sqlite, so you can run sqlite3 iebcrecords.db to get into the db or use a gui sqlite browser.
There will be a view table that aggregates all the results from the various csv files.
