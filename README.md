# Hi, I'm Sunzid Ul Alam 
Welcome to my SAP development and data analytics portfolio! Below are featured projects showcasing my technical expertise across SAP ecosystems, custom development, and business intelligence.

## Featured Portfolio Projects

### SAP S/4HANA OO-ABAP Material Master Validator
A production-grade, object-oriented ABAP validation engine designed to enforce data integrity across SAP MM and QM modules before database updates.
* **Key Skills:** OO-ABAP, SAP MM/QM Integration, Encapsulation, Clean Code, Data Governance.
* **View Code:** [GitHub Repository](https://github.com/SunUlAlam/sap-abap-material-validator)

### Live Interactive Data Analytics Dashboard
A live web application built to analyze and visualize enterprise data trends dynamically.
* **Key Skills:** Python, Streamlit, Data Visualization, Cloud Deployment.
* **Launch App:** (https://sap-qm-kpi-dashboard-vhbpbrnsu6nwlqcbgpq32o.streamlit.app/)

# 🔍 Python: SAP Interface Log File & Error Parser

[![Python](https://shields.io)](https://python.org)
[![Pandas](https://shields.io)](https://pydata.org)
[![SAP Integration](https://shields.io)](https://sap.com)

## 🧠 Project Overview
During large-scale ERP migrations, system integration phases, or bulk batch transfers (like high-volume IDoc processing), IT infrastructure and SAP support teams face massive, unstructured text-based log file dumps. When critical operations crash, troubleshooting thousands of rows manually creates immediate incident response bottlenecks.

This technical Python automation tool consumes messy text log streams, applies **Regular Expressions (Regex)** via group-capturing to extract key transaction variables, and filters/categorizes system issues into a clean, operational Excel report for rapid application management response.

---

## 🛠️ Technical Implementation & Features
* **Regex Engine Parsing:** Deploys strict pattern group capturing (`(?P<name>...)`) to cleanly isolate `Timestamp`, `Log Level`, and `Message` contexts regardless of unaligned row data.
* **Automated Exception Categorization:** Evaluates systemic text patterns to auto-segment routine transactions from blocking errors (e.g., distinguishing **RFC Connectivity Timeouts**, user-driven **Data Enqueue/Lock Conflicts**, and functional **QM Master Data Setup Anomalies**).
* **Business Intelligence Spreadsheet Generation:** Integrates `Pandas` and `openpyxl` frameworks to transform raw error strings into structured, tabular Excel datasets (`.xlsx`) complete with automated category metrics.

---

## 🚀 Practical Application Context
This solution functions as a lightweight, production-ready microservice module. In an enterprise environment, this script is designed to run as an automated **Cron Job** on interface servers or hook directly into middleware processing layers. It eliminates manual log auditing by instantly alerting SAP Application Managers when bulk staging workflows or message flows encounter critical systemic blockages.

---

## 📁 Repository Structure
* 📄 **`parser.py`** — The core Python execution script and Regex engine.
* 📝 **`sap_job_log.txt`** — Sample unstructured raw text log file representing actual SAP background processing dumps.
* ⚙️ **`requirements.txt`** — Project environment dependency specifications (`pandas`, `openpyxl`).
* 📊 **`sap_critical_errors_report.xlsx`** — The final, production-ready structured report generated automatically by the parser.
