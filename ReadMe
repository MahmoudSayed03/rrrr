# Sales Data Warehouse

## Overview

This project involves the development of a Sales Data Warehouse, designed to capture and analyze sales transactions through a star schema. The schema includes one fact table and several dimension tables to support detailed analysis and reporting.

## Schema

### Fact Table: SalesFact

The `SalesFact` table is the core of the data warehouse schema, containing transactional data related to sales orders.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| RowID           | Unique identifier for each row in the fact table    | INT                 |
| OrderID         | Unique identifier for each order                    | VARCHAR(255)        |
| DateKey         | Foreign Key referencing `DateDim.DateKey`            | INT                 |
| CustomerKey     | Foreign Key referencing `CustomerDim.CustomerKey`    | INT                 |
| ProductKey      | Foreign Key referencing `ProductDim.ProductKey`      | INT                 |
| GeographyKey    | Foreign Key referencing `GeographyDim.GeographyKey`  | INT                 |
| ShipModeKey     | Foreign Key referencing `ShipModeDim.ShipModeKey`    | INT                 |
| Sales           | Sales amount for the order                           | DECIMAL(10, 2)      |
| Quantity        | Quantity of products sold                           | INT                 |
| Discount        | Discount applied to the order                        | DECIMAL(5, 2)       |
| Profit          | Profit from the order                                | DECIMAL(10, 2)      |

### Dimension Tables

#### DateDim Table

Stores detailed information related to dates.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| DateKey         | Unique identifier for the date                      | INT                 |
| OrderDate       | Date the order was placed                           | DATE                |
| ShipDate        | Date the order was shipped                          | DATE                |
| Year            | Year component of the order date                    | INT                 |
| Quarter         | Quarter component of the order date                 | INT                 |
| Month           | Month component of the order date                   | INT                 |
| Day             | Day component of the order date                     | INT                 |
| DayOfWeek       | Day of the week component of the order date         | VARCHAR(10)         |

#### CustomerDim Table

Stores information related to customers.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| CustomerKey     | Unique identifier for the customer                  | INT                 |
| CustomerID      | Unique identifier for the customer                  | VARCHAR(255)        |
| CustomerName    | Name of the customer                                | VARCHAR(255)        |
| Segment         | Segment to which the customer belongs               | VARCHAR(255)        |

#### ProductDim Table

Stores information related to products.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| ProductKey      | Unique identifier for the product                   | INT                 |
| ProductID       | Unique identifier for the product                   | VARCHAR(255)        |
| Category        | Category of the product                             | VARCHAR(255)        |
| SubCategory     | Sub-category of the product                         | VARCHAR(255)        |
| ProductName     | Name of the product                                 | VARCHAR(255)        |

#### GeographyDim Table

Stores geographical information related to orders.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| GeographyKey    | Unique identifier for the geographical area         | INT                 |
| Country         | Country where the order was placed                  | VARCHAR(255)        |
| City            | City where the order was placed                     | VARCHAR(255)        |
| State           | State where the order was placed                    | VARCHAR(255)        |
| PostalCode      | Postal code of the order                            | VARCHAR(20)         |
| Region          | Region where the order was placed                   | VARCHAR(255)        |

#### ShipModeDim Table

Stores information related to shipping modes.

| **Column**      | **Description**                                      | **Data Type**       |
|-----------------|------------------------------------------------------|---------------------|
| ShipModeKey     | Unique identifier for the shipping mode             | INT                 |
| ShipModeID      | Unique identifier for the shipping mode             | VARCHAR(255)        |
| ShipModeName    | Name of the shipping mode                           | VARCHAR(255)        |

## Getting Started

To get started with this project, you can clone the repository and follow the instructions provided in the `docs/` directory for setting up the database schema and loading the data.

```bash
git clone https://github.com/yourusername/sales-data-warehouse.git
cd sales-data-warehouse
