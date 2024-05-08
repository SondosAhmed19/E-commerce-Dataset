# E-commerce-Dataset

This repository contains an ETL (Extract, Transform, Load) project focused on processing an E-commerce dataset. The goal of this project is to extract data from csv files, perform transformations to ensure data quality and consistency, and load the transformed data into a target database for further analysis.



## Dataset

The E-commerce dataset used in this project consists of customer information, product details, order history, and transactional data. The dataset is provided in CSV format and is located in the `data` directory. It includes the following files:

- `user_dataset.csv`: Contains information about customers, such as customer ID, name, email, and address.
- `products_dataset.csv`: Includes details about the products sold, such as product ID, name, price, and category.
- `order_item_dataset.csv`: Contains order information, including order ID, customer ID, product ID, quantity, and order date.
- `order_dataset.csv`: Contains more information about orders.
- `seller_dataset.csv`: Contains information about seller, such as seller ID, name, email, and address.
- `payment_dataset.csv`:contains payment method for orders.
- `feedback_dataset.csv`:contains feedbacks of users.
  
  
## Data modeling

1-Identify Key Entities:
Determine the essential entities in the eCommerce domain, such as customers, products, orders, payments, inventory, and shipments. These entities represent the core components of an eCommerce system.

2-Define Entity Relationships:
Establish relationships between the identified entities. For example, a customer can have multiple orders, an order can contain multiple products, and a product can be associated with various attributes like category, brand, and price.

3- Capture Data Attributes:
Identify the specific attributes or properties for each entity. For instance, customer attributes might include name, address, email, and phone number. Product attributes could encompass SKU, name, description, price, and stock quantity.

4- Determine Primary Keys and Foreign Keys:
Assign primary keys to uniquely identify each entity. These keys serve as the primary means of referencing and linking data between entities. Foreign keys represent the relationships between entities by referring to the primary key of another entity.

5- Establish Data Types and Constraints:
Define appropriate data types for each attribute, such as string, integer, decimal, or date. Additionally, set constraints and validations to ensure data integrity and consistency, such as unique constraints, not-null constraints, and range checks.

6- Consider Dimensional Modeling:
 make dimensional modeling techniques like star schema. These models facilitate efficient querying and analysis by organizing data into facts (orders) and dimensions (users, product, seller, payment, feedback).
 
7- Plan for Historical Data and Auditing:
Determine how historical data will be managed, as well as any requirements for tracking and auditing changes to the data. This could involve implementing techniques like slowly changing dimensions (SCDs) to capture historical changes in entity attributes.


## ETL Process

The ETL process for this project follows the standard flow of Extract, Transform, and Load:

1. Extraction:
   - The data is extracted from the provided CSV files.
   - The script reads the CSV files and loads the data into memory for further processing.

2. Transformation:
   - Data transformation is performed to ensure data quality and consistency.
   - The script applies cleaning operations, such as removing duplicates, handling missing values, and validating data integrity.
   - It also performs data type conversions, standardization, and enrichment based on predefined rules and business requirements.
   - Transformation steps may also include data aggregation, joining multiple datasets, or creating derived fields.

3. Load:
   - The transformed data is loaded into a target database for storage and analysis.
   - In this project, we use a SQL server database as the target database.
   - The script establishes a connection to the database and creates the necessary tables to store the transformed data.
   - Finally, it inserts the transformed data into the corresponding tables in the database.


## Future Enhancements

This ETL project can be extended and enhanced in several ways:

- Implementing incremental data extraction to handle new data updates efficiently.
- Adding data validation checks and error handling mechanisms.
- Automating the ETL process to run periodically or triggered by specific events.
- Integrating with data visualization tools for generating reports and dashboards.
- Exploring advanced data transformations and analytics on the E-commerce dataset.

Feel free to contribute to this project by suggesting improvements, fixing bugs, or adding new features.

## Contact

If you have any questions or suggestions regarding this project, please feel free to contact the project maintainer at sondosabdalmonsef19@gmail.com

