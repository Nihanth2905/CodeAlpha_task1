# CodeAlpha Financial Health Dashboard

## Project Overview

This project is a Financial Health Dashboard created using Microsoft Power BI as part of the CodeAlpha Power BI Internship.

The dashboard provides an interactive view of financial performance and helps analyze revenue, expenses, profitability, cash flow, financial position, budgeting, and future revenue estimates.

## Objectives

The main objectives of this project are:

- Analyze income and expenses
- Track profitability trends over time
- Analyze the company's financial position
- Monitor cash inflows and outflows
- Compare budgeted expenses with actual expenses
- Forecast future revenue
- Provide actionable financial insights through interactive visualizations

## Tools Used

- Microsoft Power BI Desktop
- Microsoft Excel
- DAX
- Power Query
- GitHub

## Dataset

The project uses a fictional financial dataset created in Excel.

The dataset contains the following tables:

- Transactions
- Balance Sheet
- Cash Flow
- Budget

### Transactions

Contains financial transactions with:

- Date
- Category
- Transaction Type
- Amount

Transaction types include Revenue and Expense.

### Balance Sheet

Contains:

- Account
- Type
- Amount
- Date

The balance sheet categorizes financial information into Assets, Liabilities, and Equity.

### Cash Flow

Contains:

- Date
- Category
- Cash Flow Type
- Amount

Cash flows are categorized as Inflow and Outflow.

### Budget

Contains:

- Date
- Category
- Budget Amount

This table is used to compare planned spending with actual expenses.

## Dashboard Features

### Key Performance Indicators

The dashboard includes:

- Total Revenue
- Total Expenses
- Net Profit
- Profit Margin

### Revenue and Expense Analysis

A monthly comparison of revenue and expenses is provided to identify changes in financial performance.

### Profitability Trend

The Net Profit trend shows how profitability changes from month to month.

### Cash Flow Analysis

The dashboard visualizes cash inflows and outflows by category.

### Balance Sheet Analysis

Assets, Liabilities, and Equity are displayed to provide an overview of the company's financial position.

### Budget vs Actual

Budgeted expenses are compared with actual expenses by category to identify areas requiring cost control.

### Revenue Forecast

Power BI forecasting is used to estimate future revenue based on historical transaction data.

## DAX Measures

The dashboard uses DAX measures including:

```DAX
Total Revenue =
CALCULATE(
    SUM(Transactions[Amount]),
    Transactions[TransactionType] = "Revenue"
)
