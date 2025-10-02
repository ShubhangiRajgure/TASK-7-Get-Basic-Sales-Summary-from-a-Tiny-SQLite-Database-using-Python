# TASK-7-Get-Basic-Sales-Summary-from-a-Tiny-SQLite-Database-using-Python
# Sales Data Analysis (SQLite + Python)

This project demonstrates how to use **SQLite** and **Python** to store, query, and visualize sales data.  
It is a simple end-to-end example that works in both **Jupyter Notebook and `.py` scripts**.

## Project Workflow

1. **Create Database**
   - A SQLite database file `sales_data.db` is created.
   - A table `sales` is defined with the following fields:
     - `id` (Primary Key, Auto Increment)
     - `product` (Text)
     - `quantity` (Integer)
     - `price` (Real)

2. **Insert Sample Data**
   - Example sales records for products like **Laptop, Phone, Headphones, and Tablet** are inserted.
   - Each record stores the product name, quantity sold, and unit price.

3. **Run SQL Query**
   - A SQL query is executed to calculate:
     - **Total Quantity Sold** (`SUM(quantity)`)
     - **Total Revenue** (`SUM(quantity * price)`)
   - Results are grouped by product.

4. **Load Results in Pandas**
   - The query result is loaded into a Pandas DataFrame for easy handling.
   - Data is printed to the console using print(df).

5. **Visualization**
   - A bar chart is created using matplotlib to show Revenue by Product.
   - The chart can also be saved as an image (sales_chart.png).

**Requirements**
- Python 3.x
- Libraries:
  * sqlite3 (built-in)
  * pandas
  * matplotlib
