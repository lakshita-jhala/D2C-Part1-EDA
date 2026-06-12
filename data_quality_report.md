# Data Quality Report

## Missing Values
- Missing values observed in selected customer profile and behavioral columns.
- Missing values should be imputed or handled before modeling.

## Duplicate Records
- No significant duplicate customer IDs detected.
- Order IDs appear unique.

## Outliers
- Monetary values show several high-spending customers.
- Delivery days contain extreme values compared to the majority of orders.

## Invalid Values
- No major invalid category values identified.
- Data types were checked and corrected where necessary.

## Join/Key Issues
- customer_id used as primary join key.
- Records successfully merged using customer_id.

## Date Consistency Issues
- Date columns converted to datetime format.
- Order dates occur after signup dates for most customers.

## Leakage Risk Columns
- Churn labels should not be used during feature creation.
- Future behavioral information should be excluded when building predictive models.

## Recommendations
- Handle missing values before modeling.
- Monitor outliers during feature engineering.
- Validate joins after every merge.
- Remove leakage-prone columns from model training.