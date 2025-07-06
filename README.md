# dbt Customer Orders ELT Pipeline

This is a sample dbt project implementing an ELT pipeline for a fictional customer-orders-payments dataset. It is deployed using **dbt Cloud** with **Snowflake** as the data warehouse.

## 🚀 How It Works

1. **Seeds**: Load mock customer, order, and payment data into Snowflake.
2. **Staging Models**: Apply basic transformations, standardize column names.
3. **Marts**:
   - `dim_customers`: One row per customer with lifetime value & order metrics.
   - `fct_orders`: Transaction-level order facts, joined with payments.
4. **Deployment**: Runs scheduled in **dbt Cloud** with environment-specific configs.

### Prerequisites
- A Snowflake account (with a database + schema created)
- A dbt Cloud account

### Common commands

dbt deps
dbt seed
dbt run
dbt test
dbt docs generate && dbt docs serve



