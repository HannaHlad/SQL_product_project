# SQL_product_project

In this project, I will be working with a delivery service that has recently entered the market. Orders can be placed through the app or the web version.

I plan to calculate all the necessary metrics, create charts and dashboards based on them, and generate insights to improve the service’s efficiency.

Let’s take a look at the data we will be working with. We have a relational database:

![Relation_table](https://github.com/user-attachments/assets/1777fcf4-8c76-4c6a-95f8-5b6cd6cdc9cd)

**Structure and contents of the tables:**

**user_actions** — user interactions with orders.

| Column Name | Data Type     | Description                                                        |
|-------------|---------------|--------------------------------------------------------------------|
| user_id     | INT           | ID of the user                                                    |
| order_id    | INT           | ID of the order                                                   |
| action      | VARCHAR(50)   | User's action with the order; 'create_order' = create, 'cancel_order' = cancel |
| time        | TIMESTAMP     | Time the action was performed                                     |


**courier_actions** — courier interactions with orders.



| Column         | Data Type     | Description                                                                 |
|----------------|---------------|-----------------------------------------------------------------------------|
|  courier_id    |  INT          | Courier ID                                                                  |
|  order_id      |  INT          | Order ID                                                                    |
|  action        |  VARCHAR(50)  | Courier's action: `'accept_order'` — order accepted, `'deliver_order'` — order delivered |
|  time          |  TIMESTAMP    | Timestamp of the action                                                     |


**orders** — information about orders.

| Column Name   | Data Type     | Description                              |
|---------------|---------------|------------------------------------------|
| order_id      | INT           | ID of the order                          |
| creation_time | TIMESTAMP     | Time the order was created               |
| product_ids   | integer[]     | List of product IDs included in the order |

**users** — information about users.

| Column Name | Data Type   | Description                                                       |
|-------------|-------------|-------------------------------------------------------------------|
| user_id     | INT         | ID of the user                                                    |
| birth_date  | DATE        | Date of birth                                                     |
| sex         | VARCHAR(50) | Gender; 'male' = male, 'female' = female                      |

**couriers** — information about couriers.

**products** — information about the products delivered by the service.

