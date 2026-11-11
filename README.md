Credit Card Default — Exploratory Data Analysis
A reproducible, notebook-based exploratory data analysis of the Default of Credit Card Clients dataset from the UCI Machine Learning Repository.

The project examines customer demographics, credit limits, repayment history, monthly bills and payments, and their observed relationship with next-month default status. It combines data-quality checks, statistical summaries, visual analysis, and an interactive filtering dashboard.
<p align="center">
  <a href="https://colab.research.google.com/github/abhishekpal8146/credit-exploratory-data-analysis/blob/main/CEDA.ipynb">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Google Colab">
  </a>
  <a href="https://github.com/abhishekpal8146/credit-exploratory-data-analysis">
    <img src="https://img.shields.io/badge/Project-Notebook%20EDA-295F78" alt="Notebook EDA">
  </a>
  <a href="https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients">
    <img src="https://img.shields.io/badge/Data-UCI%20Repository-blue" alt="UCI Dataset">
  </a>
</p>Project at a glance
Item	Details
Analysis type	Exploratory Data Analysis (EDA)
Dataset	Default of Credit Card Clients
Data source	UCI Machine Learning Repository
Dataset ID	350
Observations	30,000 clients
Variables	23 explanatory features + 1 target
Main tools	Python, Pandas, NumPy, Matplotlib, Seaborn, ipywidgets
Main deliverable	CEDA.ipynb


Objectives
- Load the dataset directly from its authoritative UCI source.
- Inspect dimensions, data types, missing values, unique values, and duplicate records.
- Convert encoded demographic and outcome values into readable labels for analysis.
- Explore credit limits, customer demographics, repayment status, bills, and payments.
- Compare observed patterns between clients with and without next-month default.
- Use descriptive statistics, visualizations, and correlation analysis to communicate findings.
- Provide an interactive dashboard for exploring filtered customer segments.
Dataset and provenance
The notebook retrieves the dataset using the official UCI dataset identifier through the ucimlrepo package. A separate dataset download is not required.
- Dataset page: Default of Credit Card Clients — UCI Machine Learning Repository
- Dataset DOI: 10.24432/C55S3H
The dataset contains client demographic information, credit limits, repayment-status records, six months of bill amounts, six months of payment amounts, and the next-month default-payment outcome.
Analysis workflow
1. Environment setup — check and install the notebook's required Python packages.
2. Data acquisition — retrieve dataset 350 from the UCI repository.
3. Data-quality assessment — inspect shape, column types, missing values, unique values, descriptive statistics, and duplicate rows.
4. Readable labels and derived features — prepare interpretable demographic categories and credit-behavior summaries while retaining the original loaded data.
5. Default outcome overview — examine the target distribution.
6. Demographic analysis — compare observed default patterns across sex, education, marital status, and age groups.
7. Credit profile analysis — inspect credit-limit and age distributions.
8. Repayment behavior — analyze monthly repayment status and delayed-payment patterns.
9. Bills and payments — compare monthly bill and payment patterns by outcome.
10. Correlation and segment comparison — summarize associations and compare descriptive profiles.
11. Interactive dashboard — filter the data by outcome and selected customer characteristics.
12. Evidence-based findings — generate summary observations from the loaded data.
Selected observations
The figures below are descriptive results from the notebook's executed analysis, not predictions.
Observation	Result
Clients in the dataset	30,000
Variables in the combined analysis table	24
Missing values reported	0
Duplicate rows reported	35
Observed next-month default rate	22.12%
Default rate for the up-to-50K credit-limit group	31.79%
Default rate among clients with six delayed months	70.32%
Correlation between MONTHS_DELAYED and DEFAULT	0.398


Interpretation: The notebook observes higher default rates in some groups with lower credit limits and more delayed payments. These are associations within this dataset; they do not establish that one factor causes another. Duplicate rows are reported as a data-quality observation and are not silently removed.
Repository structure
credit-exploratory-data-analysis/
├── CEDA.ipynb       # Complete exploratory analysis and interactive dashboard
├── README.md        # Project overview, methodology, findings, and setup
├── requirements.txt # Python dependencies
└── .gitignore       # Common Python and Jupyter generated files to exclude
Run the notebook
Option 1 — Google Colab (recommended)
1. Open CEDA.ipynb in Google Colab.
2. Run the notebook cells from top to bottom.
3. The setup cell checks for required packages and installs any that are missing.
4. The data-loading cell retrieves the dataset directly from UCI.
Option 2 — Run locally
Use Python 3.10 or later, then run:
git clone https://github.com/abhishekpal8146/credit-exploratory-data-analysis.git
cd credit-exploratory-data-analysis

python -m venv .venv
Activate the environment:

Windows PowerShell
.venv\Scripts\Activate.ps1
macOS / Linux
source .venv/bin/activate
Install dependencies and launch Jupyter:
pip install -r requirements.txt
jupyter notebook CEDA.ipynb
Run the cells from top to bottom. An internet connection is required to retrieve the UCI dataset. The interactive dashboard is intended to run in a live Jupyter environment; GitHub's notebook preview is static.
Tools and libraries
- Python — analysis language
- Pandas — data loading, transformation, and summaries
- NumPy — numerical operations
- Matplotlib and Seaborn — charts and statistical visualizations
- ucimlrepo — access to the UCI Machine Learning Repository
- ipywidgets — interactive dashboard controls
- Jupyter Notebook — executable analysis environment
Scope and limitations
- This is an exploratory and descriptive analysis project; it does not train or evaluate a credit-default prediction model.
- Correlation and group-level default rates indicate associations, not causation.
- The analysis reflects the dataset provided by UCI and should not be treated as current population-wide credit-risk evidence.
- The dataset contains historical client records. Interpret demographic and financial patterns in their original data context.
- The interactive dashboard requires a compatible live Jupyter environment.
Author
Abhishek Pal
- GitHub: @abhishekpal8146
- LinkedIn: Abhishek Pal
If you find this project useful, feel free to explore the notebook and share feedback.
