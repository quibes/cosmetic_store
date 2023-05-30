<h1>Shopping Behaviors Data Analysis Project</h1>

<p>This project focuses on the analysis of shopping behaviors and the organization of a database to manage relevant data. The project spans three months and tracks the purchases made in physical stores.</p>

<h2>Database Description</h2>

<p>Our database comprises of four tables: <strong>product</strong>, <strong>shop</strong>, <strong>purchase</strong>, and <strong>purchase_items</strong>.</p>

<h3>Product</h3>
<p>This table is responsible for holding information about all products sold in shops. The fields are:</p>
<ul>
<li>id</li>
<li>title</li>
<li>category_1</li>
<li>category_2</li>
<li>category_3</li>
<li>brand</li>
</ul>
<h3>Shop</h3>
<p>This table stores data related to physical shops. The fields are:</p>
<ul>
<li>id</li>
<li>address</li>
</ul>
<h3>Purchase</h3>
<p>The <strong>purchase</strong> table contains information about purchases made by customers. The fields include:</p>
<ul>
<li>id</li>
<li>user_id</li>
<li>transaction_type</li>
<li>purchase_date</li>
<li>processed_at</li>
<li>gross_transaction_amount</li>
<li>net_transaction_amount</li>
<li>connected_transaction_id</li>
<li>shop_id</li>
</ul>
<h3>Purchase Items</h3>
<p>This table keeps a record of individual items that were purchased, with relevant details such as product, amount, and price for each item. The fields are:</p>
<ul>
<li>id</li>
<li>purchase_id</li>
<li>product_id</li>
<li>amount</li>
<li>price</li>
<li>discount</li>
<li>marketing_rule</li>
</ul>
<h2>Challenges Faced</h2>
<h3>Data Organisation</h3>
<p>The initial dataset was organised into three separate files: purchases, purchase items, and product base. To enhance data efficiency and integrity, shop addresses were extracted from the purchases table and were stored separately in the shop table, with only the shop id retained in the purchase table.</p>
<h3>Constraint Issues</h3>
<p>During the database creation, several constraints such as uniqueness of id and the existence of purchase id in the purchase item list were applied. Transactions that failed to meet these constraints were excluded from the table.</p>
<h3>Documentation</h3>
<p>The original database lacked substantial documentation, including headers, making it difficult to comprehend the dataset.</p>
<h2>Conclusion</h2>
<p>Despite the challenges encountered, this project resulted in a well-structured and robust database for analyzing shopping behaviors. With the data organized and explained, we now have a solid foundation for ongoing data analysis.</p>
