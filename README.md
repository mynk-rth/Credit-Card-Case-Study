# Credit Card Case Study

A Jupyter-based exploratory data analysis (EDA) of credit card customer, spend, and repayment datasets. The repository contains raw CSV/Excel data and a notebook (casestudy2.ipynb) that demonstrates data cleaning, merging, and analysis steps used to answer business-style questions about customer behaviour and limits.

## What you'll find here

- casestudy2.ipynb — Jupyter notebook with the analysis and step-by-step code (data loading, cleaning, merging, and example EDA).
- Customer Acqusition.csv — customer/master table (customer id, age, city, product, per-transaction limit, company, segment).
- spend.csv — transactional spend records (customer id, date, category, amount).
- Repayment.csv — repayment records (customer id, date, repayment amount).
- Credit Card Data.xlsx — additional data in Excel format.
- Ps-softech Credit Card Case Study - Case Study 2.pdf — original problem statement / case study document.

## Highlights from the notebook

The notebook demonstrates common data-preparation and analysis tasks, including:
- Loading datasets with pandas and previewing rows (CSV / Excel read).
- Handling invalid/odd values (e.g., replacing ages < 18 with the dataset mean).
- Enforcing business rules (e.g., capping spend at 50% of a customer’s per-transaction limit when the recorded spend exceeds the limit).
- Merging customer, spend, and repayment tables for combined analysis.
- Basic EDA: sample tables, group-bys and summary statistics used to explore customer segments and spending behaviour.

## Quickstart — run the notebook locally

1. Clone the repository:

   git clone https://github.com/mynk-rth/Credit-Card-Case-Study.git
   cd Credit-Card-Case-Study

2. (Recommended) Create and activate a virtual environment:

   python -m venv .venv
   source .venv/bin/activate    # macOS / Linux
   .\.venv\Scripts\activate   # Windows (PowerShell)

3. Install minimal dependencies:

   pip install pandas jupyter openpyxl matplotlib seaborn

4. Start Jupyter and open the notebook:

   jupyter notebook casestudy2.ipynb

5. Follow the notebook cells to reproduce the analysis and charts.

Notes:
- The notebook reads the CSV files included in the repo; ensure they remain in the same folder as the notebook.
- If you prefer, you can convert the notebook to a script with nbconvert: `jupyter nbconvert --to script casestudy2.ipynb`.

## Reproducible commands (copy/paste)

   git clone https://github.com/mynk-rth/Credit-Card-Case-Study.git
   cd Credit-Card-Case-Study
   python -m venv .venv
   source .venv/bin/activate
   pip install pandas jupyter openpyxl matplotlib seaborn
   jupyter notebook casestudy2.ipynb

## Contributing

This repository is primarily a single-notebook case study. If you want to contribute:
- Open an issue to describe the change or improvement.
- For code changes, convert notebook edits into a new branch and open a pull request.
- If you add dependencies, include a requirements.txt file.

## License

Add a LICENSE file to specify the repository license. If you want a quick default, consider the MIT License.

## Contact

For questions about the analysis or data, open an issue or contact the repository owner: mynk-rth on GitHub.
