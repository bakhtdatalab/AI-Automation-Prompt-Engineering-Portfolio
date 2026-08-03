# AI Business Report Generator

## Project Overview

The **AI Business Report Generator** is an AI-powered business analytics application that transforms structured business data into a professional, evidence-based, and decision-focused business performance report.

The project combines **Python**, **pandas**, **data analysis**, **prompt engineering**, and the **OpenAI API** to calculate key business metrics and generate clear business insights, performance observations, risk areas, and actionable recommendations.

Python is used to prepare and validate the data and calculate business metrics. The AI model then interprets the validated information and presents it in a structured business-report format.

---

## Business Problem

Business data is often stored as raw numbers that can be difficult and time-consuming to interpret.

Business owners, analysts, and managers may need to review:

* Revenue performance
* Business expenses
* Profit and profit margins
* Customer growth
* Marketing spending
* Customer acquisition cost
* Business strengths
* Performance risks
* Recommended actions

Creating a clear report manually can require significant time and analytical effort.

This project demonstrates how AI automation can support the business-reporting process by converting structured data into a readable and decision-focused report.

---

## Project Goal

The goal of this project is to automate business reporting by combining Python-based calculations with AI-generated analysis.

The application is designed to:

1. Collect or process business-performance data.
2. Calculate important business metrics with Python.
3. Prepare a structured business-data summary.
4. Send the validated data to the OpenAI API.
5. Generate a professional business-performance report.
6. Identify data-supported strengths and areas requiring attention.
7. Provide prioritized recommendations and follow-up metrics.
8. Clearly explain the limitations of the available data.

---

## Key Features

* Creates and analyzes monthly business datasets.
* Calculates total revenue.
* Calculates total expenses.
* Calculates total profit.
* Calculates profit margins.
* Calculates month-to-month revenue growth.
* Calculates customer acquisition cost.
* Identifies high-performing and low-performing periods.
* Generates AI-powered business reports.
* Produces executive summaries.
* Analyzes revenue, expenses, profit, customers, and marketing performance.
* Identifies data-supported business strengths.
* Highlights risks and areas requiring further investigation.
* Generates prioritized business recommendations.
* Suggests measurable follow-up metrics.
* Explains data limitations.
* Includes an interactive business-report workflow.
* Validates important user inputs.
* Avoids unsupported trend and causation claims.

---

## Technologies Used

| Technology         | Purpose                                                            |
| ------------------ | ------------------------------------------------------------------ |
| Python             | Data processing, calculations, validation, and workflow automation |
| pandas             | Creating and analyzing structured business datasets                |
| OpenAI API         | Generating AI-powered business reports                             |
| Prompt Engineering | Creating structured, accurate, and evidence-based AI instructions  |
| Google Colab       | Developing, testing, and running the project                       |
| GitHub             | Version control and portfolio presentation                         |

---

## Project Workflow

```text
Business Data
      ↓
Python Data Preparation
      ↓
Business Metric Calculations
      ↓
Input Validation
      ↓
Structured Business Summary
      ↓
Evidence-Based AI Prompt
      ↓
OpenAI API
      ↓
Professional Business Report
      ↓
Insights, Risks, and Recommendations
```

---

## Business Metrics Calculated

The project calculates the following metrics before sending the information to the AI model.

### Total Revenue

```text
Total Revenue = Sum of Revenue Values
```

### Total Expenses

```text
Total Expenses = Sum of Expense Values
```

### Total Profit

```text
Profit = Revenue − Expenses
```

### Profit Margin

```text
Profit Margin (%) = Profit ÷ Revenue × 100
```

### Revenue Growth

```text
Revenue Growth (%) =
(Current Revenue − Previous Revenue)
÷ Previous Revenue × 100
```

### Customer Acquisition Cost

```text
Customer Acquisition Cost =
Total Marketing Spend ÷ Total New Customers
```

Calculating these metrics with Python improves transparency and reduces the need for the AI model to perform the core calculations.

---

## AI Report Structure

The AI-generated report includes:

1. Business Name
2. Reporting Period
3. Executive Summary
4. Key Performance Metrics
5. Revenue Performance Analysis
6. Expense and Profit Analysis
7. Customer Growth and Marketing Analysis
8. Key Performance Highlights
9. Business Strengths
10. Risks and Areas for Attention
11. Recommended Actions
12. Suggested Follow-Up Metrics
13. Data Limitations
14. Conclusion

---

## Prompt Engineering Approach

The project uses a structured prompt to improve report quality and reduce unsupported conclusions.

The prompt instructs the AI to:

* Use only the provided business data and calculated metrics.
* Avoid inventing financial figures.
* Avoid inventing market conditions.
* Avoid inventing customer behavior.
* Avoid inventing competitor information.
* Avoid assigning unsupported causes to business results.
* Avoid treating correlation as proof of causation.
* Avoid unsupported predictions or forecasts.
* Clearly distinguish facts from observations.
* Clearly distinguish observations from recommendations.
* Identify information gaps.
* Connect recommendations to data-supported observations.
* Assign a priority level to each recommendation.
* Suggest measurable follow-up metrics.
* Explain the limitations of the available data.

---

## Testing

The project was tested using multiple business scenarios.

### Scenario 1: Consistent Business Growth

The first scenario included:

* Increasing monthly revenue
* Increasing profit
* Improving profit margins
* Growing new-customer acquisition
* Increasing marketing investment

Python calculated:

| Metric                    |               Result |
| ------------------------- | -------------------: |
| Total Revenue             |             $837,000 |
| Total Expenses            |             $550,000 |
| Total Profit              |             $287,000 |
| Overall Profit Margin     |               34.29% |
| Total New Customers       |                3,090 |
| Total Marketing Spend     |              $89,000 |
| Customer Acquisition Cost | Approximately $28.80 |

The AI-generated report identified:

* Positive revenue performance
* Strong profit growth
* Improving profit margins
* Customer-growth progress
* Data-supported business strengths
* Practical business recommendations

---

### Scenario 2: Mixed Business Performance

The second scenario included:

* Revenue growth followed by a decline
* Increasing expenses
* Falling profit
* Declining profit margins
* Reduced new-customer acquisition
* Increasing marketing spending

Python calculated:

| Metric                    |               Result |
| ------------------------- | -------------------: |
| Total Revenue             |             $935,000 |
| Total Expenses            |             $671,000 |
| Total Profit              |             $264,000 |
| Overall Profit Margin     |               28.24% |
| Total New Customers       |                3,630 |
| Total Marketing Spend     |             $131,000 |
| Customer Acquisition Cost | Approximately $36.09 |

The report was evaluated to confirm that the AI:

* Identified the revenue pattern accurately.
* Recognized increasing expenses.
* Identified the decline in profitability.
* Highlighted the reduction in new-customer acquisition.
* Identified the increase in marketing spending.
* Avoided claiming that marketing spending caused customer changes.
* Treated the relationship as an area requiring further investigation.
* Connected recommendations to the available data.
* Included priorities and follow-up metrics.
* Explained important data limitations.

---

### Interactive Testing

The interactive workflow was tested using multiple business inputs.

Users entered:

* Business name
* Reporting period
* Total revenue
* Total expenses
* Total new customers
* Total marketing spend

Python then calculated:

* Total profit
* Profit margin
* Customer acquisition cost

The OpenAI API generated a structured business report using the validated metrics.

Input validation was included to prevent:

* Zero or negative revenue values
* Zero or negative customer counts
* Negative expenses
* Negative marketing-spend values
* Division-by-zero calculation errors

---

## Sample Business Input

```text
Business Name:
NovaFit

Reporting Period:
July to December 2026

Total Revenue:
$950,000

Total Expenses:
$670,000

Total New Customers:
4,100

Total Marketing Spend:
$145,000
```

---

## Sample Calculated Output

```text
Total Profit:
$280,000

Profit Margin:
29.47%

Customer Acquisition Cost:
$35.37
```

---

## Example AI Report Output

The AI generates a structured report containing:

```text
Business Performance Report

Business Name:
NovaFit

Reporting Period:
July to December 2026

Executive Summary:
The business generated $950,000 in revenue and
$280,000 in profit during the reporting period.
The overall profit margin was 29.47%.

Key Performance Metrics:
- Total Revenue: $950,000
- Total Expenses: $670,000
- Total Profit: $280,000
- Profit Margin: 29.47%
- Total New Customers: 4,100
- Total Marketing Spend: $145,000
- Customer Acquisition Cost: $35.37

Recommended Actions:
1. High Priority:
   Review major expense categories and monitor
   profit-margin performance.

2. Medium Priority:
   Monitor customer acquisition cost by marketing
   channel when channel-level data is available.

3. Medium Priority:
   Track revenue, expenses, and customer acquisition
   monthly to identify performance trends.

Data Limitations:
Monthly performance data, expense categories,
marketing-channel data, and historical comparisons
would improve the analysis.
```

AI-generated wording may vary.

---

## How to Run the Project

### 1. Open the Google Colab Notebook

Open:

```text
AI_Business_Report_Generator.ipynb
```

### 2. Install the Required Libraries

```python
!pip install -q openai pandas
```

### 3. Add Your OpenAI API Key

Store the API key in Google Colab Secrets using:

```text
OPENAI_API_KEY
```

Enable **Notebook access** for the secret.

Do not place the API key directly in the notebook or upload it to GitHub.

### 4. Run the Notebook

Run the cells in order.

The notebook will:

1. Create or collect business data.
2. Validate the inputs.
3. Calculate business metrics.
4. Build a structured business summary.
5. Create the AI business-report prompt.
6. Send the prompt to the OpenAI API.
7. Display the generated business report.

---

## Project Structure

```text
06_AI_Business_Report_Generator/
│
├── AI_Business_Report_Generator.ipynb
│
├── README.md
│
└── sample_outputs/
    ├── growth_business_report.txt
    └── mixed_performance_report.txt
```

The `sample_outputs` folder is optional but recommended for portfolio presentation.

---

## Important Limitations

This project is designed as an AI-assisted business-reporting tool.

The generated report:

* Is not financial, legal, tax, or investment advice.
* Should be reviewed before being used for important business decisions.
* Is limited by the quality and completeness of the input data.
* Cannot determine the cause of a performance change unless supporting evidence is provided.
* Should not be used as a replacement for professional financial analysis.
* May require additional historical, operational, customer, or market data for deeper analysis.

---

## Future Improvements

Potential future improvements include:

* Uploading business data from CSV files.
* Uploading Excel business reports.
* Adding monthly, quarterly, and yearly reporting options.
* Creating revenue and profit charts.
* Adding expense-category analysis.
* Adding marketing-channel analysis.
* Adding customer-retention metrics.
* Comparing current performance with previous periods.
* Exporting reports as PDF files.
* Exporting reports as Word documents.
* Creating an interactive Streamlit web application.
* Adding automated data-quality checks.
* Adding business-performance dashboards.
* Supporting multiple businesses and reporting periods.

---

## Skills Demonstrated

This project demonstrates:

* Python programming
* Data analysis
* pandas DataFrame operations
* Business-metric calculations
* Financial-performance analysis
* Data validation
* Prompt engineering
* OpenAI API integration
* AI workflow automation
* Business-report generation
* Trend analysis
* Evidence-based AI reporting
* Risk identification
* Business recommendation design
* Interactive application development
* Google Colab
* GitHub project documentation

---

## Portfolio Value

This project demonstrates how AI can be combined with data analysis to automate a practical business workflow.

Rather than relying on an AI model to calculate and interpret everything, the application separates responsibilities:

```text
Python:
Data preparation, validation, and calculations

AI:
Interpretation, report organization,
business insights, and recommendations
```

This approach improves transparency, reproducibility, and control over the business-reporting workflow.

---

## Author

**Bakht Zamin**

AI Automation | Python | Data Analytics | Digital Marketing | E-commerce | Prompt Engineering

---

## Project Status

✅ Completed

Part of a 7-project AI Automation Portfolio.

## Project Status

In Progress
