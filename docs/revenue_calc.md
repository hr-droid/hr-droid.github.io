# Revenue Transformation
This logic calculates **Gross Revenue** by joining sales headers with line items.
- **Source:** `raw_sales`, `raw_customers`
- **Logic:** `SUM(price * quantity)` excluding returns.
- **Business Rule:** Only include 'Completed' status orders.
