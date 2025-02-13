Finanace Performance Dashboard 
Here's a detailed **GitHub description** for your **Finance Performance Dashboard** project:  

---

## **Finance Performance Dashboard** 📊  
**Created using Power BI**  

### **Overview**  
This **Finance Performance Dashboard** provides a comprehensive analysis of financial performance across multiple products and regions. The dashboard is divideds into **two sections**:  
✅ **Overall Performance Analysis** (First 2 slides)  
✅ **Product-wise Analysis** (Laptops, Accessories, Tablets & Smartphones)  

---

### **Key Features & Insights**  
🔹 **Overall Financial Performance**  
- Evaluates revenue, sales, and trends across multiple regions.  
- Identifies key drivers of financial growth.  

🔹 **Product-Wise Breakdown**  
- **Laptops** 💻: Sales and revenue performance across different countries.  
- **Accessories** 🎧: Market contribution and demand trends.  
- **Tablets** 📱: Revenue trends across years and customer segmentation.  
- **Smartphones** 📲: Performance analysis by country and customer demographics.  

🔹 **Regional & Demographic Analysis**  
- Revenue distribution by country (England, Japan, Singapore, etc.).  
- Sales segmentation by **gender & customer profile**.  

🔹 **Visualizations & Metrics**  
- **Revenue Trend Analysis** 📈  
- **Market Share Distribution** 🌍  
- **Top-Selling Products & Locations** 🏆  

---
### **Dax Queries ** [Performed here].
**Page-1**
- Revenue_Amount = SUM(Sheet1[Revenue (USD)]).
- Average_Revenue = AVERAGE(Sheet1[Revenue (USD)]).
- Total_transactions = COUNT(Sheet1[First Name]).
- Total_country's = DISTINCTCOUNT(Sheet1[Country]).
- Total_Regions = DISTINCTCOUNT(Sheet1[Region]).
- Country% = DIVIDE([Revenue_Amount],[Country_wise_Revenue],0)
- Product_Revenue% = DIVIDE([Revenue_Amount],[Total_Revenue_Product],0)
  
**Laptop**
- Laptop_Revenue = CALCULATE(SUM(Sheet1[Revenue (USD)]),Sheet1[Products]="Laptops")
- Laptop_Avg_Revenue = CALCULATE(AVERAGE(Sheet1[Revenue (USD)]),Sheet1[Products]="Laptops")
- Laptop_Reveneu_% = DIVIDE([Laptop_Revenue],[Revenue_Amount],0)
  
**Assessories**
- Accessories_Revenu = CALCULATE(SUM(Sheet1[Revenue (USD)]),Sheet1[Products]="Assessories")
- Accessories% = DIVIDE(Accessories[Accessories_Revenu],[Revenue_Amount],0)
- Avg_Accessories_Revenue = CALCULATE(AVERAGE(Sheet1[Revenue (USD)]),Sheet1[Products]="Assessories")
  
**Smartphones**
- SmartPhones_Revenue = CALCULATE(SUM(Sheet1[Revenue (USD)]),Sheet1[Products]="Smartphones")
- Smartphones_Avg = CALCULATE(AVERAGE(Sheet1[Revenue (USD)]),Sheet1[Products]="Smartphones")
- Smartphones_% = DIVIDE(SmartPhones[SmartPhones_Revenue],[Revenue_Amount],0)
  
**Tablets**
- Tablets_Revenue = CALCULATE(SUM(Sheet1[Revenue (USD)]),Sheet1[Products]="Tablets")
- Tablets_Avg_Revenue = CALCULATE(AVERAGE(Sheet1[Revenue (USD)]),Sheet1[Products]="Tablets")
- Tablets% = DIVIDE([Tablets_Revenue],[Revenue_Amount],0)

  
### **Product-Wise Insights & Conclusion**  

✔ **Laptops** 💻  
- Strongest revenue-generating product.  
- High demand in **Japan & New York**.  
- Increasing sales trends over time.  

✔ **Accessories** 🎧  
- Consistent sales, but lower revenue share.  
- Popular in **England & Hong Kong**.  
- Requires marketing efforts to boost sales.  

✔ **Tablets** 📱  
- Moderate performance with fluctuating demand.  
- High sales in **England & Taiwan**.  
- Price sensitivity affecting sales.  

✔ **Smartphones** 📲  
- **Highest selling category** in terms of volume.  
- Strong demand in **England, Las Vegas & Singapore**.  
- Competitive pricing leads to revenue variations.  

---
