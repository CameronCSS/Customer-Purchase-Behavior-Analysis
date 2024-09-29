<a name="readme-top"></a>




## About The Project

**Description:** This dataset contains sales transaction records for an electronics company over a one-year period, spanning from September 2023 to September 2024. 
It includes detailed information about customer demographics, product types, and purchase behaviors.


### Objectives
The goal of this project is to conduct an in-depth analysis to uncover key insights that can inform business strategies:

#### Insights and recommendations are provided covering the following key areas:

- Sales Trend Analysis: Evaluation of historical sales patterns by month and by products, focusing on revenue and Average Order Value (AOV)
- Product Performance: an Analysis on various products to understand their impact on sales and returns.
- Loyalty Program Success: Assessment of loyalty membership
- Customer Demographics Comparisons: high level comparison of sales and orders by different customers and how their metrics compare to the overall business

#### Significance
The insights derived from this analysis will help optimize marketing efforts, enhance customer engagement, and drive sales growth in the company's electronics category.


<br>
<br>

Detailed code analysis and findings are documented in this [notebook](https://www.kaggle.com/code/cameronseamons/customer-purchase-behavior-analysis)

<br>

><p align="left"><a href="#insights"> ➡️ Jump straight to the insights 💡</a></p>
>
><p align="left"><a href="#recommend"> ✅ View my Recommendations</a></p>
>

<br>

## Data Structure Overview:
The Electronic Sales Database contains both numeric and categorical data, capturing essential customer and transaction details.

<details>
  <summary>Click to View Data Details</summary>
  <br>
  
- Customer ID: Unique identifier for each customer.
- Age: Age of the customer (numeric)
- Gender: Gender of the customer (Male or Female)
- Loyalty Member: (Yes/No) (Values change by time, so pay attention to who cancelled and who signed up)
- Product Type: Type of electronic product sold (e.g., Smartphone, Laptop, Tablet)
- SKU: a unique code for each product.
- Rating: Customer rating of the product (1-5 stars) (Should have no Null Ratings)
- Order Status: Status of the order (Completed, Cancelled)
- Payment Method: Method used for payment (e.g., Cash, Credit Card, Paypal)
- Total Price: Total price of the transaction (numeric)
- Unit Price: Price per unit of the product (numeric)
- Quantity: Number of units purchased (numeric)
- Purchase Date: Date of the purchase (format: YYYY-MM-DD)
- Shipping Type: Type of shipping chosen (e.g., Standard, Overnight, Express)
- Add-ons Purchased: List of any additional items purchased (e.g., Accessories, Extended Warranty)
- Add-on Total: Total price of add-ons purchased (numeric)

</details>


**Entity Relationship Diagram:**

![ERD Customer Data](https://github.com/user-attachments/assets/feaf00b1-59c6-4e2d-bd1a-de81f3ba6e03)


Total row count: 20,000 Records

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="insights"></a>
# Insights

## 1. Sales Performance

Total revenue from completed sales: **42,629,615.57**.

**Revenue by Product Type:**
<br>

| Product Type | Total Revenue      |
|--------------|---------------------|
| **Smartphone** | 14,407,835.84    |
| **Smartwatch** | 9,398,591.23     |
| **Laptop**     | 8,365,905.25     |
| **Tablet**     | 7,722,632.25     |
| **Headphones** | 2,734,651.00     |

<br>

Smartphones dominate our sales, accounting for **33.8%** of total revenue, indicating strong market demand.

## 2. Customer Demographics

Our products appeal to a broad age range (18-80 years). Gender distribution is relatively even for smartphones, but there’s a male preference for tablets and smartwatches.

**Top Product Orders by Gender:**

| Product Type        | Count |
|---------------------|-------|
| **Smartphone (Male)**   | 2998  |
| **Smartphone (Female)** | 2980  |
| **Tablet (Male)**       | 2088  |
| **Smartwatch (Male)**   | 2033  |
| **Tablet (Female)**     | 2016  |

## 3. Loyalty Program Impact

Extended Warranty purchase rate is higher for Non loyalty members. 

This suggests we do not have enough benefits for loyalty members and should focus our loyalty efforts on extra benefits.


**Average Order Value (AOV) by Loyalty Status:**

| Loyalty Status   | AOV       |
|------------------|-----------|
| **New Member**    | 3,237.40  |
| **Non Member**    | 3,192.94  |
| **Churned**       | 3,182.00  |
| **Regular Member** | 3,092.65  |

New members have the highest AOV, suggesting a need to revitalize our loyalty program.

## 4. Order Status and Seasonal Trends

Cancellation rate: **32.84%**, which is concerning.

**Seasonal Revenue:**

| Season | Total Revenue      |
|--------|---------------------|
| **Summer** | 13,305,374.29     |
| **Spring** | 12,989,365.54     |
| **Winter** | 9,723,550.84      |
| **Fall**   | 6,611,324.90      |

Sales peak in January 2024, with May and August close behind. Sales dip from September through December.

## 5. Add-ons and Shipping Impact

**Orders without add-ons have a higher AOV:**

| Add-ons Purchased | AOV       |
|-------------------|-----------|
| **No Add-ons**    | 3,198.85  |
| **With Add-ons**  | 3,083.23  |

Expedited shipping is the star of the show!

Expedited has the lowest percentage of Total orders, but has the second highest revenue. 

Expedited shipping has a **$627 higher AOV** than standard shipping.

<br>


## 6. Payment Methods and Customer Behavior

Credit cards and PayPal are equally popular. Bank transfers show a **$500 higher average spend** but also an **8% higher cancellation rate**.

Impulse items are popular across most age groups. The **25-34** and **55-64** age groups purchase more accessories, while the **35-44** age group has the highest percentage of warranty add-ons.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="recommend"></a>
## ✅ Recommendations

1. **Revamp the Loyalty Program**
   - Incentivize higher spending among regular members.
   - Consider tiered benefits and additional warranty options.

2. **Investigate Cancellation Rates**
   - Focus on root causes of the high cancellation rate.
   - Improve order fulfillment, product descriptions, and customer communication to reduce cancellations.

3. **Targeted Marketing Campaigns**
   - Develop campaigns for the fall and winter seasons, particularly for November and December, to align with typical retail high-sales periods.

4. **Reassess Add-on Strategy**
   - Personalize add-on offers based on customer purchase history and preferences.

5. **Exclusive Benefits for Loyalty Members**
   - Offer loyalty members exclusive benefits like free expedited shipping or discounted extended warranties.
   - Target the **35-44 age group**, who show higher interest in warranties.

6. **Age-Specific Marketing Strategies**
   - Focus on accessories for the **25-34** and **55-64 age groups**.
   - Emphasize warranties for the **35-44 age group**.

7. **Address Bank Transfer Cancellations**
   - Investigate the higher cancellation rate for bank transfer orders.
   - Consider offering incentives or guarantees to encourage this high-value payment method while mitigating risks.

8. **Gender-Specific Marketing Strategies**
   - Develop strategies for non-smartphone categories to balance out the current male-skewed purchases in tablets and smartwatches.

<br>

#### By implementing these recommendations, we can optimize our sales strategy, enhance customer satisfaction, and drive growth across all product categories and customer segments.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

----

<a name="Contact"></a> 
## <a href="https://camdoesdata.com/#contact">Contact Me</a>

  </table>
  <p style="margin-left: auto;">
    <a href="https://drive.google.com/file/d/1YaM4hDtt2-79ShBVTN06Y3BU79LvFw6J/view?usp=sharing" target="_blank" rel="noopener noreferrer">
      <img src="https://user-images.githubusercontent.com/121735588/215364205-abdfc0ac-53db-4733-8d43-b57c1bafb802.png" alt="Resume button">
    </a>
  </p>
</div>


<p align="right">(<a href="#readme-top">back to top</a>)</p>
