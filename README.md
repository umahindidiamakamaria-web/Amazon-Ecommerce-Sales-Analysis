#  Amazon E-Commerce Sales & Product Performance Analysis

##  Project Overview
This project presents an Amazon E-Commerce Sales and Product Performance Analysis using real Amazon product data. The analysis covers product ratings, pricing, discounts and customer engagement across multiple product categories to uncover powerful business insights and performance trends.

**Track:** Data Analysis — NTTS Stage 7 | MicroTech Africa Nigeria
**Prepared by:** Ndidiamaka Umahi
**Tools Used:** Microsoft Excel | Power Query | Pivot Charts | Dashboard Design

##  Files in This Repository
| File | Description |
| `Amazon_Sales.csv` | Raw dataset — 1,465 Amazon product records |
| `Amazon sales analysis dashboard.xlsx` | Cleaned data and interactive dashboard |
| `DASHBOARD.png` | Screenshot of the final dashboard |
| `BUSINESS_QUESTIONS.pdf` | All 5 business questions with data-driven answers |
| `EXECUTIVE_SUMMARY.pdf` | One-page executive summary for management |

##  Dataset Description
| Column | Description |
| `Product_id` | Unique product identifier |
| `Product_name` | Name of the product |
| `Category` | Full product category hierarchy |
| `Discounted_price` | Current selling price |
| `Actual_price` | Original price before discount |
| `Discount_percentage` | Percentage discount applied |
| `Rating` | Average customer rating (1-5) |
| `Rating_count` | Number of customer ratings |
| `User_name` | Name of reviewer |
| `Review_title` | Short review title |

## 🧹 Data Cleaning Steps (Power Query)
- Removed unnecessary columns — `about_product`, `img_link`, `product_link`, `review_content`, `review_id`, `user_id`
- Removed ₹ symbol and commas from price columns and converted to Whole Number
- Removed % symbol from discount column and converted to Decimal Number
- Handled 1 invalid rating row containing only a pipe symbol "|"
- Replaced null values in `rating` and `rating_count` with 0
- Added **Main_Category** column — extracted first category before "|" delimiter
- Added **Price_Range** column — Budget, Mid-Range, Premium, Luxury
- Added **Discount_Range** column — Low, Medium, High, Very High


##  Business Questions & Key Findings

### Q1 — Top Performing Products by Rating
| Rank | Product | Rating |
|------|---------|--------|
| 1 | Syncwire LTG to USB Cable | 5.00 |
| 2 | Amazon Basics Wireless Mouse | 5.00 |
| 3 | REDTECH USB-C to Lightning Cable | 5.00 |
| 4 | Instant Pot Air Fryer Vortex 2QT | 4.80 |
| 5 | Swiffer Instant Electric Water Heater | 4.80 |
> Top 3 products share a perfect 5.00 rating — all simple reliable accessories confirming that practical everyday products consistently achieve the highest customer satisfaction.

### Q2 — Price vs Rating Analysis
| Price Range | Avg Actual Price | Avg Discounted Price | Avg Rating |
|-------------|-----------------|---------------------|-----------|
| Budget (₹0-500) | ₹362.83 | ₹195.15 | 4.07 |
| Mid-Range (₹501-2,000) | ₹1,222.04 | ₹587.45 | 4.10 |
| Premium (₹2,001-10,000) | ₹4,727.81 | ₹2,374.40 | 4.07 |
| Luxury (₹10,000+) | ₹27,424.71 | ₹16,877.23 | 4.18 |
> Price does not significantly affect customer rating — all ranges score between 4.07 and 4.18 showing customers are equally satisfied regardless of spending level.

### Q3 — Category Performance
| Category | Avg Rating | Total Reviews |
|----------|-----------|--------------|
| Office Products | 4.31 | 149,675 |
| Toys & Games | 4.30 | 15,867 |
| Electronics | 4.08 | 15,778,848 |
| Computers & Accessories | 4.15 | 7,728,689 |
| Car & Motorbike | 3.80 | 1,118 |
> Office Products leads by rating (4.31) while Electronics dominates by volume (15.7M reviews). Car & Motorbike is the weakest category with lowest rating and fewest reviews.

### Q4 — Product Popularity by User Engagement
| Rank | Product | Total Reviews |
|------|---------|--------------|
| 1 | Amazon Basics High-Speed HDMI Cable | 853,946 |
| 2 | AmazonBasics Flexible Premium HDMI Cable | 853,945 |
| 3 | boAt Bassheads 100 In Ear Earphones | 727,426 |
| 4 | Redmi 9A Sport (Coral Green) | 627,668 |
| 5 | JBL C100SI Wired In Ear Headphones | 577,766 |
> Amazon Basics HDMI Cables dominate the top 2 positions confirming Amazon's own brand products are extremely popular.

### Q5 — KPIs & Additional Insights

**Key Performance Indicators:**
| KPI | Value |
|-----|-------|
| Total Products | 1,464 |
| Average Rating | 4.10 |
| Average Discount | 47.71% |
| Most Reviewed Category | Electronics |
| Average Price Saving | ₹2,321 |

**Additional Insight 1 — Discount Distribution:**
| Discount Range | Count | Percentage |
|----------------|-------|-----------|
| High (41-60%) | 514 | 35% |
| Very High (61%+) | 440 | 30% |
| Medium (21-40%) | 339 | 23% |
| Low (0-20%) | 171 | 12% |
> 65% of all products offer discounts above 40% confirming Amazon's aggressive discount pricing strategy.

**Additional Insight 2 — Price Range Distribution:**
| Price Range | Count | Percentage |
|-------------|-------|-----------|
| Mid-Range (₹501-2,000) | 523 | 35.7% |
| Premium (₹2,001-10,000) | 422 | 28.8% |
| Budget (₹0-500) | 312 | 21.3% |
| Luxury (₹10,000+) | 208 | 14.2% |
> Mid-Range products dominate the catalog at 35.7% showing Amazon caters primarily to value conscious customers.

---

##  Dashboard Features

- **5 KPI Cards** — Total Products, Average Rating, Average Discount, Most Reviewed Category, Average Price Saving
- **6 Interactive Charts:**
  - Top Products by Rating (Bar Chart)
  - Price vs Rating Analysis (Clustered Bar with Secondary Axis)
  - Category Performance by Rating (Bar Chart)
  - Top Products by User Engagement (Bar Chart)
  - Discount Distribution (Donut Chart)
  - Category by Total Review Count (Bar Chart)
- **3 Dynamic Slicers** — Main Category, Price Range, Discount Range
- **Colour Theme** — Amazon Orange `#FF9900` and Dark Navy `#232F3E`

##  Recommendations

1. **Invest in Office Products and Toys marketing** — highest ratings but low review counts suggest untapped potential
2. **Improve Car & Motorbike category** — lowest rating (3.80) and fewest reviews (1,118) need urgent attention through product quality improvement and targeted promotions

##  Key Takeaways

- Amazon maintains strong customer satisfaction with an average rating of **4.10**
- Price does **NOT** significantly impact customer satisfaction
- **65%** of products offer discounts above 40% — value for money is Amazon's core strength
- Electronics dominates engagement with **15.7 million** reviews
- Customers save an average of **₹2,321** per product

