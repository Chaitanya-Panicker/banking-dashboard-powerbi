# Bank Loan Summary Dashboard

## Project Overview
This project is an interactive dashboard for analyzing bank loan data, providing insights into loan applications, funding, repayments, and borrower demographics. Built on a dataset of 38,576 loans, it visualizes key metrics like total applications (39K), funded amount ($436M), and average interest rate (12%). The dashboard helps identify trends, risks, and performance.

## Key Visualizations
- **Summary Metrics**: Cards showing total applications, funded/received amounts, avg interest rate (12%), and avg DTI (13.3%)
- **Good vs Bad Loans Pie Chart**: 86.18% good loans vs 13.82% bad loans
- **Loan Applications by Home Ownership Bar Chart**: Highest for RENT (18.4K), MORTGAGE (17.2K), OWN (2.8K)
- **Loan Status Table**: Breakdown by status (Fully Paid: 32,145 apps; Current: 1,098; Charged Off: 5,333) with funded/received amounts and rates
- **Monthly Applications Line Chart**: Upward trend from ~2K in Jan to ~4K in Dec
- **Applications by State Map**: Highest in CA (darkest shade), followed by TX, NY, FL
- **Applications by Term Pie Chart**: 73.2% for 36 months, 26.8% for 60 months
- **Applications by Employee Experience Bar Chart**: Most for 10+ years, decreasing for fewer years
- **Applications by Purpose Bar Chart**: Top purposes: Debt consolidation, credit card, home improvement
- **Funded vs Received Bar Chart**: Close alignment, with received slightly higher
- **Details Table**: Loan-level data including ID, purpose, ownership, grade, date, amounts, rates

## Insights and Analysis
- **Loan Performance**: 86% good loans indicate strong portfolio health; charged-off loans (14%) total $65M funded but only $37M received, highlighting $28M loss
- **Borrower Trends**: Renters dominate applications (47%), suggesting targeting homeowners for lower risk. Debt consolidation is the top purpose (~50%), with high approval in CA/TX
- **Temporal Growth**: Applications doubled from Jan to Dec, peaking in summer—potential seasonal marketing opportunity
- **Risk Factors**: Higher interest rates (15%) for current loans; 60-month terms riskier (26.8% share but higher DTI)
- **Recovery Rate**: Overall, received $473M vs funded $436M (108% recovery), but charged-off at 57% recovery signals need for better screening

## Technologies Used
- **Database**: PostgreSQL (managed via pgAdmin) for storing loan data
- **Data Visualization**: Power BI (or Tableau) for creating interactive dashboards with charts, maps, and tables
- **Querying**: SQL for data extraction (e.g., `SELECT * FROM loan;`)
- **Other**: Potential Python (Pandas/Matplotlib) for preprocessing, though not shown

## Project Steps
1. **Data Collection**: Import loan dataset into PostgreSQL table 'loan' with columns like id, address_state, emp_length, grade
2. **Database Setup**: Create schema in pgAdmin, load ~38K records
3. **Data Cleaning**: Handle missing values, format dates/amounts using SQL queries
4. **Dashboard Design**: Build views in Power BI/Tableau—summary cards, charts, map, and details table
5. **Analysis**: Generate insights from aggregations (e.g., SUM funded, AVG rates)
6. **Deployment**: Export dashboard for web/desktop/mobile viewing

## How to Use
1. Clone repo: `git clone <repo-url>`
2. Set up PostgreSQL: Import loan.sql dump into pgAdmin
3. Open dashboard: Load .pbix file in Power BI
4. Filter: Use dropdowns for purpose/grade to explore
5. Query data: Run SQL in pgAdmin for custom analysis

## Contact
For questions, reach out to [your-email@example.com] or open an issue on GitHub.

## License
MIT License - Free to use, modify, and distribute. See LICENSE file for details.
