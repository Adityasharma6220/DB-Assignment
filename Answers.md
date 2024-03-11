Question 1) Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
 
Solution 1)-->
The "Product" and "Product_Category" entities have a one-to-many relationship, where each category can have multiple products associated with it, but each product can only be associated with one category. This relationship is established through the "category_id" attribute in the "Product" table, which is a foreign key referencing the "id" attribute in the "Product_Category" table.

Question 2) How could you ensure that each product in the "Product" table has a valid category assigned to it? 

Solution 2) --> 
To ensure that each product in the "Product" table has a valid category assigned to it, you can implement a foreign key constraint on the "category_id" attribute in the "Product" table, referencing the "id" attribute in the "Product_Category" table. This constraint would ensure that any attempt to insert or update a product record with an invalid category_id value would result in an error.
