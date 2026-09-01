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

# Python: SAP Interface Log File & Error Parser

## 🧠 Project Overview
During large-scale ERP migrations, system integration steps, or bulk batch transfers (like IDoc processing), IT support teams face extensive, unformatted text log dumps. 

This technical Python automation tool consumes unstructured text-based log streams, parses transaction contexts via **Regular Expressions (Regex)**, and filters out system exceptions to generate an explicit, categorized Excel sheet for immediate incident management response.

## 🛠️ Key Technical Features Implemented
* **Text Parsing via Regex Parsing:** Deploys pattern group capturing (`(?P<name>...)`) to parse logs regardless of row density or text alignment.
* **Automated Categorization:** Evaluates transaction failure codes (e.g., locking conflicts vs. functional QM Master Data setup anomalies like missing active inspection types) and segments them automatically.
* **Business Spreadsheet Generation:** Utilizes `Pandas` and `openpyxl` structures to translate systemic raw error strings into categorized operational metrics.

## 🚀 Practical Application Context
This script acts as a microservice framework tool. It mimics logic that can easily be run as a daily Cron Job on an interface server or integrated into middleware processing layers to automatically alert SAP Application Managers when bulk material staging operations or message flows encounter structural blockages.

