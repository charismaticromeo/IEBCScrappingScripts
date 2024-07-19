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

## The results should look something like this:

### The aggregate views table
![Screenshot_2024-07-19_00-38-18](https://github.com/user-attachments/assets/a56e997f-3b7a-4a76-934c-87d46546a8c6)
![Screenshot_2024-07-19_00-37-42](https://github.com/user-attachments/assets/73260653-fd11-4e6b-9571-b85b118031e9)

### Counties table
![Screenshot_2024-07-19_18-36-59](https://github.com/user-attachments/assets/607fa819-3649-4c31-8e21-e178a8688f38)

### Constituencies table
![Screenshot_2024-07-19_18-38-45](https://github.com/user-attachments/assets/0e7f1bcc-a779-4c3b-82ff-c0c0f11ebdf8)

### Wards table
![Screenshot_2024-07-19_18-39-57](https://github.com/user-attachments/assets/bc984e2e-5970-473f-999c-574dba775449)

### Polling Stations Table
![Screenshot_2024-07-19_18-41-06](https://github.com/user-attachments/assets/3842d6fa-120f-4789-955b-bc84fb810a19)

Then finally a table of registration officers for each constituency.
