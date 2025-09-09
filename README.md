# 🎯 TZ Gaming: Optimal Targeting of Mobile Ads  

This project focuses on **targeted advertising optimization** for **TZ Gaming**, a mobile game developer. Using impression-level data from the **Vneta ad network**, the goal was to build predictive models to improve ad targeting, evaluate profitability across strategies, and compare in-house analytics vs. vendor-provided predictions.  

---

## 📌 Project Overview  
TZ Gaming spends heavily on mobile ads but has historically only broken even when accounting for direct click-through conversions. Executives believe there may be long-term brand benefits but want to ensure **short-term ROI** is maximized.  

The challenge: Should TZ rely on **random targeting, in-house logistic regression modeling, or Vneta’s proprietary predictions**?  

**Objectives:**  
1. Build and evaluate predictive models for ad click-through rates (CTR).  
2. Compare targeting strategies:  
   - Spam all prospects  
   - Current random targeting  
   - Logistic Regression predictions  
   - Vneta’s proprietary model  
3. Simulate campaign economics for a **20M impression purchase**.  
4. Recommend an optimal targeting strategy based on profit and ROI.  

---

## 🔍 Methodology  

### 1. Data Preparation  
- **Dataset:** 115,488 ad impressions with click/no-click outcomes.  
- **Features:** impression time, app ID, mobile OS, past impressions/clicks (per user, app, time, and ad).  
- **Splits:** Training (87,535) and Test (27,953).  

---

### 2. Modeling Approach  
- **Logistic Regression:** predicted probability of click-through.  
- **Model Checks:** Permutation importance, partial dependence plots, pseudo R², Chi-square test.  
- **Addressed Issues:** Multicollinearity (high correlation between features like imppat & clpat).  
- **Evaluation:** Decile analysis, Gains Curves, Confusion Matrices.  

---

### 3. Campaign Simulation  
- **Costs & Assumptions:**  
  - $10 CPM (cost per 1,000 impressions)  
  - 5% conversion rate from click to game signup  
  - $25 CLV per new player  
  - Data purchase: $50K  
  - Vendor consulting services: $150K  

- **Strategies compared:**  
  1. **Spam all** (baseline).  
  2. **Current random targeting**.  
  3. **In-house Logistic Regression**.  
  4. **Vneta’s predictions**.  

- Simulated **profits and ROME (Return on Marketing Expenditures)** for each option.  

---

## 🛠️ Tools & Libraries  
- **Python:** pandas, numpy, matplotlib, seaborn  
- **scikit-learn:** Logistic Regression, model evaluation  
- **Custom Code:** Decile analysis, gains curves, confusion matrices  
- **Simulation:** profit and ROI calculations for large-scale campaigns  
- **Jupyter Notebook:** reproducible workflow & reporting  

---

## 💡 Key Skills & Concepts  
- **Digital Marketing Analytics**  
- **Ad Targeting Optimization**  
- **Logistic Regression for CTR Prediction**  
- **Multicollinearity & Model Diagnostics**  
- **Gains Curves & Decile Analysis**  
- **Profit Simulation & ROI Analysis**  
- **Vendor vs In-House Model Evaluation**  

---

## 🚀 Key Takeaways  
- Logistic Regression provided **interpretable, cost-effective predictions** that outperformed random targeting.  
- Vneta’s proprietary model improved CTR prediction but came with **significant consulting fees**.  
- Simulation results showed **profit lift from predictive targeting**, making a strong case for **data-driven ad allocation**.  
- Data science enables **better ad spend efficiency**, especially at scale (20M+ impressions).  
