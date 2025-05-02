https://regex101.com/

📊 Introduction to Data Manipulation
Definition: Adjusting, structuring, or formatting data to make it more usable and readable.
Reference: Chatterjee & Segev (1991)

🐼 Pandas Overview
Open-source Python library for data manipulation and analysis.

Core components:

DataFrame: 2D table (like a spreadsheet).

Series: 1D labeled array.

Data Loading
read_csv(), read_excel(), read_json(), read_sql(), etc.

Useful methods:

head(), tail() – preview rows

describe() – summary statistics

🛠️ Data Manipulation in Pandas
Filtering & Sorting
Boolean indexing to filter rows.

sort_values() to sort by column(s).

Basic Transformations
Add/drop columns, rename, change data types (astype()).

Handling Missing & Duplicate Data
dropna() – remove missing values

fillna() – fill in missing values

.duplicated() and .drop_duplicates() – remove duplicates

📦 Data Wrangling
Cleaning: Handle missing/duplicate values, fix formats

Filtering: Extract relevant subsets

Transforming: Reshape data for analysis or visualization

🔁 Grouping and Aggregation
groupby() – group data by column(s)

Aggregation functions: sum(), mean(), count(), etc.

📐 Pivot Tables
pivot_table() to summarize data (like Excel pivot tables)

🔗 Combining DataFrames
merge(), join(), concat(), append() – combine datasets

⏱️ Time Series in Pandas
Data indexed by datetime (e.g., daily stock prices)

Use pd.to_datetime() to convert, pd.date_range() to generate dates

🔍 Regular Expressions (Regex)
What is Regex?
A search pattern used to match, locate, and manage text.

Common use: Validating inputs like email addresses.

Key Symbols:
Symbol	Meaning
^	Start of input
$	End of input
[A-Za-z0-9]	Character range
\s, \S	Whitespace / Non-whitespace
\d, \D	Digit / Non-digit
.	Any character

🧩 PRegEx: A Friendly Alternative to Regex
PRegEx: Write regex patterns in plain English.

Syntax examples:

AnyDigit(), Exactly(4), AnyButWhitespace()

Easier for beginners & collaborative teams

Installed via: pip install pregex==2.0.1 (requires Python ≥ 3.9)

[Uploading L5DE M3T5 V1.pdf…]()
