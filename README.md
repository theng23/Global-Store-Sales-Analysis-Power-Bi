# 📊Global Store Sales Analysis| Power BI
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
## 📂II. Dataset
📌 Dataset for this topic: [**Dataset**](https://drive.google.com/drive/folders/1Qo6H6D1tSZq0FDsOPBx5dNLj6TlxikNY?hl=vi)
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

![7bff3d4c-c733-4b1a-b255-27adc9c3f0a5](https://github.com/user-attachments/assets/d017bcc2-93e4-460b-a22c-e4196357a118)



## 🧠III. Design Thinking Method
Here are the five steps of design thinking:
### Step 1 - Empathize
➡️ Applied 5W1H to define the problem

![2c836ce1-942d-49d1-acc1-630d6e522dfc](https://github.com/user-attachments/assets/c321814b-bf0a-4d06-a700-3e1d0b618de8)


➡️ Empathy for Stakeholders


![cc62559c-9c5c-4136-919e-44d0ede79bd1](https://github.com/user-attachments/assets/6520c7c2-cd6a-4309-8f39-18a78c00ef5e)

### Step 2 - Define POV
➡️ Find the North star metric

![20e25f10-ee44-4813-9cf0-03744ab058ba](https://github.com/user-attachments/assets/153e4406-1e0e-447c-bf51-7be6c9ef0797)



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

![5e5f3e2a-9b43-4e44-a541-a9da319ba7b1](https://github.com/user-attachments/assets/3300d7a3-c7d8-415c-b5d5-dc14906de26a)

- Steady growth in total sales. Sales increased significantly from 2011 (1.68M) to 2014 (3.21M)
- APAC dominates the market. Leading in both sales (2.7M) and orders (5.4K),
- Return orders at 4.7%. Monitoring reasons for returns could help improve product quality and reduce losses.
- 4Strong order volume increase. Orders nearly doubled from 2011 (4.4K) to 2014 (8.5K), showcasing consistent customer demand.
### 2. Sales

![e2940261-302f-4951-8289-66c04b5aa046](https://github.com/user-attachments/assets/313c9441-bcbb-411c-8299-d582a4e24450)

- Strong revenue growth → Sales increased to 9.48M, showing continued business expansion.
- High return order ratio (4.68%) → Addressing reasons for returns could enhance customer satisfaction and reduce losses.
- Technology leads in sales (3.7M) → Indicates high demand; optimizing inventory and marketing for tech products could further boost revenue.
- Top 5 seller: **Staples(91)**, **Eldon File Cart, Single Width(66)**, **Rogers File Cart, Single Width(49)**, **Smead File Cart, Single Width(49)**, **Tenex File Cart, Single Width(48)**

### 3. Analysis
- Overview

![9f64c9de-881c-4e54-b81c-bafe5cc98ae6](https://github.com/user-attachments/assets/0c90c8af-6558-4360-8d11-5dd5dfb0afcd)



**Furniture**

![e907bf1c-2cbb-4b25-ba38-4882fe3f5ade](https://github.com/user-attachments/assets/e8b1c817-f9bf-409f-933d-5b05afa61698)

- Sales Growth → Increased from 0.60M (2011) to 1.09M (2014), indicating rising demand.
- Top Markets → APAC (1.08M) leads in sales, followed by LATAM (0.64M) and EU (0.62M).
- Customer Segments → Consumer (1.70M) dominates, while Corporate (0.99M) and Home Office (0.57M) contribute significantly.
- Profit Margin → 6.65%, suggesting room for optimization in pricing and cost management.
	

**Office Supplies**

![789f9950-ca74-4f39-8bb6-05c48378731f](https://github.com/user-attachments/assets/64a02273-71b4-43a3-a84a-5f4bb297cbb3)

- Sales Growth → Increased from 0.60M (2011) to 1.09M (2014), reflecting rising customer demand.
- Market Leaders → APAC (1.08M) leads in sales, followed by LATAM (0.64M) and EU (0.62M).
- Top Customer Segments → Consumers (1.70M) generate the highest revenue, with Corporate (0.99M) and Home Office (0.57M) also contributing.
- Return Orders → 322 returns indicate a need for better customer experience and product quality improvements.

**Technology**

![ca422dfc-4316-4338-bd42-4e3e17bb8791](https://github.com/user-attachments/assets/488c931e-ecf2-4ac6-b58c-47d81b5edbd7)





### 4. Trending

![651402e6-d1b5-42d4-9d48-a6bf84ddfdf7](https://github.com/user-attachments/assets/abbe43ad-e9ae-4750-b392-ccd6c4c82b76)


![36b080db-ab9f-4bfc-aa67-5dbd21ac6839](https://github.com/user-attachments/assets/f0a9b834-4889-4aad-84c2-4b5ac99155f4)


![c0339988-c0c8-4f85-a7f0-5be052c10651](https://github.com/user-attachments/assets/ea0f3e8d-45e3-43d5-9884-2b68c4121f66)



![26d48cc6-141a-4f55-83d6-5f31a2dc08e0](https://github.com/user-attachments/assets/a1288090-ea6a-48a9-b691-11da0f9d5a0a)


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
