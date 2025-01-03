# Data Sourcing Challenge

---

## Overview

This repository contains the solution to the Data Sourcing Challenge, focusing on retrieving and analyzing data from NASA's DONKI API. The project demonstrates data retrieval, cleaning, and analysis techniques to identify relationships between Coronal Mass Ejections (CMEs) and Geomagnetic Storms (GSTs).

---

## Key Tasks

The analysis consists of the following major tasks:

1. **Data Retrieval:**
	- Fetching CME and GST data from NASA's DONKI API using custom API queries.
	- Specifying time ranges for retrieving historical data (2013–2024).
	- Exporting retrieved data for further processing.

2. **Data Cleaning and Preparation:**
	- Filtering and expanding nested fields like `linkedEvents` for granular analysis.
	- Ensuring consistent datetime formatting for event comparisons.
	- Removing invalid or missing data to maintain data integrity.

3. **Data Analysis:**
	- Merging CME and GST datasets based on linked activity IDs.
	- Calculating the time difference between CME and GST events.
	- Summarizing the mean and median time for a CME to cause a GST.

4. **Results Export:**
	- Exporting the processed data into `merged_data.csv` for easy access and review.

---

## How to Run

Clone the Repository:
```bash
git clone https://github.com/CCIEMikeG/data-sourcing-challenge.git
cd data-sourcing-challenge
```

1. **Set Up the Environment:**
	- Ensure Python 3.x is installed.
	- Install required libraries:
	```bash
	pip install -r requirements.txt
	```

2. **Add Your API Key:**
	- Rename `example.env` to `.env`.
	- Add your NASA API key to the `.env` file in the following format:
	```
	NASA_API_KEY=<your_api_key>
	```

3. **Run the Notebook:**
	- Open `retrieve_data_2.ipynb` using Jupyter Notebook or VS Code.
	- Execute each cell sequentially to replicate the analysis.

---

## Dependencies:

Ensure the following Python libraries are installed:

	- pandas
	- numpy
	- requests
	- matplotlib
	- dotenv

You can install these libraries with:
```bash
pip install pandas numpy requests matplotlib python-dotenv
```

---

## Results

The analysis successfully:

	- Retrieved historical data on CMEs and GSTs.
	- Cleaned and prepared datasets for analysis, ensuring consistent formatting and structure.
	- Merged CME and GST datasets to analyze relationships.
	- Calculated the time difference between CMEs and GSTs, identifying average response times.

---

## License

This project is licensed under the MIT License.

