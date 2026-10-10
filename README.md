# Retail Customer Analysis | Python, Pandas & EDA

## Project overview

This project analyses retail transaction data by combining transaction records, customer demographics, and product-category information. The notebook uses Python and Pandas to clean and join datasets, explore distributions, compare categories, and answer business questions.

## Tools

- Python
- Pandas and NumPy
- Matplotlib
- Jupyter Notebook

## Repository structure

```text
retail-customer-analysis/
├── Retail_Customer_Analysis.ipynb
├── README.md
└── data/
    ├── Transactions.csv
    ├── Customer.csv
    └── prod_cat_info.csv
```

## How to run

1. Download or clone this repository.
2. Install Python and Jupyter Notebook (or use Google Colab).
3. Install the libraries used in the notebook:

   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

4. Open `Retail_Customer_Analysis.ipynb` from the repository root.
5. Run the notebook cells in order. The notebook loads the three CSVs from the `data/` folder.

## Analysis workflow

1. Load and inspect the three datasets.
2. Convert transaction dates and customer dates of birth to datetime values.
3. Merge transactions with customer information and product hierarchy.
4. Review column types, observations, numeric summaries, and categorical frequency tables.
5. Create histograms and frequency bar charts.
6. Answer business questions about transaction dates, negative amounts, product-category activity by gender, customer city codes, store type, flagship-store sales, and customers aged 25–35.
7. Summarise the results and key observations.

## Selected findings from the notebook

- The merged transaction-level dataset contains **23,053 rows and 18 columns**.
- The transaction dates range from **25 January 2011 to 28 February 2014**.
- **2,177** transaction records have a negative `total_amt`; these are treated as potential returns/reversals in the case study and are analysed separately where required.
- **Books** has the highest number of transaction records for both female and male customers.
- **City code 3** has the highest number of unique customers represented in the merged transaction data (**576**, or **10.46%**).
- **e-Shop** has the highest aggregate transaction value and quantity in the supplied data.

These findings describe this dataset and should not be interpreted as general conclusions about all retail businesses.

## Data notes

The notebook expects the following filenames under `data/`:

- `Transactions.csv`
- `Customer.csv`
- `prod_cat_info.csv`

Before making the repository public with the CSV files included, confirm that the original dataset's terms permit redistribution. If redistribution is not permitted, remove the CSVs from the public repository and add instructions linking to the original authorised dataset source instead. The customer file includes demographic fields such as date of birth, gender, and city code, so keep the repository limited to the provided dataset and do not add personal or confidential information.

## Limitations

- Negative amounts are interpreted in the context of the case study; the dataset alone does not prove the reason for every negative transaction.
- Results depend on the supplied dataset, join logic, and analysis definitions.
- Age is calculated relative to the transaction date in the notebook.

## Author

Created as a data analytics learning project to practise data preparation, exploratory data analysis, visualisation, and business-focused analysis.
