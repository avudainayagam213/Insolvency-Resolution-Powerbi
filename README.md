# Insolvency Resolution Analysis – Power BI

## 📊 Project Overview

This project is a Power BI analysis of an insolvency resolution portfolio. The report focuses on understanding insolvency cases, resolution outcomes, outstanding balances, and payment recovery performance.

The project uses a synthetic dataset designed to simulate a real-world insolvency/debt-resolution environment.

## 🎯 Business Objectives

The analysis aims to answer key business questions:

- How many insolvency cases are currently being managed?
- What are the most common insolvency types?
- What is the resolution rate across insolvency types?
- How much outstanding balance is associated with each insolvency type?
- How long does it take to resolve cases?
- How much has been recovered through payments?
- Which payment methods contribute most to recovery?
- How are insolvency cases and payments trending over time?

## 🛠️ Tools & Technologies

- Power BI Desktop
- Power Query
- DAX
- Microsoft Excel

## 🔄 Data Preparation

Power Query was used to transform and clean the raw data, including:

- Removing duplicate records
- Handling missing values
- Standardizing inconsistent text values
- Cleaning insolvency type and case status values
- Correcting data types
- Removing invalid/null payment records
- Preparing tables for data modelling

## 🧩 Data Model

The report uses a star-style relational model consisting of:

- Customers
- Accounts
- Insolvency Cases
- Payments
- Status History
- Date

Key relationships were created between customers, accounts, insolvency cases, payments, status history, and the date dimension.

## 📐 DAX

DAX measures were created to calculate:

- Total Cases
- Active Cases
- Completed Cases
- Failed Cases
- Outstanding Balance
- Resolution Amount
- Total Payments
- Payment Count
- Resolution Rate
- Recovery Rate
- Average Resolution Days
- Average Payment
- Failed Case Rate
- Average Outstanding Balance
- Month-over-Month Case Growth
- Running Total Cases
- Case Ranking
- YTD Case Analysis

Inactive date relationships were also handled using `USERELATIONSHIP()` for referral-date analysis.

## 📈 Report Pages

### 1. Executive Overview

Provides a high-level view of:

- Total Cases
- Active Cases
- Outstanding Balance
- Recovery Rate
- Cases by Insolvency Type
- Annual Insolvency Cases

### 2. Insolvency & Resolution Analysis

Focuses on:

- Case Status Distribution
- Resolution Rate by Insolvency Type
- Average Resolution Days
- Outstanding Balance by Insolvency Type
- Case Status by Insolvency Type
- Annual Case Trends

### 3. Payments & Recovery

Analyzes:

- Total Payments
- Payment Count
- Payments by Payment Method
- Annual Payment Trends
- Recovery Amount by Insolvency Type
- Average Payment by Payment Method

## 💡 Key Insights

The dashboard enables analysis of:

- Differences in resolution performance across insolvency types
- Case volumes and status distribution
- Outstanding balance exposure
- Recovery performance
- Payment behaviour and payment methods
- Trends in insolvency referrals and payments

## 📁 Repository Contents

- `Insolvency.pbix` – Power BI report containing the data model, Power Query transformations, DAX measures and dashboards.
- Synthetic raw dataset – Used as the source data for the analysis but not included in this repository because of GitHub's file-size limitation.

## ⚠️ Disclaimer

This project uses synthetic data created for learning and portfolio purposes. It does not contain real customer information, financial information, or confidential company data.
