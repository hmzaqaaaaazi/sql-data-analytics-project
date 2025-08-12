# Data Warehouse Analytics Project

## 📊 Overview

This repository showcases a comprehensive **Business Intelligence and Analytics** implementation built on top of a modern data warehouse. The project demonstrates advanced SQL analytics, customer segmentation, product performance analysis, and business intelligence reporting using PostgreSQL.

## 🎯 Project Objectives

- **Customer Intelligence**: Deep dive into customer behavior, segmentation, and lifetime value analysis
- **Product Analytics**: Comprehensive product performance tracking and categorization
- **Business Insights**: Revenue analysis, trends identification, and strategic recommendations
- **Scalable Reporting**: Automated views and analytics ready for BI tool integration

## 🏗️ Architecture Overview

```mermaid
graph LR
   A[Bronze Layer<br/>Raw Data] --> B[Silver Layer<br/>Cleaned Data]
   B --> C[Gold Layer<br/>Business Ready]
   C --> D[Analytics Views]
   C --> E[Customer Reports]
   C --> F[Product Reports]
   D --> G[Business Intelligence<br/>Dashboards]

Data Flow

Bronze Layer: Raw data ingestion from CRM and ERP systems
Silver Layer: Cleaned, validated, and standardized data
Gold Layer: Business-ready fact and dimension tables
Analytics Layer: Advanced calculations and business logic

📈 Analytics Capabilities
1. Customer Analytics
Advanced customer intelligence with behavioral segmentation

Customer Segmentation: VIP, Regular, and New Customer classification
Lifetime Value Analysis: Total spending and relationship duration
Recency Analysis: Time since last purchase for retention strategies
Age Demographics: Customer age distribution and targeting
Purchase Behavior: Order frequency, average order value, and product diversity

Key Metrics:

Customer Lifetime Value (CLV)
Average Order Value (AOV)
Purchase Frequency
Customer Recency Score
Age-based Segmentation

2. Product Performance Analytics
Comprehensive product intelligence for inventory and marketing optimization

Product Segmentation: High, Mid, and Low performer classification
Revenue Analysis: Total sales, quantity sold, and profitability
Lifecycle Tracking: Product lifespan and market presence
Price Optimization: Average selling price vs. cost analysis
Customer Reach: Unique customers per product

Key Metrics:

Product Revenue Performance
Average Selling Price
Product Lifespan in Market
Customer Penetration Rate
Monthly Revenue Trends

3. Time-Series Analytics
Temporal analysis for trend identification and forecasting

Monthly Revenue Trends: Sales performance over time
Quarterly Analysis: Seasonal pattern identification
Year-over-Year Growth: Performance comparison across periods
Customer Acquisition Trends: New customer onboarding patterns

🗂️ Database Schema
Fact Tables

fact_sales: Core transactional data with foreign keys to dimensions

Dimension Tables

dim_customers: Customer master data with demographics
dim_products: Product catalog with categorization
dim_dates: Time dimension for temporal analysis

Analytics Views

report_customers: Customer intelligence dashboard
report_products: Product performance dashboard
