# 🇧🇷 Verra Carbon Audit: Brazil's Value Strategy

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Analytics-150458?style=for-the-badge&logo=pandas)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

> **Executive Summary:** While Asian markets dominate carbon credit *volume* (commodities), Brazil leads in *financial value* due to high-premium Nature-Based Solutions (NBS).

---

## 📊 The Core Insight
This project audits the Verra (VCS) registry data (2015-2025) to uncover a hidden market dynamic: **Volume $\neq$ Value.**

![Market Share Graph](market_share_insight.png)

### Key Findings
* **The Volume Illusion:** Global competitors (India/China) focus on renewable energy credits, trading at low margins (~$1.50/tCO2e).
* **The Brazilian Edge:** Brazil captures **~13.3% of the global financial market share**, despite lower physical volume. This is driven by Forestry/Land Use projects trading at premium prices (~$10.00+/tCO2e).
* **Top Developers:** Biofílica Ambipar and Carbonext emerged as the revenue leaders in the domestic landscape.

---

## 🛠️ Technical Strategy
This is not just a visualization; it is a full ETL pipeline.

| Stage | Tools/Methods |
| :--- | :--- |
| **Ingestion** | `Pandas` (CSV parsing, latin1 encoding handling) |
| **Cleaning** | `Unicodedata` for text sanitization (fixing "Mojibake" errors) |
| **Modeling** | Custom `Pricing Engine` based on Project Type (AFOLU vs. Energy) |
| **Viz** | `Seaborn` & `Matplotlib` (Dual Axis & Market Share Area Charts) |

## 📂 Project Structure
```bash
├── data/                  # Raw registry data (Ignored by git for compliance)
├── outputs/               # Generated high-res charts
├── vcs_analysis.ipynb     # Main Analysis Notebook (Source Code)
├── vcs_analysis.html      # Executive Report (No-code view)
└── README.md              # Documentation
