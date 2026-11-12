# Debugging_Code
Sharpened your debugging skills to enhance sales data accuracy

## Sales Data Quality: Defensive Python Functions with Custom Exception Handling | Python, pandas

Hardened two sales-analysis functions so bad data raises clear, specific errors instead of silently producing wrong totals or crashing. On a 25-column sales dataset, the corrected code returns a verified total of 98985 units ordered.

# CONTEXT
Business decisions rely on sales analytics, but results are only as reliable as the code behind them. The starting functions broke on missing values, wrong data types and impossible values such as negatives.

# MY ROLE
I read the error messages, identified the failure cases and added the exception handling.

# WHAT I DID
• Reproduced runtime and logic errors in get_quantity_ordered_sum() and get_price_each_average() by testing them on messy input
• Added input validation with try/except and informative error messages for: empty input, non-numeric types, missing values, negative values, division by zero
• Checked that data quality issues in quantity_ordered and price_each were caught before they could distort results
• Re-ran the corrected functions on the full dataset and stored the output as total_quantity_ordered (int)

# RESULTS
• Total quantity ordered: 98985 units
• Average price each: 83.63 $
• Both functions now fail loudly with a clear message on bad input, rather than returning a misleading number

# TECH STACK
Python, pandas, exception handling (try/except, raise)
