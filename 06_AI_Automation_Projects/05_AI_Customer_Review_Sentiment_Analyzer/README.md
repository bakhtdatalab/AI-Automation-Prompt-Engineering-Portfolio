# AI Customer Review Sentiment Analyzer

## Project Overview

The **AI Customer Review Sentiment Analyzer** is an AI-powered customer-feedback analytics project built with **Python, pandas, Prompt Engineering, Google Colab, and the OpenAI API**.

The application analyzes unstructured customer reviews and converts them into structured customer insights. It identifies overall sentiment, extracts positive and negative feedback, detects important themes, highlights customer concerns, and generates practical business recommendations.

The project supports both **single-review analysis** and **batch review analysis**. Batch results are stored in a pandas DataFrame and summarized using sentiment counts and percentages.

This project demonstrates how artificial intelligence can support e-commerce, customer experience, product improvement, and business decision-making by transforming written customer feedback into actionable insights.

---

## Features

* Analyzes individual customer reviews
* Supports interactive customer-review input
* Analyzes multiple customer reviews in a batch
* Classifies each review as:

  * Positive
  * Negative
  * Neutral
  * Mixed
* Assigns an AI confidence level
* Extracts evidence-based feedback
* Identifies positive customer experiences
* Identifies negative customer experiences
* Detects key customer-feedback themes
* Highlights the main customer concern
* Generates practical business actions
* Creates overall customer-insight summaries
* Counts sentiment categories
* Calculates sentiment percentages
* Stores results in a pandas DataFrame
* Uses reusable Python functions
* Applies structured prompt-engineering techniques
* Includes rules to reduce unsupported claims
* Supports e-commerce and customer-experience analysis

---

## Technologies Used

* **Python**
* **pandas**
* **Google Colab**
* **OpenAI API**
* **OpenAI Python Library**
* **Prompt Engineering**
* **AI Automation**
* **Sentiment Analysis**
* **Customer Analytics**
* **Data Analysis**
* **Business Intelligence**
* **E-commerce Analytics**
* **GitHub**

---

## How It Works

```text
Customer Reviews
        ↓
Python Review Dataset
        ↓
Structured AI Prompt
        ↓
OpenAI API
        ↓
Sentiment Classification
        ↓
Customer Feedback Analysis
        ↓
Key Themes and Concerns
        ↓
Business Recommendations
        ↓
pandas Sentiment Summary
```

---

## Sentiment Categories

The AI assigns exactly one sentiment category to each review.

### Positive

The review is mainly favorable and expresses satisfaction, approval, or a positive customer experience.

### Negative

The review is mainly unfavorable and expresses dissatisfaction, complaints, frustration, product failure, or a negative customer experience.

### Neutral

The review is mainly factual, informational, uncertain, or observational and does not contain a meaningful positive or negative overall judgment.

### Mixed

The review contains meaningful positive and negative feedback.

---

## Input

The application accepts customer-review text.

### Example Input

```text
The wireless earbuds are comfortable and the sound quality is clear.
However, the battery drains faster than I expected, and the charging
case feels less durable than the earbuds themselves.
```

---

## Example Output

```text
## Sentiment

Sentiment: Mixed
Confidence: High

## Evidence

- The customer describes the earbuds as comfortable.
- The customer reports clear sound quality.
- The customer states that the battery drains faster than expected.
- The customer expresses concern about the charging case's durability.

## Positive Feedback

- Comfortable fit
- Clear sound quality

## Negative Feedback

- Battery performance did not meet expectations
- Concern about charging-case durability

## Key Themes

- Comfort
- Sound quality
- Battery performance
- Product durability

## Main Customer Concern

Battery life and the perceived durability of the charging case.

## Suggested Business Action

Review customer feedback related to battery performance and
charging-case durability, then investigate whether these concerns
appear consistently across a larger group of customers.
```

> AI-generated results may vary. All outputs should be reviewed before being used for important business decisions.

---

## Project Structure

```text
05_AI_Customer_Review_Sentiment_Analyzer/
│
├── AI_Customer_Review_Sentiment_Analyzer.ipynb
└── README.md
```

---

## Installation and Setup

### 1. Open the Google Colab Notebook

Open:

```text
AI_Customer_Review_Sentiment_Analyzer.ipynb
```

### 2. Install the OpenAI Python Library

Run:

```python
!pip install -q openai
```

### 3. Import pandas

Run:

```python
import pandas as pd
```

### 4. Create an OpenAI API Key

Create an API key through the OpenAI API Platform.

### 5. Add the API Key to Google Colab Secrets

In Google Colab:

1. Open the **Secrets** section from the left sidebar.
2. Click **Add a new secret**.
3. Use the following secret name:

```text
OPENAI_API_KEY
```

4. Paste the API key into the value field.
5. Enable **Notebook access**.

### 6. Load the API Key Securely

```python
from google.colab import userdata

api_key = userdata.get("OPENAI_API_KEY")
```

### 7. Create the OpenAI Client

```python
from openai import OpenAI

client = OpenAI(api_key=api_key)
```

---

## How to Use

### Analyze One Customer Review

1. Open the Google Colab notebook.
2. Run the installation and setup cells.
3. Enter a customer review.
4. Run the interactive prompt cell.
5. Run the AI-analysis cell.
6. Review the sentiment classification and customer insights.

### Analyze Multiple Customer Reviews

1. Add customer reviews to the batch dataset.
2. Run the reusable analysis function.
3. Analyze each review through the OpenAI API.
4. Store the results in a Python list.
5. Create a pandas DataFrame.
6. Extract sentiment labels.
7. Calculate sentiment counts.
8. Calculate sentiment percentages.
9. Review the business interpretation.

---

## Prompt Engineering Approach

The project uses a structured prompt with the following components:

### 1. AI Role

The AI is assigned the roles of:

* Customer-insights analyst
* Sentiment-analysis specialist
* E-commerce analyst
* Business-intelligence assistant

### 2. Customer Review Data

The prompt includes the customer-review text and its review ID when applicable.

### 3. Clear Sentiment Definitions

The prompt defines:

* Positive
* Negative
* Neutral
* Mixed

Clear definitions help improve classification consistency.

### 4. Evidence-Based Rules

The AI is instructed to:

* Analyze each review independently
* Assign exactly one sentiment label
* Use only the four approved labels
* Base the result on the customer’s overall message
* Use only information stated or clearly supported by the review
* Avoid inventing product details
* Avoid inventing customer experiences
* Avoid inventing causes or business facts
* Avoid assuming that one review represents all customers
* Separate review evidence from business recommendations
* Avoid guessing when information is missing

### 5. Structured Output

Each review is analyzed using:

```text
Review ID
    ↓
Sentiment
    ↓
Confidence
    ↓
Evidence
    ↓
Positive Feedback
    ↓
Negative Feedback
    ↓
Key Themes
    ↓
Customer Concern
    ↓
Suggested Business Action
```

### 6. Business-Level Insights

For multiple reviews, the AI generates:

* Overall sentiment summary
* Common positive themes
* Common negative themes
* Main customer concerns
* Recommended business priorities

---

## Batch Analysis Workflow

The project uses a reusable Python function to analyze multiple reviews.

```python
def analyze_review(review_text):
    """
    Analyzes one customer review and returns
    an AI-generated sentiment analysis.
    """

    # Create the prompt
    # Send the request to the OpenAI API
    # Return the generated analysis
```

The function is applied to each review in the dataset.

The results are stored in a structured format containing:

* Review ID
* Customer review
* AI-generated analysis
* Extracted sentiment label

---

## Data Analysis

The batch results are converted into a pandas DataFrame.

Example:

| Review ID | Sentiment | Customer Review                              |
| --------: | --------- | -------------------------------------------- |
|       201 | Positive  | Comfortable and easy to use                  |
|       202 | Mixed     | Modern design but connection issues          |
|       203 | Neutral   | Limited experience with the product          |
|       204 | Mixed     | Clear display but battery concerns           |
|       205 | Negative  | Product failure and unresolved support issue |
|       206 | Positive  | Easy setup and useful tracking               |

The project then calculates:

* Number of reviews in each sentiment category
* Percentage of reviews in each sentiment category

Example summary:

| Sentiment | Review Count | Percentage |
| --------- | -----------: | ---------: |
| Positive  |            2 |      33.3% |
| Mixed     |            2 |      33.3% |
| Neutral   |            1 |      16.7% |
| Negative  |            1 |      16.7% |

> The exact results may vary because AI-generated classifications can differ depending on the review content and model output.

---

## Testing

The analyzer was tested with multiple review types.

### Positive Reviews

Tested for:

* Customer satisfaction
* Product comfort
* Clear product performance
* Ease of use
* Battery performance
* Positive recommendations

### Negative Reviews

Tested for:

* Product failure
* Connection problems
* Charging problems
* Unclear instructions
* Customer-support issues
* Customer dissatisfaction

### Neutral Reviews

Tested for:

* Limited product experience
* Factual delivery information
* Early product use
* Uncertain customer opinions

### Mixed Reviews

Tested for:

* Positive product features combined with performance concerns
* Attractive design combined with connection issues
* Good comfort combined with battery concerns
* Useful features combined with durability concerns

---

## Business Interpretation

The sentiment summary provides a high-level view of customer feedback.

Positive feedback may help businesses:

* Identify product strengths
* Improve marketing messages
* Highlight valued features
* Understand customer satisfaction

Mixed and negative feedback may help businesses:

* Identify recurring customer concerns
* Investigate product-quality issues
* Improve usability
* Improve customer support
* Prioritize product improvements

The results should be treated as an initial customer-insights signal rather than a final business conclusion. A larger dataset, additional analysis, and human review would be needed before making major business decisions.

---

## Skills Demonstrated

This project demonstrates:

* Python programming
* AI automation
* OpenAI API integration
* Prompt engineering
* Sentiment analysis
* Customer-feedback analysis
* Data cleaning and organization
* Interactive user input
* Reusable Python functions
* Python lists and dictionaries
* Text processing
* AI-output parsing
* pandas DataFrames
* Data aggregation
* Sentiment counts
* Percentage calculations
* Customer-insight generation
* Business-intelligence thinking
* E-commerce analytics
* AI-output evaluation
* Prompt refinement
* GitHub project organization
* Secure API key management

---

## Challenges and Learning Outcomes

During this project, I learned how to:

* Convert unstructured customer reviews into structured AI insights
* Define clear sentiment categories
* Create evidence-based sentiment-analysis prompts
* Classify positive, negative, neutral, and mixed reviews
* Add confidence levels to AI analysis
* Extract positive and negative feedback
* Identify customer-feedback themes
* Identify customer concerns
* Generate practical business actions
* Build an interactive AI application
* Create reusable Python functions
* Analyze multiple reviews automatically
* Extract sentiment labels from AI-generated text
* Store AI results in a pandas DataFrame
* Calculate sentiment counts and percentages
* Interpret customer feedback for business use
* Test and refine AI prompts
* Reduce unsupported AI claims
* Build an AI-powered customer-analytics workflow

---

## Limitations

* AI sentiment classifications may vary.
* Short or ambiguous reviews may be difficult to classify.
* AI output should be reviewed before making important business decisions.
* A small dataset may not represent the full customer population.
* One customer review should not be treated as proof of a widespread issue.
* The current version uses text-based output rather than a strict structured-data format.
* Batch analysis makes one API request per review, which may increase processing time and API costs.

---

## Future Improvements

Possible future enhancements include:

* Add JSON-structured AI output
* Add automatic sentiment validation
* Add sentiment visualizations
* Create bar charts and pie charts
* Add customer-review CSV uploads
* Add Excel-file support
* Add bulk review processing
* Add sentiment trends over time
* Add product-level sentiment comparisons
* Add topic-frequency analysis
* Add keyword extraction
* Add customer-support issue detection
* Add review-priority scoring
* Add automatic alerting for serious complaints
* Add a Streamlit dashboard
* Add interactive data filters
* Add multilingual review analysis
* Add export to CSV or Excel
* Add database integration
* Add Shopify review integration
* Add WooCommerce review integration
* Add human-review workflows

---

## Security

The OpenAI API key is stored using **Google Colab Secrets**.

The API key is:

* Not written directly in the Python code
* Not included in the GitHub repository
* Not displayed in notebook output
* Not shared publicly

---

## Project Status

**Completed — Version 1.0**

---

## Author

**Bakht Zamin**

Aspiring AI Automation Specialist | Python Developer | Data Analyst

Portfolio Areas:

* Python
* AI Automation
* Data Analytics
* Prompt Engineering
* Digital Marketing
* E-commerce

---

## License

This project was created for educational and portfolio purposes.
