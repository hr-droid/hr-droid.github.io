# Customer Churn Logic
Identifies customers who haven't made a purchase in 90 days.
- **Source:** `dim_customers`, `fact_orders`
- **Logic:** `DATEDIFF(day, last_order_date, CURRENT_DATE) > 90`
- **Definition:** Labeled as 'At Risk' if they have a pending support ticket.
