# Customer Churn Logic
Identifies customers who haven't made a purchase in 100 days.
- **Source:** `dim_customers`, `fact_orders`
- **Logic:** `DATEDIFF(day, last_order_date, CURRENT_DATE) > 100`
- **Definition:** Labeled as 'At Risk' if they have a pending support ticket.
