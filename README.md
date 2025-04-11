# SQL_product_project

In this project, I will be working with a delivery service that has recently entered the market. Orders can be placed through the app or the web version.

I plan to calculate all the necessary metrics, create charts and dashboards based on them, and generate insights to improve the service’s efficiency.

Let’s take a look at the data we will be working with. We have a relational database:

![Relation_table](https://github.com/user-attachments/assets/1777fcf4-8c76-4c6a-95f8-5b6cd6cdc9cd)

**Structure and contents of the tables:**

**user_actions** — user interactions with orders.
![ChatGPT Image 7 апр  2025 г , 20_51_36](https://github.com/user-attachments/assets/ed8e7b58-b90f-4cc7-b204-8aad730683fd)


**courier_actions** — courier interactions with orders.
### 📄 Table: `courier_actions`

**Description**: Contains the history of couriers’ actions related to orders.

| Column         | Data Type     | Description                                                                 |
|----------------|---------------|-----------------------------------------------------------------------------|
| `courier_id`   | `INT`         | Courier ID                                                                  |
| `order_id`     | `INT`         | Order ID                                                                    |
| `action`       | `VARCHAR(50)` | Courier's action: `'accept_order'` — order accepted, `'deliver_order'` — order delivered |
| `time`         | `TIMESTAMP`   | Timestamp of the action                                                     |


**orders** — information about orders.

**users** — information about users.

**couriers** — information about couriers.

**products** — information about the products delivered by the service.

