# Global Store Sales Analysis| Power BI
## I. Introduction
### 📖 What is this project about?
- Senior manager wants to grasp information about the company's business situation to devise a market expansion strategy and decide on strategic product selection.
- From this report he can identify the market and come up with better strategies and products
### 👤 Who is this project for?
➡️ **The Sales Managers** can make data-driven decisions on expansion strategies
### ❓Business Questions:
- How can we leverage data-driven insights to enhance business performance and support market expansion?
- Which product category is the most dominant? Which area has the product category that needs more attention?
- Grasp the business trends of the years through growth.
## II. Dataset
- Dataset for this topic: [**Dataset**](https://drive.google.com/drive/folders/1Qo6H6D1tSZq0FDsOPBx5dNLj6TlxikNY?hl=vi)
- Dataset stores sales information of some products of a company worldwide\
1️⃣ Consists of 3 data tables:
  - Table 1: Orders - Fact order
  - Table 2: People - Information of Sales person
  - Table 3: Return - Information of Return orders
  
2️⃣ Detail dataset

<details> 
<summary>Table 1: Orders</summary>

| Field Name | Data Type | Description |
|-------|-------|-------|
| Order ID          | 	INTEGER          | A unique identifier for each order.                         |
| Order Date        | DATETIME     | The date when the order was placed.                         |
| Ship Date         | DATETIME     | The date when the order was shipped.                        |
| Ship Mode         | STRING | The method or mode of shipping used for the order.          |
| Customer          | STRING | The name or identifier of the customer who placed the order.|
| Customer Segment  | STRING | The segment or category to which the customer belongs.      |
| City              | STRING | The city where the customer is located.                     |
| State             | STRING | The state where the customer is located.                    |
| Country           | STRING | The country where the customer is located.                  |
| Postal Code       | nvarchar(20) | The postal code of the customer's location.                 |
| Market            | STRING | The market or region where the order was placed.            |
| Region            | STRING | The specific region within the market where the order was placed. |
| Product ID        | 	INTEGER          | A unique identifier for each product in the order.          |
| Category          | STRING | The category to which the product belongs.                  |
| Sub-Category      | STRING | The sub-category to which the product belongs.              |
| Product Name      | STRING| The name of the product.                                    |
| Sales             | 	INTEGER        | The total sales amount for the order.                      |
| Quantity          | INTEGER          | The quantity of products ordered.                          |
| Profit            |	INTEGER       | The profit earned from the order.                          |


</details>

<details> 
<summary>Table 2: Returns</summary>

| Field Name | Data Type | Description |
|-------|-------|-------|
|Returned|BIT|Indicates if the order was returned.|
|Order ID|INTEGER|A unique identifier for each order.|		
		
</details>


<details> 
<summary>Table 3: People</summary>
  
| Field Name | Data Type | Description |
|-------|-------|-------|
|Person|STRING|The name of the person.|
|Region|STRING|The region where the person is located.|

</details>

3️⃣ Data Relationships:


## 🧠III. Design Thinking Method
Here are the five steps of design thinking:
### Step 1 - Empathize
➡️ Applied 5W1H to define the problem
![b85a174f-9a53-4d4a-bbb5-766493ebaa6c](https://github.com/user-attachments/assets/57a92cbd-193a-4f8d-8abd-e91983364d97)

➡️ Empathy for Stakeholders

![5e3ec47a-cf66-4e96-9e22-f41e2bdbe8ba](https://github.com/user-attachments/assets/e29726b9-16ea-42e1-8e14-362477961bad)


### Step 2 - Define POV
➡️ Find the North star metric

![a60ad506-23d1-4151-94e2-3b7addfe7d5e](https://github.com/user-attachments/assets/156c5991-fdae-4d5a-90ac-d8fa1b4fa4a7)

➡️ Define Point of View

![f859a614-ec97-470a-9531-a2e3ac860c99](https://github.com/user-attachments/assets/444123a4-5803-4653-99af-92383d9823f2)

➡️ Growth Formula

![9241150e-247c-4c86-a93c-6ef9f23d0939](https://github.com/user-attachments/assets/46bc8f4c-0d5c-43a4-816d-f7041f25f0c8)



### Step 3 - Ideate

➡️ Brainstorming

![3736b524-ddfa-42d9-8490-c53cda2d5b23](https://github.com/user-attachments/assets/e4b2ecff-516f-4d72-a7d9-622e0332914e)



➡️ Structure Idea

![4e00e5d4-8eb4-44c3-9bfe-ad9acd75b7c9](https://github.com/user-attachments/assets/72f618ff-f8e2-414f-8f74-3cfe42acb144)



### Step 4-5 - Prototype & Review

![Step4-5](https://github.com/user-attachments/assets/37f97b59-0fd7-4039-8dcc-ace6629ae6b0)

## III. Visualization
### 1. Overview

![Overview](https://github.com/user-attachments/assets/9ae52045-b5de-41cc-bf89-d379c68a3d62)

### 2. Sale by Location
![Sale by Location](https://github.com/user-attachments/assets/cccee9d3-64c8-4cc3-a173-c5f467595677)

### 3. Sale by Customer

![Sale by Customer](https://github.com/user-attachments/assets/d94fa99f-ced7-4b49-b241-c22bc3aa7888)

### 4. Profit & Return
![Profit   Return](https://github.com/user-attachments/assets/1fdbdd6b-8f5f-4507-9612-84769b72fa95)

## Recommendation & Insight

### Insight 
- Revenue and profit trends
  - 2012 had the highest revenue (3.2M USD), but then gradually decreased in 2013 (2.6M USD) and 2014 (2.0M USD).
  - Profit fluctuates quarterly, with peaks in Q2 2012 and Q3 2013, but a decline in Q4 2014.

- Performance by market 
  - APAC, LATAM and US have the highest number of orders.
  - Central and North Asia are the most profitable, suggesting expansion potential. LATAM, APAC and US have the highest return order rates.
  
- Customer segmentation 
  - Consumer is the largest customer group (51.59%), but also has the highest return rate (51.11%).
  - Corporate and Home Office have lower but more stable order rates. \
    
- Product catalog
  - Office Supplies has the highest number of orders, but Technology has the highest profit margin (42.06%).
  - Furniture has the lowest profit margin (19.25%), need to consider adjustment strategy.
  - Staples, Eldon File Cart are best-selling products. 
- Shipping method
  - Standard Class is the most used (~7.5K orders), while Same Day and First Class are less popular.
  - Expedited shipping may need to be improved for high-value orders or business customers.


### Recommendation
* Restore revenue growth by implementing marketing and sales campaigns in low-performing quarters.
* Expand business in Central and North Asia, because these are the two most profitable regions.
* Reduce return rates in LATAM, APAC and US by improving quality control and after-sales service.
* Focus on Corporate and Home Office customers to increase stable revenue, instead of just depending on Consumer.
* Promote sales of technology products, because they have the highest profit margin (42.06%), and optimize the strategy for Furniture.
* Improve logistics and shipping services, especially enhancing fast shipping for high-value orders.
