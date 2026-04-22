# Research-Robots-txt-Governance
Clustering-based big data analysis of AI crawler blocking strategies using robots.txt (ICBDA 2026).
# Clustering-Based Big Data Analysis of Web Crawler Opt-Out Strategies: A Scientific Approach to Robots.txt Governance

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Conference](https://img.shields.io/badge/ICBDA-2026-orange.svg)
![Location](https://img.shields.io/badge/Presentation-Waseda_University-red.svg)

本專案為發表於 **ICBDA 2026 (第 11 屆大數據分析國際會議)** 之研究實作。研究運用科學的大數據分析方法，量化評估全球頂尖網站針對網路爬蟲（特別是生成式 AI 爬蟲）的治理現狀與防禦趨勢。

## 📖 研究摘要 (Abstract)
大型語言模型 (LLM) 極度依賴大規模網頁數據，然而網站主權意識抬頭。本研究以 2024 BEDC 全球前百大網站為樣本，獲取 98 份有效 `robots.txt` 檔案，透過 **K-means 聚類** 與 **主成分分析 (PCA)** 識別出三種主要的治理模式：
1. **全面拒絕型 (Full Opt-out)**
2. **AI 特定阻斷型 (Partial AI-targeted Opt-out)**
3. **限速存取型 (Rate-limited Access)**

研究發現 **61.2%** 的採樣網站已實施至少一項針對 AI 爬蟲的限制指令，顯示開放網頁數據空間正在實質收縮。

---

## 🛠️ 技術實作 (Methodology)

### 1. 數據採集與特徵工程
* **自動化採集**：實作非同步 Request 腳本，精準獲取全球 Top 100 網站之治理規則。
* **向量化處理**：將非結構化的 `robots.txt` 指令轉化為數值特徵，包含「指令強度」、「Agent 涵蓋率」及「路徑深度」。

### 2. 機器學習模型應用
* **K-means 聚類分析**：透過手肘法 (Elbow Method) 確定最佳群數 $K=3$，將不同產業的治理策略進行分類。
* **主成分分析 (PCA)**：將多維特徵縮減至「阻斷強度」與「模式差異化」兩個核心維度，解釋了 85% 以上的數據變異。

---

## 📊 關鍵研究發現 (Key Findings)
* **AI 治理成熟度**：研究證實「阻斷強度」是衡量網站 AI 治理成熟度的關鍵指標。
* **產業差異化**：媒體與新聞產業對 AI 爬蟲表現出最強的一致性防禦趨勢。
* **數據收縮驗證**：量化數據支持了網頁數據供應鏈正在縮減的理論假設。

---

## 🎓 發表紀錄與引用 (Publication & Citation)
本研究由 **鄭博仁 (Bo-Ren Cheng)** 於 2026 年 4 月在日本東京 **早稻田大學 (Waseda University)** 進行口頭發表。

```text
Cheng, B. R., & Cheng, C. Y. (2026). Clustering-Based Big Data Analysis of Web Crawler Opt-Out Strategies: A Scientific Approach to Robots.txt Governance. In Proceedings of the 11th International Conference on Big Data Analytics (ICBDA 2026).
