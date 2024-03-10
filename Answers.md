# Tanish Basu

## 1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

### Answer

```

The relationship between the Product and Product_Category entities in the above diagram is one to many
which means that one product can belong to many categories,
but a category can only have many products in the given database diagram.

In the database diagram, there is a foreign key called category_id within the Product table.
This foreign key references the primary key id  within the Product_Category table.
This creates the link between the two tables.

```

## 2. How could you ensure that each product in the Product table has a valid category assigned to it?
### Answer

```
To ensure that each product in the Product table has a valid category assigned to it
according to the diagram it follows two patterns which are 

Foreign Key :

Defining a foreign key on the category_id column in the product table
that references the primary key of the product_category table.

This enforces that any value assigned to category_id must exist in the the linked table,
preventing invalid assignment.

Checking Constraint:

Implement checking constraints on the category_id column in the "Product" table.

This constraint can be a list of allowed valid inputs.

Any attempt to insert a product with an invalid information will be rejected.


```
