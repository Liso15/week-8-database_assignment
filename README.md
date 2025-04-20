# week-8-database_assignment
#E-commerce Database Design Solution

## Description of the project
-e-commerce app for selling products. Below is the data flow
-Product Hierarchy:
Brands → Products → Product Items
 Categories form a hierarchy (parent/child relationships)
-Variation System:
 Products can have multiple variations (size, color, etc.)
 Each combination becomes a unique Product Item with its own SKU
-Attribute System:
 Flexible attribute system for product specifications
Attributes are categorized and typed for better organization
-Inventory Management:
 Stock levels are tracked at the Product Item level
 Each variation combination has its own inventory count

# insert SQL

Create an ERD
Entities and Attributes
product_image
image_id (Primary Key)
product_id (Foreign Key)
url (URL or file reference)
color
color_id (Primary Key)
name (e.g., Red, Blue)
product_category
category_id (Primary Key)
name (e.g., Clothing, Electronics)
product
product_id (Primary Key)
name
brand_id (Foreign Key)
base_price
category_id (Foreign Key)
product_item
item_id (Primary Key)
product_id (Foreign Key)
variation_id (Foreign Key)
price
quantity
brand
brand_id (Primary Key)
name
description
product_variation
variation_id (Primary Key)
product_id (Foreign Key)
size_option_id (Foreign Key)
color_id (Foreign Key)
size_category
size_category_id (Primary Key)
name (e.g., Clothing Sizes, Shoe Sizes)
size_option
size_option_id (Primary Key)
size_category_id (Foreign Key)
size (e.g., S, M, L, 42)
product_attribute
attribute_id (Primary Key)
product_id (Foreign Key)
attribute_type_id (Foreign Key)
value
attribute_category
attribute_category_id (Primary Key)
name (e.g., Physical, Technical)
attribute_type
attribute_type_id (Primary Key)
attribute_category_id (Foreign Key)
type (e.g., Text, Number, Boolean)
Relationships
A product can have multiple product_images.
A product belongs to one product_category.
A product is associated with one brand.
A product can have multiple product_variations.
A product_variation is linked to one size_option and one color.
A size_option belongs to one size_category.
A product can have multiple product_attributes.
An attribute_type belongs to one attribute_category.

# Screenshot
![Screenshot (6)](https://github.com/user-attachments/assets/5746d683-04c9-4bd6-912e-63edebb868e8)
![Screenshot (7)](https://github.com/user-attachments/assets/22cd07e6-e508-4ee3-947b-c1b61840ba75)

# Technologies used
- Mysqal
- Node.js
- vs code
# By
- Liso Mlunguza - lisomlunguza8@gmail.com

