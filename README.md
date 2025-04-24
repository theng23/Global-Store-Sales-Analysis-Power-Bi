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


- Sales Growth → Increased from 0.64M (2011) to 1.26M (2014), showing consistent expansion.
- Top Markets → APAC (1.07M) leads in sales, followed by EU (0.86M) and US (0.66M).
- Customer Segments → Consumers (1.93M) generate the highest revenue, with Corporate (1.13M) and Home Office (0.69M) also contributing.
- Return Orders → 337 returns, with APAC (50 returns) and LATAM (21 returns) being key regions to monitor.



### 4. Trending
**Trending of Sales**

![651402e6-d1b5-42d4-9d48-a6bf84ddfdf7](https://github.com/user-attachments/assets/abbe43ad-e9ae-4750-b392-ccd6c4c82b76)

- Strong Sales Growth → Sales increased from 1.68M (2011) to 3.21M (2014), reflecting continuous business expansion.
- APAC Leads Market Performance → With 2.7M in sales, APAC shows the highest revenue, followed by EU (2.1M) and US (1.8M).
- Technology Category Dominates → Sales reached 1.26M in 2014, outperforming Furniture and Office Supplies.
- Consumer Segment Drives Revenue → 1.60M in 2014, indicating strong customer engagement compared to Corporate and Home Office.



**Trending of Profit**

![36b080db-ab9f-4bfc-aa67-5dbd21ac6839](https://github.com/user-attachments/assets/f0a9b834-4889-4aad-84c2-4b5ac99155f4)

- Profit growth accelerated → Profit increased from 0.18M (2011) to 1.09M (2014), with the highest jump in 2013.
- Technology outperforms other categories → Profit grew from 93K (2011) to 184K (2014), showing strong demand.
- APAC leads market performance → Profit hit 0.33M, followed by EU (0.25M) and US (0.22M), making APAC the top contributor.
- EMEA shows exceptional profit growth → Despite lower total profit (0.03M), its 134% growth rate suggests a high-potential emerging market.


**Trending of Orders**
![c0339988-c0c8-4f85-a7f0-5be052c10651](https://github.com/user-attachments/assets/ea0f3e8d-45e3-43d5-9884-2b68c4121f66)

- Strong Order Growth → Orders increased 51.69%, reaching 25K total orders, reflecting solid customer demand.
- APAC Leads Orders Growth → APAC saw the highest order volume (5.4K orders, 53.07% growth), signaling a dominant market presence.
- Furniture Orders Increased Steadily → Grew from 2.2K (2011) to 4.3K (2014), showing consistent demand for furniture products.
- Consumer Segment Drives Purchases → Orders grew sharply from 2K (2011) to 4.4K (2014), confirming strong engagement among individual buyers.

**Trending of Return Orders**

![b4f723a1-003e-4318-a747-0382ca00f469](https://github.com/user-attachments/assets/bd2415aa-2174-469a-9a2b-35be7810a78a)


- Steady Increase in Return Orders → Growth rate remained around 0.22 - 0.23 yearly, with total return orders reaching 1K.
- Market Distribution of Returns → EU (0.543) and US (0.539) show the highest return order growth, suggesting potential service or product quality concerns.
- Office Supplies Have the Highest Returns → 173 return orders in 2014, outpacing Furniture (116) and Technology (99), signaling possible product issues.
- Consumer Segment Drives Most Returns → 203 returns in 2014, compared to Corporate (122) and Home Office (63), emphasizing the need for improved customer experience and retention strategies.

## Recommendation
* Expand in High-Performing Regions → APAC, EU, and US show strong revenue growth, so further investment in targeted promotions could maximize opportunities.
* Leverage Technology Demand → Technology consistently outperforms other categories, suggesting more inventory optimization and enhanced marketing strategies.
* Recommendations by Category
	- Technology
 		- Focus on product innovation and targeted digital marketing.
 		- High returns in APAC & LATAM suggest a need for better customer service and quality control measures.
 	- Furniture
  		- Implement personalized recommendations and promotions to increase conversion rates.
  		- Expand in APAC & LATAM because these rigions exhibit strong sale potential.
  	- Office Supplies
	  	- Office Supplies have the highest return orders, requiring product quality improvements and clearer descriptions.
	  	- Encourage businesses to purchase in bulk through corporate packages and discounts.
* Encourage Higher Order Values → Promising & Cannot Lose Them segments show strong potential for increased spending; cross-sell and upsell strategies can drive revenue.
* Improve Customer First Impressions → Engaging New Customers with seamless service and personalized follow-ups can foster long-term retention.
