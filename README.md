# Project-Motoparts

## Introduction

Motoparts is an imaginary company that sells motorcycle parts, and they've asked for some help in analysing their sales data!

They operate three warehouses in Australia, selling both retail and wholesale. They offer a variety of parts and accept credit cards, cash, and bank transfer as payment methods. However, each payment type incurs a different fee.

The board of directors wants to gain a better understanding of wholesale revenue by product line, and how this varies month-to-month and across warehouses. You have been tasked with calculating net revenue for each product line and grouping results by month and warehouse. The results should be filtered so that only `"Wholesale"` orders are included.

They have provided you with access to their database, which contains the following table called `sales`:

<br>

## Schema
| Column | Data type | Description |
|--------|-----------|-------------|
| `order_number` | `VARCHAR` | Unique order number. |
| `date` | `DATE` | Date of the order, from June to August 2021. |
| `warehouse` | `VARCHAR` | The warehouse that the order was made from&mdash; `North`, `Central`, or `West`. |
| `client_type` | `VARCHAR` | Whether the order was `Retail` or `Wholesale`. |
| `product_line` | `VARCHAR` | Type of product ordered. |
| `quantity` | `INT` | Number of products ordered. | 
| `unit_price` | `FLOAT` | Price per product (dollars). |
| `total` | `FLOAT` | Total price of the order (dollars). |
| `payment` | `VARCHAR` | Payment method&mdash;`Credit card`, `Transfer`, or `Cash`. |
| `payment_fee` | `FLOAT` | Percentage of `total` charged as a result of the `payment` method. |

<br>

## Requirements

They have requested the query output be presented in the following format:

| `product_line` | `month` | `warehouse` |	`net_revenue` |
|----------------|-----------|----------------------------|--------------|
| product_one | --- | --- | --- |
| product_one | --- | --- | --- |
| product_one | --- | --- | --- |
| product_one | --- | --- | --- |
| product_one | --- | --- | --- |
| product_one | --- | --- | --- |
| product_two | --- | --- | --- |
| ... | ... | ... | ... |

<br>

## Solution Part 1: PostgreSQL

[Click here to view the Jupyter Notebook solution for part 1](https://github.com/tom-stannard/Project-Motoparts/blob/main/project-motoparts.ipynb), which details my approach to querying the `sales` table and extracting data in the requested format. 

<br>

## Solution Part 2: R & R-Trelliscope

[Click here to view the Jupyter Notebook solution for part 2](/), which details my approach to visualising the various indicators of location and product performance from the previously extracted data.

<br>

## Solution Part 3: Looker Studio

[Click here to view the Dashboard solution for part 3](/), where I have designed and published a scalable performance dashboard in Google Looker Studio based on the original `sales` data. 
