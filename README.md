# Barwaaqo Coffee Co. — Sales & Operations Analysis

> A full-scope analysis of 396,619 transactions across 5 Mogadishu branches, 6 months, and 15 products — built to surface the decisions the business should be making but currently isn't.

![Dashboard Overview](screenshots/overview.png)

🔗 [View Interactive Power BI Dashboard](#) &nbsp;|&nbsp; 📁 [Dataset](#) &nbsp;|&nbsp; 👤 [Author](#author)

---

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
| Power BI | Dashboard development, DAX measures, data modeling |
| Power Query | Data transformation and cleaning |
| DAX | KPI calculations, time intelligence, margin analysis |
| Excel | Initial data exploration and validation |

---

## Dashboard Pages

| Page | What It Covers |
|---|---|
| Overview | Monthly revenue, total cost, net profit, daily trend, branch performance, peak hours, busiest days |
| Product Performance | Top 5 by revenue, category split, full profitability table with margin per product |
| Staff Performance | Staff leaderboard, revenue by shift hour, orders per shift, skill-level comparison |

---

## Executive Summary

Barwaaqo Coffee Co. generated **$1.66M in total revenue** across six months, peaking at **$294,740 in March** with a 74.4% profit margin. Revenue runs on two daily surges — a sustained 7–9 AM plateau and a strong 12–1 PM second peak — with Latte anchoring both windows as the top product by volume and profit. Hodan leads all five branches at 30% of total revenue, a performance tied directly to its central business district location. The business is operationally stable and commercially predictable — but that stability is obscuring three structural problems: dangerous revenue concentration in one branch, two underperforming products with no corrective strategy, and the top-performing staff member deployed in the lowest-volume location.

---

## Insights Deep Dive

### 1. Peak Hours — 6-Month View

![Peak Hours Chart](screenshots/peak_hours.png)

Across the full six months, the **7–9 AM window generates ~$193K per hour** — the highest and most consistent revenue band of the entire operating day:

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

This is not a spike with a single peak hour — it is a **flat plateau across three consecutive hours**, meaning the bottleneck risk is sustained, not momentary. A preparation failure at 6:50 AM does not cost one rush — it costs three.

The **12–1 PM window is a genuine second peak at ~$126K per hour** — 65% the size of the morning plateau. It demands the same operational discipline, not an afterthought.

The **10 AM dip to $79K** partially recovers at 11 AM, meaning demand still exists in that window — a targeted mid-morning offer has a real customer base to work with.

**Recommendations:**
- Complete all restocking and staff deployment before 6:45 AM — not during the rush
- Keep latte-skilled staff on the floor continuously from 7–9 AM, not rotated out mid-peak
- Pre-position Iced Latte and cold drink ingredients specifically for the 12–1 PM window
- Test a mid-morning offer (10–11 AM) to lift the dip and extend the morning revenue curve

---

### 2. Peak Month — March

March is the highest-revenue month at **$294,740 — 9.5% above February**. Within March, the hourly pattern sharpens significantly:

| Period | March Revenue |
|---|---|
| 7–9 AM (morning plateau) | $102,893 |
| Single-hour peak (9 AM) | $34,641 |
| 12–1 PM (lunch peak) | $45,219 |

The March spike was not broad-based. **Latte alone drove it**, growing from $53K in February to $58K. Four other products contributed $1K–$1.5K increases each, with Americano providing structural support at 85% margin. Everything else held steady.

More significant: **product rankings never shifted across all six months.** The same products led every month in the same order with no movement. Demand is stable — but also means the business has not developed a single new revenue source in six months. The top two products are carrying everything.

**Recommendations:**
- Treat March as a planned commercial event — begin promotional preparation in February across the full product range, not just Latte
- Use March's elevated volume to stress-test operations and expose bottlenecks before peak demand hits
- Invest in growing mid-tier products to reduce single-product revenue dependency

---

### 3. Product Profitability

Hot Drinks account for **67.3% of total revenue ($1.12M)**. Food follows at $340K (20.45%) and Cold Drinks at $204K (12.26%).

**Full product breakdown:**

| Rank | Product | Category | Units Sold | Revenue | Margin | Profit |
|---|---|---|---|---|---|---|
| #1 | Latte | Hot Drink | 93,091 | $325,819 | 80.7% | $262,915 |
| #2 | Cappuccino | Hot Drink | 59,797 | $179,391 | 79.8% | $143,171 |
| #3 | Americano | Hot Drink | 62,973 | $157,433 | 85.4% | $134,402 |
| #4 | Chai Latte | Hot Drink | — | $123,269 | 81.9% | — |
| #5 | Croissant | Food | 54,932 | $109,864 | 55.0% | — |
| — | Macchiato | Hot Drink | — | — | 85.8% | — |
| — | Water Bottle | Food | 49,644 | $49,644 | 55.0% | — |
| — | Cold Brew | Cold Drink | 14,222 | $56,888 | 45.8% | — |

**What the numbers reveal:**

**Macchiato** has the highest margin in the entire portfolio at 85.8% but does not appear in the top 5 by revenue. Customers are not ordering it — which is a sales floor problem, not a product problem.

**Croissant** moves high volume but 45 cents of every dollar goes to cost. Bundling it with Latte or Americano as a morning combo improves its revenue-per-transaction contribution without touching the price.

**Cold Brew** is the weakest product: lowest margin and lowest volume. Marketing before repricing — a price increase on an already low-volume product accelerates decline, not recovery.

**Water Bottle** at $1 per unit with 55% margin is a convenience item. Treat it as one.

**Recommendations:**
- Run a 30-day price test on Cold Brew and Water Bottle (+$0.50) at one mid-volume branch — reverse if units drop more than 10%
- Train staff to mention Macchiato at point of sale — highest margin product, currently invisible
- Bundle Croissant with Latte or Americano as a named morning combo
- Do not discount Latte or Cappuccino — protect margins through upselling and loyalty only

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

Hodan generates 30% of total revenue — nearly double Yaqshid and Karaan individually. Its central business district location drives organic foot traffic no other branch can match without active intervention.

The risk is structural. At 30% dependency, a single bad month at Hodan — operational disruption, a competitor opening nearby, a key staff departure — pulls the entire business down in a way no combination of the remaining four branches can offset. The business does not have a revenue spread. It has a revenue anchor.

Yaqshid and Karaan together represent **30.7% of revenue across two residential-area branches**. Lower walk-in traffic is a location constraint, not a brand constraint — which means loyal repeat customers are more achievable there than at a transient business district location. That lever is currently unpulled.

**Recommendations:**
- Invest in community-focused marketing at Yaqshid and Karaan — loyalty programs, neighbourhood promotions, local partnerships
- Launch a Latte-specific branch promotion at Yaqshid — it leads revenue everywhere else and any underperformance there compounds the branch's already weaker position
- Do not reallocate Hodan's resources to compensate. Grow the others up, not Hodan down

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

Saado Axmed leads every metric — revenue, orders, and orders per shift — while working at Yaqshid, **the lowest-volume branch in the chain**, classified as Medium skill.

The pattern holds across the full leaderboard: **Medium-skill staff consistently outperform High-skill staff**. The explanation is not individual ability — it is shift structure. High-skill staff work the 7–9 AM morning peak alongside three to four colleagues. Top performers like Saado work afternoon slots with one to two colleagues, absorbing the full operational load of a lower-traffic period alone. **The performance gap is a workload gap, not a skill gap.**

The secondary problem: if Medium consistently outranks High across volume, timing, and branch controls, the skill classification system is not measuring what it claims to. Any hiring or promotion decision built on that rating is operating on flawed data.

**Recommendations:**
- Rebalance shifts — move one to two staff from the over-staffed morning peak to afternoon slots
- Build an Employee of the Month framework on measurable output: revenue, orders handled, orders per shift — not skill rating
- Audit the skill classification methodology before using it for any further staffing decisions

![Staff Performance](screenshots/staff.png)

---

## Recommendations Summary

| Area | Action | Priority |
|---|---|---|
| Peak Hours | Pre-open restock, sustained latte-skilled coverage 7–9 AM, test 10–11 AM bridge offer | High |
| Peak Month | Start March prep in February; reduce top-2 product dependency | Medium |
| Product Portfolio | Price test Cold Brew +$0.50, bundle Croissant, push Macchiato at POS | High |
| Branch Balance | Community marketing at Yaqshid and Karaan; Latte push at Yaqshid specifically | Medium |
| Staff Deployment | Rebalance morning vs afternoon shifts; output-based recognition; audit skill ratings | High |

---

## Project Info

This is a portfolio project built to demonstrate end-to-end data analysis — from raw transactional data to a structured business report with actionable recommendations.

Tools: Power BI · DAX · Power Query · Excel
