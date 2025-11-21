# Bike Purchase Insights Dashboard 🚴📊

This project explores customer bike purchase behaviour using Excel, PivotTables, and interactive dashboards.

---

## 📂 Dataset Overview

I worked with a customer dataset containing **13 columns** and **1,027 rows** (including headers).  
Key fields include:

- Marital Status  
- Gender  
- Income  
- Number of Children  
- Education  
- Occupation  
- Home Ownership  
- Number of Cars  
- Commute Distance  
- Region  
- Age  
- Purchased Bike (Yes/No)

---

## 1️⃣ Data Cleaning & Standardisation

### 🔁 Removed Duplicates
To ensure accurate analysis, I removed duplicate records so that each row represents a **unique customer**.
<img width="1867" height="693" alt="Screenshot 2025-11-21 212925" src="https://github.com/user-attachments/assets/3b1b6f19-402f-4471-837d-f1e950acb5e5" />


### 🏷️ Made Categories More Readable
- Replaced marital status codes **"M" / "S"** with full labels **"Married" / "Single"**.
- Cleaned the **Gender** column to use consistent labels (e.g. **"Male"**, **"Female"**) so slicers and charts are easier to understand.
<img width="1225" height="658" alt="Screenshot 2025-11-21 213200" src="https://github.com/user-attachments/assets/63220918-6775-4224-ad50-3833f0a0e07a" />
<img width="1161" height="632" alt="Screenshot 2025-11-21 213245" src="https://github.com/user-attachments/assets/940aa86e-2b28-4073-b53a-fc3bd48acd18" />
<img width="1620" height="636" alt="Screenshot 2025-11-21 213351" src="https://github.com/user-attachments/assets/d387350b-8371-4883-bbed-361d2b9e4c1e" />

### 💰 Formatted Income for Consistency
- Updated the **Income** column to show **three decimal places**, improving consistency and making summary statistics look more professional in tables and charts.
<img width="119" height="619" alt="Screenshot 2025-11-21 213542" src="https://github.com/user-attachments/assets/57378122-df8f-4664-9dcf-3576e79997f4" />
---

## 2️⃣ Feature Engineering: Age Brackets

There were many distinct age values, which made charts cluttered and harder to interpret.  
To simplify, I created an **Age Bracket** field using `IF` functions:

- **Adolescent**: age `< 31`  
- **Middle Age**: age `≥ 31` and `≤ 54`  
- **Old**: age `> 54`
<img width="1862" height="669" alt="Screenshot 2025-11-21 214733" src="https://github.com/user-attachments/assets/ea480739-2727-45a2-b919-b80f2ad0a591" />

This transformation turned raw ages into three clear segments that are easier to compare visually in PivotTables and dashboards.

---

## 3️⃣ Pivot Tables & Charts

Using the cleaned sheet, I created several **PivotTables** and linked **PivotCharts** to explore patterns in bike purchases.

### 📊 Table & Chart 1 – Income vs Bike Purchase by Gender

**Pivot:** Average Income by **Gender** and **Purchased Bike (Yes/No)**

- **Females**
  - No bike: **53,440**
  - Bike purchased: **55,754**

- **Males**
  - No bike: **56,208**
  - Bike purchased: **60,124**
<img width="1473" height="531" alt="Screenshot 2025-11-22 093159" src="https://github.com/user-attachments/assets/4b111e8a-f674-4129-a2da-5a79f70bb787" />

> 🔍 **Key Pattern:** For both males and females, customers who **purchased a bike** have **higher average income** than those who did not.

---

### 🚴‍♂️ Table & Chart 2 – Commute Distance vs Bike Ownership

**Pivot:** Commute Distance vs **Purchased Bike**

- Customers are more likely to own/purchase bikes when their commute is **shorter (0–1 miles and 2–5 miles)**.
- For **5–10 miles** and **10+ miles**, customers tend to choose **other transportation modes** rather than bikes.
<img width="1484" height="470" alt="Screenshot 2025-11-22 093227" src="https://github.com/user-attachments/assets/90c6a507-9f78-4ff2-97da-0550ed2ac743" />

> 🔍 **Key Pattern:** Bikes are mainly used for **short-distance commuting**, not for medium or long-distance travel.

---

### 👥 Table & Chart 3 – Age Brackets vs Bike Purchase

**Pivot:** Age Bracket vs **Purchased Bike**

- **Middle Age** customers are the **most likely** to purchase bikes.
- **Adolescent** and **Old** brackets purchase bikes at **similar but lower levels**, which is interesting because we might initially expect younger customers to buy more bikes.
<img width="1476" height="520" alt="Screenshot 2025-11-22 093514" src="https://github.com/user-attachments/assets/29c49a9e-a8b3-45bb-a91c-aae41a3ef830" />

> 🔍 **Key Pattern:** The core bike-buying segment in this dataset is **middle-aged adults**, not necessarily the youngest group.

---

## 4️⃣ Final “Bike Sales Dashboard”

I consolidated everything into a **“Bike Sales Dashboard”** that includes the three main charts above.

To make the analysis interactive, I added **slicers** for:

- **Marital Status**
- **Region**
- **Education**
<img width="924" height="584" alt="Screenshot 2025-11-22 093744" src="https://github.com/user-attachments/assets/b3ec5b6b-40b8-43a0-a75e-68a4dd90db29" />

These slicers are connected to all three charts, allowing users to filter the view quickly and explore specific segments.

### 🎛 Example Slice: Single + Europe + Bachelor’s

When filtering for **Single**, **Europe**, and **Bachelor’s**:

- Only **Middle Age** and **Old** brackets appear.
- **Middle Age** customers dominate in terms of **ownership** (and often have more cars and higher incomes).
- For commute, bikes are used **most frequently in the 0–1 mile range**, and usage drops sharply beyond that, where customers **switch to other transport options**.
<img width="852" height="596" alt="Screenshot 2025-11-22 094407" src="https://github.com/user-attachments/assets/defcb950-6ad8-4568-a378-4de3ab418ce0" />

---

## 5️⃣ Insights & Recommendations 🚀

### 🔎 Key Insights

- **Income Effect**  
  Customers who purchase bikes tend to have **higher average incomes**, regardless of gender. Bikes may be positioned as a **lifestyle or commuting upgrade** rather than a purely budget option.

- **Commute Distance**  
  Bikes are strongly associated with **short commutes (0–5 miles)**. For longer distances, customers prefer **other modes of transport**.

- **Age Segment**  
  **Middle-aged customers** are the main bike-buying group, while **adolescents** and **older customers** buy at **similar, lower levels**. This challenges the assumption that bikes are dominated by younger customers.

- **Segment Slices (Single, Europe, Bachelor’s)**  
  Within this filtered segment, **middle-aged singles in Europe with a bachelor’s degree** show strong ownership patterns and a preference for bikes mainly over **short distances**.

---

### ✅ Recommendations

- **Target Middle-Aged, Higher-Income Professionals**
  - Design marketing campaigns and dashboards that highlight **commuting convenience, health benefits, and lifestyle**.
  - Use messaging that connects bikes with **time-saving short trips** and **urban mobility**.

- **Reposition for Younger Customers (Adolescents)**
  - Since adolescents are not leading bike purchases, consider **student discounts**, **installment plans**, or **bundles** (e.g. helmet + lock + maintenance) to reduce barriers.
  - Emphasise bikes as a **fun, social, and fitness-related** activity, not just a commute tool.

- **Leverage Commute Patterns**
  - Focus promotions on areas and segments with **short commute distances**, where bikes fit naturally into daily routines.
  - For customers with longer commutes, market bikes as a **first/last mile solution** (e.g. to/from public transport), rather than the entire journey.

- **Use the Dashboard for Ongoing Segmentation**
  - Encourage users to **explore slicers** (Region, Education, Marital Status) to uncover **high-potential micro-segments** (e.g. “Married, North America, Graduate degree”) for tailored campaigns.
  - Future iterations could include **conversion tracking** (before/after campaigns) and additional metrics like **frequency of use** or **preferred bike type** (if available).

---

