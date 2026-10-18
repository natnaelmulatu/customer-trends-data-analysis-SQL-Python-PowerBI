<img src="images/From_Raw_Data_to_Revenue_Growth.png" alt="Logo" width="1000">

# From Raw Data to Revenue Growth: Decoding Consumer Behavior Using Python, SQL & Power BI

<br>

In modern retail, data is rarely the bottleneck—clarity is. E-commerce platforms and storefronts generate thousands of transactional records daily, yet leadership teams frequently struggle with a fundamental question: Which consumer behaviors actually drive long-term value, and where are we leaving money on the table?

<br>

## Why This Project?

As a data analyst, I’ve learned that raw numbers dont solve business problems; structured narrative and actionable strategy do. I undertook this Customer Shopping Behavior Analysis to bridge the gap between technical data engineering and executive decision-making. 

<br>

The primary objective wasn't just to aggregate historical metrics, but to solve a pressing enterprise challenge: **How can a retail organization leverage multi-channel shopping data to uncover purchasing trends, improve customer engagement, and optimize marketing and product strategies?**

<br>

To answer this comprehensively, I designed and executed a complete end-to-end analytics workflow. 
<br> 

- **Data Preparation and Engineering (Python):** Cleaning, imputing, and feature-engineering raw transactional data. 
- **Relational Database Analysis (SQL / PostgreSQL):** Modeling transactions in a relational database to run deep-dive queries on customer loyalty, discount dependencies, and revenue distribution.
- **Executive Visualization (Power BI):** Building an interactive dashboard to give non-technical stakeholders direct exploration capabilities. 
- **Strategic Roadmap:** Translating data patterns into clear business recommendations to maximize revenue and loyalty.
<br>

## Unearthing the Signal: Engineering the Data Pipeline

Every reliable insight starts with disciplined data hygiene. Analyzing 3,900 customer records across 18 transactional variables required cleaning before attempting any deep-dive querying.
<br> 

Using Python and Pandas, I focused on preparing the dataset for seamless relational modeling:
<br>

- **Imputation over Deletion:** Missing values in product review ratings were imputed using category-specific median ratings to preserve total record volume without biasing overall distributions. 
- **Schema Standardization:** Column headers were converted to standard snake_case, and redundant features (such as duplicate promo code indicators) were dropped to streamline downstream database performance. 
- **Feature Engineering:** I created demographic bins (age_group) and structured purchase frequency intervals to enable granular demographic querying. 
<br>

Once transformed, the clean dataset was ingested directly into PostgreSQL, creating a structured relational foundation for advanced analytical queries.

<br>

## What the Queries Revealed: The Story Behind the Numbers

Running targeted SQL queries across the dataset exposed several key behavioral insights that high-level averages usually obscure:

<br>

**1. The Subscription Bottleneck**

<br>

While 3,116 customers fell into the Loyal segment based on repeat purchase history, only 27% of total customers (1,053 buyers) were enrolled in the subscription program. Interestingly, average spend between subscribers ($59.49) and non-subscribers ($59.87) was nearly identical. The business was retaining repeat buyers, but completely failing to monetize or formalize that loyalty into predictable subscription revenue.

<br>

<img src="images/1791557993048.png" alt="Logo" width="600">

<br>

<img src="images/1791558060375.png" alt="Logo" width="600">

<br>

## 2. Discount Reliance vs. High-Value Spenders

Promotions drive sales volume, but do they erode profit margins unnecessarily? My SQL analysis revealed two critical nuances:

<br>

  - **839 customers** used discounts while still spending above the average store transaction value ($59.76). These high-value buyers did not require promotional pricing to make substantial purchases. 
  - Category-level discount dependence varied drastically: **Hats (50.00%), Sneakers (49.66%), and Coats (49.07%)** had roughly half of their total order volume tied directly to promotional discounts.

<br>

<img src="images/1791558210459.png" alt="Logo" width="600">

<br>

## 3. Demographic & Category Distribution

Total revenue reached **$233,081** across the portfolio, led by male shoppers ($157,890) compared to female shoppers ($75,191). Across age demographics, **Young Adults ($62,143) and Middle-aged ($59,197)** buyers generated the highest total revenue contributions. However, spending per purchase remained remarkably consistent across all age groups and shipping tiers—indicating that order size is driven by product selection rather than age or shipping urgency 

<br>

<img src="images/1791558302534.png" alt="Logo" width="600">

<br>

<img src="images/1791558323264.png" alt="Logo" width="600">

<br>

## Visualizing Impact: The Power BI Executive Dashboard

To turn query results into an intuitive visual story, I built an interactive Power BI Dashboard designed for rapid decision-making by executive leadership. 

<br>

The visual layout prioritizes key operational metrics:

<br>

  - **Core Business KPIs:** Top-line cards immediately highlight total customer count (3.9K), average basket size ($59.76), and customer satisfaction (3.75 average review rating). 
  - **Dynamic Slicers:** Stakeholders can slice transaction volumes and revenue by Subscription Status, Gender, Shipping Method, and Product Category (Accessories, Clothing, Footwear, Outerwear). 
  - **Demographic Breakdown:** Visual bars clearly illustrate sales volume and total spend across age cohorts, helping merchandising teams identify top-performing product lines like Blouses, Jewelry, and Jackets at a glance.

<br>

[![Watch the Demo](images/Power_BI_Picture.png)](https://youtu.be/YdjJWSYvqYo) 

<br>

## Strategic Roadmap: Turning Insights into Action

<br>

Data analysis creates real business value only when it shapes strategic execution. Based on the patterns identified throughout this project, I framed five actionable initiatives for executive leadership:

<br>

 - **Overhaul the Subscription Value Proposition:** Because non-subscribers generate 73% of revenue and spend the same per transaction as subscribers, current subscription benefits lack differentiation. Introducing perks such as free express shipping upgrades or early access to seasonal product drops will convert high-frequency buyers into formal subscribers. 

  - **Refine Discount Rules to Protect Margins:** Shift away from blanket, unconstrained discount codes. Implementing minimum spend thresholds (e.g., $15 off orders over $80) will prevent margin leakage on the 839 high-spending shoppers who are currently claiming discounts unnecessarily. 

  - **Targeted Merchandising and Positioning:** Maintain promotional strategies for discount-sensitive inventory like Coats and Sneakers to clear seasonal stock, while featuring top-rated staples like Gloves (3.86 rating) and Sandals (3.84 rating) in organic acquisition campaigns. 

<br>

Building this project from end to end reinforced why I love data analytics: it’s the process of converting raw, disconnected operational metrics into a clear human narrative and a concrete strategic playbook. By combining Python for data engineering, SQL for transactional analysis, and Power BI for executive storytelling, we can transform raw logs into meaningful business growth. 
