# Evaluation of Cache Usage on Ecommerce Catalogs of Multitenant Platforms

Final undergraduate thesis by **Thúlio Ícaro Castro Carvalho**, presented at the Federal University of Campina Grande (UFCG) in 2023.

## 📍 Summary

This work explores how caching systems behave in large-scale **multitenant ecommerce platforms**. By analyzing production traffic data from a real-world catalog application, the study uncovers patterns in workload characteristics and evaluates how those patterns affect cache performance — particularly **cache hit rate** and its relationship to **tenant distribution**.

---

## 📊 Key Findings

- **Hit Ratio (from backend perspective):** 55%
- **Stale Responses:** 30%
- **Standard Deviation of Hit Rate:** ~7%
- **Request concentration:** Top 10% of tenants generated 76% of traffic
- **No strong correlation** between tenant popularity and hit rate (r ≈ 0.09)

---

## 🖼️ Visual Insights

### 📈 Hit Ratio Over Time
![Hit Ratio](./media/image2.png)

### 🏪 Tenant Request Distribution
![Tenant Distribution](./media/image5.png)

### 🔄 Popularity vs Hit Ratio Correlation
![Correlation Plot](./media/image4.png)

---

## 🔬 Methodology

- Analyzed traces from real production traffic to a **search API cache layer** in a large ecommerce platform.
- Used NGINX instrumentation and log sampling to measure cache behavior.
- Investigated **multitenancy challenges**, including traffic skew and potential for tenant-aware optimization.

---

## ⚠️ Limitations

- Work was based on sampled request data due to storage constraints.
- Only a single time frame was analyzed (approx. 45 minutes of traffic).

---

## 📄 Full Paper

For full methodology, data analysis, and discussion, [read the full paper here](./TCC.md) or explore the raw markdown version in this repo.

---

## 📬 Contact

Feel free to reach out if you're working on caching, infra, or distributed systems — always happy to chat.

> 📧 thulioicc@gmail.com
