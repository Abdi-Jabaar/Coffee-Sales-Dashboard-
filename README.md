# Barwaaqo Coffee Co. — Sales & Operations Analysis
Barwaaqo Coffee Co. is a Mogadishu-based coffee chain established in 2021, operating across five city branches Hodan, Wadajir, Medina, Yaqshid, and Karaan ,through a direct in-store retail model.

The company collects daily transactional data covering sales, product performance, branch operations, staff activity, and customer payment behavior. This project analyzes six months of that data to uncover the patterns, gaps, and opportunities that can improve how the business operates and grows.

### Key Areas of Analysis:
- Sales trends by hour, day, and month across all five branches
- Product performance ranked by revenue, volume, and profitability
- Branch-level comparison to identify top performers and growth opportunities
- Staff output analysis to understand what is actually driving individual performance

An interactive Power BI dashboard used to explore and report the findings can be found [here](https://app.powerbi.com/view?r=eyJrIjoiY2QxN2RkMzEtM2Y1MS00NWQ1LTlhZmYtNTE3YWY3Y2JlMWZlIiwidCI6IjI1Y2UwMjYxLWJiZDYtNDljZC1hMWUyLTU0MjYwODg2ZDE1OSJ9)

## Dataset Overview

| Detail | Value |
|---|---|
| Total Transactions | 396,619 |
| Time Period | January – June 2024 |
| Branches | 5 (Hodan, Wadajir, Medina, Yaqshid, Karaan) |
| Products | 15 across 3 categories |
| Total Revenue | $1.66M |
| Profit Margin | 74.4% (peak month) |
| Active Staff | 28 |
| Data Tables | 9 (transactions, products, staff, branches, shifts, customers, ingredients, and more) |

---

## Tools Used

| Tool | Purpose |
|---|---|
| Power BI | Dashboard development and data modeling |
| Power Query | Data transformation and cleaning |
| DAX | KPI calculations and margin analysis |
| Excel | Initial data exploration |

---

## Dashboard Pages

### Page 1 — Monthly Performance Overview
![Overview](screenshots/overview.png)

The first page shows the overall business performance for any selected month. At the top there are four KPI cards — Monthly Revenue, Total Cost, Net Profit, and Profit Margin — each compared against the previous month. Below that, there is a daily revenue trend line that shows how revenue moved day by day, and a branch bar chart showing how much each branch contributed. The bottom section has two charts: one showing which hours of the day generate the most revenue, and another showing which days of the week are the busiest.

### Page 2 — Product Performance
![Product](screenshots/product.png)

This page breaks down performance by product. The top cards highlight the best selling product (Latte), total units sold, the leading category (Hot Drink at 67.3%), and the highest margin product (Americano at 91.4%). There is a horizontal bar chart ranking the top 5 products by revenue, a donut chart splitting revenue across the three categories, and a full profitability table at the bottom that shows every product with its units sold, revenue, cost, profit, and margin.

### Page 3 — Staff Performance
![Staff](screenshots/staff.png)

The third page looks at how staff are performing individually. The top cards show the top performer (Saado Axmed with $90,650 at Yaqshid branch), the most orders handled, total active staff, and average revenue per staff member. The main section has a matrix showing how much revenue each staff member generates per shift hour. On the right is a leaderboard ranking all 28 staff by total revenue, and below is a full summary table with orders, units sold, revenue, and orders per shift for each person.

---

## Executive Summary

Barwaaqo Coffee Co. made **$1.66M in total revenue** over six months, with March being the strongest month at **$294,740** and a 74.4% profit margin. Most of the revenue happens during two periods — the 7–9 AM morning rush and the 12–1 PM lunch window. Latte is the top product in both. Hodan branch leads all five locations with 30% of total revenue. Overall the business is in a good position, but there are a few things that stand out: too much revenue is coming from one branch, a couple of products are underperforming with no plan to fix them, and the best staff member is working at the lowest volume branch.

---

## Insights Deep Dive

### 1. Peak Hours

![Peak Hours Chart](screenshots/peak_hours.png)

Looking at the full 6 months, the **7–9 AM window is the busiest part of the day** — each of those three hours generates around $193K, which is nearly double the next busiest period.

| Hour | 6-Month Revenue |
|---|---|
| 6 AM | $88,883 |
| **7 AM** | **$193,386** |
| **8 AM** | **$193,444** |
| **9 AM** | **$193,088** |
| 10 AM | $79,762 |
| 11 AM | $91,691 |
| **12 PM** | **$126,330** |
| **1 PM** | **$126,250** |
| 2 PM | $92,126 |
| 3–8 PM | ~$79K each |

What makes this interesting is that the morning peak is not a spike at one hour — all three hours (7, 8, and 9 AM) are almost exactly the same. So the pressure on staff and stock is sustained for three hours straight, not just one.

Revenue drops at 10 AM but partially comes back at 11 AM, then there is a clear second rush at **12–1 PM generating around $126K per hour**. This lunch peak is often treated as minor but it is actually 65% the size of the morning window — it deserves the same attention.

**Recommendations:**
- Make sure everything — staff, stock, ingredients — is ready before 6:45 AM, not during the rush
- Keep latte-skilled staff available throughout the full 7–9 AM window
- Stock Iced Latte and cold drink ingredients before the lunch window starts
- Try a mid-morning promotion around 10–11 AM to fill the drop between the two peaks

---

### 2. Peak Month — March

March was the highest month at **$294,740 — 9.5% above February**. Looking at just March, the hourly numbers also sharpen:

| Period | March Revenue |
|---|---|
| 7–9 AM | $102,893 |
| 9 AM alone | $34,641 |
| 12–1 PM | $45,219 |

The reason March was the best month is mostly Latte — it grew from $53K in February to $58K in March. A few other products each added $1K–$1.5K, and Americano held strong at 85% margin. Nothing else changed significantly.

One thing worth noting: **the product rankings stayed the same every single month across all six months**. The same products led in the same order with no changes. That tells you demand is stable and predictable — but it also means nothing new is growing. The business is still relying on the same two or three products.

**Recommendations:**
- Plan ahead for March — start promotions in February and cover all products, not just Latte
- Use the high-volume months to test operations and find where things slow down under pressure
- Start building up mid-tier products so the business is not dependent on Latte alone

---

### 3. Product Profitability

Hot Drinks bring in **67.3% of total revenue ($1.12M)**. Food accounts for $340K and Cold Drinks for $204K.

| Rank | Product | Category | Units Sold | Revenue | Total Cost | Profit | Margin |
|---|---|---|---|---|---|---|---|
| #1 | Latte | Hot Drink | 93,091 | $325,819 | $62,904 | $262,915 | 80.7% |
| #2 | Cappuccino | Hot Drink | 59,797 | $179,391 | $36,220 | $143,171 | 79.8% |
| #3 | Americano | Hot Drink | 62,973 | $157,433 | $23,031 | $134,402 | 85.4% |
| #4 | Chai Latte | Hot Drink | 37,929 | $123,269 | $22,368 | $100,902 | 81.9% |
| #5 | Croissant | Food | 54,932 | $109,864 | $49,423 | $60,441 | 55.0% |
| #6 | Hot Chocolate | Hot Drink | 36,206 | $108,618 | $27,506 | $81,112 | 74.7% |
| #7 | Banana Bread | Food | 39,748 | $99,370 | $29,800 | $69,570 | 70.0% |
| #8 | Iced Latte | Cold Drink | 24,267 | $97,068 | $18,096 | $78,972 | 81.4% |
| #9 | Mocha | Hot Drink | 22,357 | $83,839 | $23,603 | $60,236 | 71.8% |
| #10 | Macchiato | Hot Drink | 22,820 | $79,870 | $11,312 | $68,558 | 85.8% |
| #11 | Cheese Sandwich | Food | 25,184 | $75,552 | $23,918 | $51,634 | 68.3% |
| #12 | Espresso | Hot Drink | 29,692 | $59,384 | $10,859 | $48,525 | 81.7% |
| #13 | Cold Brew | Cold Drink | 14,222 | $56,888 | $30,858 | $26,030 | 45.8% |
| #14 | Fruit Cup | Food | 21,981 | $54,953 | $16,480 | $38,473 | 70.0% |
| #15 | Water Bottle | Cold Drink | 49,644 | $49,644 | $22,326 | $27,318 | 55.0% |

A few things stand out here:

**Macchiato has the highest margin of any product at 85.8%** but it is not in the top 5 by revenue. It is not a bad product — people just are not ordering it because staff are not promoting it.

**Croissant sells well (54,932 units)** but almost half of what it earns goes to cost at 55% margin. Pairing it with Latte or Americano as a morning combo would help increase its value without changing the price.

**Cold Brew has both the lowest volume and the lowest margin at 45.8%.** The issue here is awareness first — not many customers are ordering it. Raising the price before more people know about it would just make it worse.

**Water Bottle moves a lot of units (49,644)** but at $1 each with 55% margin, it is basically a convenience item and should be treated that way.

**Recommendations:**
- Test a +$0.50 price increase on Cold Brew and Water Bottle at one branch for 30 days — if orders drop more than 10%, go back to the original price
- Ask staff to mention Macchiato to customers — it is the highest margin product and most people do not even think to order it
- Create a morning combo with Croissant and Latte or Americano to increase the average order value
- Do not discount Latte or Cappuccino — they are already the top sellers, protect the margins

![Product Performance](screenshots/product.png)

---

### 4. Revenue by Branch

| Branch | 6-Month Revenue | Share |
|---|---|---|
| **Hodan** | **$500,591** | **30.1%** |
| Wadajir | $332,500 | 20.0% |
| Medina | $314,800 | 18.9% |
| Yaqshid | $261,400 | 15.7% |
| Karaan | $248,920 | 15.0% |

Hodan is the top branch by a significant gap — it brings in 30% of total revenue, nearly double what Yaqshid and Karaan each make. This makes sense given that Hodan is in the central business district where there is naturally more foot traffic during the week.

The concern is that the business is heavily dependent on one branch. If Hodan has a bad month for any reason — a problem with the location, a competitor nearby, or losing a key staff member — there is no other branch that can make up for it. The other four branches together make up 70%, but that is spread across four locations.

Yaqshid and Karaan are in residential areas and have lower traffic, but that also means customers there are more likely to be regulars if the branch builds a relationship with the local community.

**Recommendations:**
- Focus marketing efforts at Yaqshid and Karaan — loyalty programs, local promotions, and community-based campaigns to grow repeat customers
- Run a Latte promotion specifically at Yaqshid since it leads everywhere else but seems to underperform there
- Keep investing in Hodan — do not reduce resources there to balance things out, instead grow the other branches

![Branch Performance](screenshots/branch.png)

---

### 5. Staff Performance

| Staff | Branch | Skill | Revenue | Orders | Orders/Shift |
|---|---|---|---|---|---|
| **Saado Axmed** | Yaqshid | Medium | $90,650 | 22,930 | 126.0 |
| Deeqa Cali | Karaan | Medium | $86,052 | 21,588 | 118.6 |
| Hibo Cali | Hodan | High | $85,619 | 21,603 | 118.7 |
| Faadumo Ciise | Hodan | Medium | $85,535 | 21,693 | 119.2 |
| Amina Warsame | Hodan | High | $83,293 | 19,145 | 105.2 |

Saado Axmed is number one across every metric — revenue, total orders, and orders per shift — and she works at Yaqshid, which is the lowest volume branch in the whole chain. She is also rated Medium skill.

Looking at the full leaderboard, Medium-skill staff consistently outrank High-skill staff. At first this seems like a skill rating issue, but when you look at how shifts are structured it makes more sense: High-skill staff work the 7–9 AM morning rush with 3–4 colleagues around them. Staff like Saado work afternoon shifts mostly alone or with one other person, handling everything by themselves during a slower but still active period. The gap is about workload distribution, not actual skill level.

This also raises a question about the skill rating system itself. If Medium staff keep outperforming High staff even when you account for shift timing and branch volume, the rating may not be measuring what it is supposed to.

**Recommendations:**
- Move one or two staff from the morning peak to afternoon shifts where the workload is being handled by too few people
- Create a recognition system based on actual output — revenue, orders handled, and orders per shift — not skill rating
- Review how the skill levels are being assigned before using them to make any staffing or hiring decisions

![Staff Performance](screenshots/staff.png)

---

## Recommendations Summary

| Area | Action | Priority |
|---|---|---|
| Peak Hours | Pre-open restock, full staffing coverage 7–9 AM, test mid-morning offer 10–11 AM | High |
| Peak Month | Start March prep in February, develop mid-tier products | Medium |
| Product Portfolio | Price test Cold Brew +$0.50, bundle Croissant, promote Macchiato at point of sale | High |
| Branch Balance | Community marketing at Yaqshid and Karaan, Latte push at Yaqshid | Medium |
| Staff | Rebalance shifts, output-based recognition, review skill rating system | High |

---

## Project Info

This is a portfolio project that covers the full data analysis workflow — data cleaning, modeling, DAX calculations, dashboard design, and business reporting.

Tools: Power BI · DAX · Power Query · Excel
