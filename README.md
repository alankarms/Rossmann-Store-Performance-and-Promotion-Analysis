# An Analysis of Store Performance Imbalance and Promotion Effectiveness in Rossmann Stores

Business analysis of Rossmann store sales data to identify store-performance differences, evaluate promotion effectiveness, and develop store-level strategic recommendations.

## Project Overview

This project analyses historical sales and store information for 1,115 Rossmann stores using Python.

The analysis focuses on two business objectives:

1. Analyse variation in sales and customer footfall across stores based on store type, assortment, competition distance, holiday conditions, and time patterns.
2. Evaluate promotion effectiveness and recommend strategies for improving store-level sales planning and promotional decision-making.

The final analysis used 844,338 valid operating-day records covering the period from January 2013 to July 2015.

## Key Findings

- Regular promotional days were associated with a 38.77% increase in average sales.
- Customer footfall increased by 21.17% during promotional periods.
- Sales per customer increased by 13.87% during promotions.
- High-promotion-response stores recorded an average sales uplift of 65.23%.
- 87 stores were identified as High-Value Promotion Priority stores.
- 450 stores were classified as Turnaround Priority locations.
- Type B stores recorded the highest average sales and customer footfall.
- Type D stores recorded the highest average sales per customer.
- Extended-assortment stores generally outperformed Basic-assortment stores within comparable store types.
- Promo2 did not show the same short-term sales improvement as regular promotions.

## Strategic Store Segmentation

Stores were classified into five business-focused categories:

- High-Value Promotion Priority
- Strong Core Performer
- High Customer Value Store
- Conversion Improvement Priority
- Turnaround Priority

The segmentation combines store sales, customer footfall, sales per customer, sales variability, and historical promotion response to support differentiated store-level decision-making.

## Analysis Workflow

The project included:

- Data validation and quality checks
- Merging daily sales and store-level datasets
- Missing-value assessment
- Filtering closed and anomalous store records
- Feature engineering
- Descriptive statistics
- Store-type analysis
- Assortment analysis
- Competition-distance analysis
- Holiday analysis
- Weekday and monthly trend analysis
- Promotion uplift analysis
- Promo2 effectiveness analysis
- Individual store-performance analysis
- Store segmentation
- Strategic recommendation framework

## Key Derived Metrics

The analysis created several additional business metrics, including:

- Sales per Customer
- Sales Coefficient of Variation
- Competition Distance Bands
- Promotion Sales Uplift
- Promotion Response Segments
- Store Performance Segments
- Strategic Store Categories

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Dataset

The project uses the publicly available Rossmann Store Sales dataset from Kaggle.

Dataset:
https://www.kaggle.com/competitions/rossmann-store-sales

Primary files used:

- `train.csv`
- `store.csv`

The source dataset does not explicitly specify the currency of the `Sales` variable, so sales values are reported without assigning a currency symbol.

## Repository Structure

```text
Rossmann-Store-Performance-and-Promotion-Analysis/
│
├── data/
│   ├── train.csv
│   └── store.csv
│
├── notebook/
│   └── rossmann_store_analysis_project.ipynb
│
├── outputs/
│   ├── tables/
│   └── plots/
│
├── report/
│   └── rossmann_final_report.pdf
│
├── requirements.txt
└── README.md

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Rossmann-Store-Performance-and-Promotion-Analysis.git
cd Rossmann-Store-Performance-and-Promotion-Analysis
```

2. Create a virtual environment:

```bash
python -m venv venv
```

3. Activate the virtual environment.

On macOS/Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

4. Install the required packages:

```bash
pip install -r requirements.txt
```

5. Download the Rossmann Store Sales dataset from Kaggle:

https://www.kaggle.com/competitions/rossmann-store-sales/data

Place the required files inside the `data/` folder:

```text
data/
├── train.csv
└── store.csv
```

6. Launch Jupyter Notebook:

```bash
jupyter notebook
```

7. Open the project notebook:

```text
notebook/rossmann_store_analysis_project.ipynb
```

8. Run the notebook cells in order.

## Selected Business Insights

Regular promotions were associated with substantially stronger store performance, but the response varied significantly across locations. Type A stores recorded the strongest average promotion uplift, while Type B stores showed a weaker relative response despite higher baseline sales and footfall.

Store performance also followed different operating models. Some stores achieved strong sales through customer volume, while others relied more heavily on higher sales per customer.

The final strategy framework therefore recommends targeted promotion allocation instead of a uniform network-wide approach.

## Business Recommendations

- Prioritise historically high-response stores for regular promotions.
- Protect strong core performers from unnecessary discounting.
- Improve sales per customer in high-footfall underperforming stores.
- Build traffic selectively in high-customer-value stores.
- Review low-sales, low-footfall stores individually before increasing promotional activity.
- Review Promo2 separately from regular promotions.
- Strengthen inventory and staffing preparation during peak periods such as November and December.

## Limitations

This is an observational secondary-data analysis, so the results identify associations rather than causal effects.

The dataset does not include:

- Promotion costs
- Profit margins
- Product-level sales
- Store size
- Staffing levels
- Local demographics
- Detailed competitor characteristics

As a result, promotion profitability and the precise causes of store-level performance differences cannot be determined from this dataset alone.

## Author

Alankar Singh

MSc Data Science, University of Exeter
