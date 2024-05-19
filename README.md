I've used a database consisting of several tables: customers, transactions, markets, products, and date. To understand the data better, I started with basic queries to view the contents of each table, such as SELECT * FROM customers; which retrieves all customer information.

To get an overview of the data, I used count queries like SELECT COUNT(*) FROM transactions; to count the number of records in the transactions table. I also filtered the data to extract specific information. For instance, SELECT * FROM transactions WHERE market_code="Mark001"; retrieves transactions from a specific market. Similarly, I used conditions to filter transactions with a specific currency or sales amount.

For more detailed analysis, I summarized sales amounts and quantities. For example, SELECT SUM(sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020 AND transactions.currency="INR\r" OR transactions.currency="USD\r"; calculates the total sales amount for 2020 in either Indian Rupees or US Dollars.

Additionally, I explored data visualization using PowerBI, creating pie charts, line charts, and bar charts to visualize various aspects of the data. In PowerBI, I also performed data cleaning to ensure the data was accurate and ready for analysis. This included handling missing values, correcting data types, and removing duplicates.

This comprehensive approach helped me gain insights into the data, identify trends, and make informed decisions based on the cleaned and visualized data.
