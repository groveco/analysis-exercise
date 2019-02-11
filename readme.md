Data
----

This repo contains a sqlite database with a single "orders" table with the following schema:

```
CREATE TABLE orders(
    order_number INTEGER,
    customer_id INTEGER,
    shipment_date DATE,
    order_value TEXT,
    acquisition_channel_id INTEGER
)
```

A few notes about the data:

- The "order number" field is an ordinal indicating whether this is the customer's first order (1), second order (2), etc.
- Note that order_value is in a string format
- Acquisition Channel ID is an integer indicating what marketing channel the customer was originally acquired from. The Channel ID will be the same for all the customer's orders.

Your Tasks
----------

Please complete the tasks below, and upload all files to a public Github repo.

1) Perform a retention analysis of weekly cohorts that identifies where the biggest drop in the retention curve occurs. You can use any tools/technologies you'd like, though please do at least some of the data processing/analysis in SQL. For instance, do NOT simply run a `SELECT * FROM orders`, export to Excel, and perform the analysis from there. Show a little bit of your SQL chops! Please save any relevant queries to a .sql file, and provide a writeup in a markdown file. Feel free to use Excel, R, or Python as well.

2) Which is the bigger lever for revenue impact: an increase in 3+ order retention of 500 basis points or an increase in 3+ order average order value of $3? Drawing from past experience, which do you think will be easier to achieve and why?

3) Suggest two other data sets you wish you had access to and which analytic techniques you would suggest for mining the overall data set for further insights.
