# Finvera Financial Services Analytics
## Capstone Project Requirements

**Project:** Cross-Functional Financial Services Analytics at Finvera Financial Services Group

**Industry:** Financial services, covering insurance, wealth management and lending.

---

## 1. Project Overview

Finvera Financial Services Group operates across insurance, wealth management and lending. Its Sales, Marketing, Operations and Finance teams maintain separate data and work with limited visibility across functions.

The project asks the learner, acting as a Business Analyst, to connect these business views, assess the reliability of the available data, identify performance and risk patterns, and present evidence-based recommendations to leadership.

## 2. Business Problem

- **Sales:** Lacks a reliable view of agent productivity and the products and channels generating policy sales.
- **Marketing:** Cannot consistently connect campaign activity with lead quality or growth in Assets Under Management (AUM).
- **Operations:** Needs to understand claim turnaround time and the proportion of claims processed manually.
- **Finance:** Needs visibility into loan approval time, delinquency and the customer segments or credit-score bands associated with risk.
- **Customer Insights:** Customer information is not consistently connected across products, making cross-sell activity difficult to identify.

The required analytical approach is to improve data quality first, connect relevant datasets second, and use the resulting evidence to recommend business action.

## 3. Project Objectives

- Translate a broad, cross-functional business situation into clear analytical questions and measurable KPIs.
- Clean inconsistent financial-services data and prepare it for analysis.
- Join data across products and departments to answer questions that cannot be addressed using one dataset alone.
- Use statistical methods to assess assumptions relating to claims processing and credit risk.
- Develop an integrated dashboard connecting Sales, Marketing, Operations and Finance, supported by actionable recommendations.

## 4. Data Provided

The project provides ten CSV datasets:

1. Customers
2. Agents
3. Branches
4. Products
5. Policies
6. Leads
7. Marketing Campaigns
8. Investments
9. Claims
10. Loans

The datasets are connected through shared identifiers, including customer, agent, branch, product, campaign and policy IDs.

The data is intentionally imperfect. Expected issues include:

- Missing values.
- Duplicate records.
- Inconsistent text and category values.
- Mixed date formats.
- Numeric amounts stored as text.
- Out-of-range values such as negative claim-processing days or placeholder values of 9999.

## 5. Scope and Required Tasks

### Task 1 – Prompt-Driven Problem Discovery

Use a GenAI tool through prompts to:

- Convert the business story into a leadership briefing.
- Identify candidate KPIs for the four departments.
- Propose three to five business hypotheses for further testing.
- Retain the prompts and refined outputs.

**Required Deliverables:**
- One-page briefing note.
- Draft departmental KPI list.
- Business hypotheses.
- Prompts used.

### Task 2 – KPI and Metric Definition

Select two to three priority KPIs for each department.

Define each KPI precisely, including:

- KPI formula.
- Required source tables and columns.
- Level of analysis.
- Responsible department.
- Relevant data-quality risks.

**Required Deliverable:**

KPI definition document or framework covering the metric, formula, source fields, owner and data risks.

### Task 3 – Data Cleaning and Sales Performance Analysis

Use the customer, policy, agent and product data.

Activities include:

- Remove duplicate records.
- Standardise gender, segment, status and city values.
- Correct date formats.
- Convert text-based premiums to numbers.
- Document rules for missing age, income-band and monthly-target values.
- Analyse policy sales by product and channel.
- Analyse premiums by product.
- Evaluate agent performance against targets.
- Identify cross-sell customers across policies, investments and loans.

**Required Deliverables:**

- Cleaned Excel workbook.
- Data-cleaning log.
- Pivot-table analysis.
- Three to four findings written in plain language.

### Task 4 – SQL Joins and Aggregation Analysis

Connect campaigns, leads, customers and investments using SQL.

Analyse:

- Leads and conversions by campaign and channel.
- Lead quality by source and campaign.
- AUM and AUM growth by customer segment and product.
- Value of customers associated with converted leads.
- Campaign and channel performance rankings.

**Required Deliverables:**

- Saved SQL queries with comments.
- Results summary linking campaign performance, lead quality and AUM growth.

### Task 5 – Hypothesis Testing and Distribution Analysis

Use cleaned data and exclude invalid records, including negative and 9999 processing or approval-time values.

Activities include:

- State null and alternative hypotheses.
- Select suitable statistical tests.
- Interpret results in business terms.
- Describe distributions for claim turnaround time, loan approval time and AUM growth.

**Required Deliverable:**

A concise statistics report stating each hypothesis, test used, result and business interpretation.

### Task 6 – Dashboard Design and Data Storytelling

Model relationships using shared keys and create departmental views for:

- Sales
- Marketing
- Operations
- Finance

The dashboard should:

- Include an executive summary connecting campaign-to-lead-to-policy or investment activity.
- Connect policy-to-claim activity.
- Connect customer-to-loan activity.
- Include cross-sell and delinquency analysis.
- Provide filters for region, product category and date.
- Include three to five recommendations, each supported by a dashboard metric.

**Required Deliverables:**

- Multi-page dashboard file or shared link.
- Short narrative explaining the findings and recommendations.

## 6. Expected Business Insights

The final analysis should identify:

- Agents, products and sales channels that contribute to policy sales, and assess agent productivity.
- Campaigns and channels that generate stronger leads and contribute to AUM growth.
- Areas of slow claim turnaround and the share of claims handled manually.
- Delinquency levels and higher-risk customer segments or credit-score bands.
- Extent of cross-sell activity among customers holding more than one product.

## 7. Recommendation Expectations

The final analysis should lead to prioritised, evidence-based actions.

Examples include:

- Redirecting effort towards productive agents and channels.
- Reallocating campaign budget towards stronger lead sources.
- Automating claim types associated with manual handling and slower turnaround.
- Tightening credit rules for score bands or segments with higher delinquency.

**Each recommendation must be supported by a number from the analysis.**

## 8. Working and Submission Guidelines

- Complete the six tasks in sequence because each task builds on the output of the preceding task.
- Use the appropriate tools:
  - GenAI chat tool for Task 1.
  - Excel for Task 3.
  - SQL for Task 4.
  - Statistical tools such as Excel, Python or R for Task 5.
  - Power BI or Looker Studio for Task 6.
- Preserve the original raw files.
- Perform cleaning on copies and maintain a log of all changes.
- Present findings in clear business language, stating both the result and its business meaning.
- Organise the submission into one folder per task, named Task1 through Task6.
- Include working files and a one-page summary for each task.
- Prepare one final document combining the summaries and recommendations.
- Use clear, descriptive filenames.

---

**Source Note:** This is a concise, reformatted summary of the supplied 12-page project brief. It preserves the stated scope and requirements while omitting the detailed data dictionary tables.
