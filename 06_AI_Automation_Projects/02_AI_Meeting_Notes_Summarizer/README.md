# AI Meeting Notes Summarizer

## Project Overview

The **AI Meeting Notes Summarizer** is an AI automation project that uses **Python, Prompt Engineering, and the OpenAI API** to convert unstructured meeting notes into clear, organized, and action-oriented business summaries.

Users can paste meeting notes directly into the application. The AI analyzes the content and identifies important updates, discussion points, decisions, action items, responsible people, deadlines, follow-up tasks, and the next meeting date.

This project demonstrates how AI can reduce the time required to review meeting notes and help teams quickly understand important outcomes and responsibilities.

---

## Features

* Accepts multi-line meeting notes through interactive user input
* Generates a concise meeting overview
* Identifies key project updates
* Extracts main discussion points
* Detects important decisions
* Extracts action items
* Identifies responsible people
* Identifies deadlines
* Separates completed work from future tasks
* Lists follow-up items
* Identifies the next meeting date
* Uses structured output for easy review
* Avoids inventing information not included in the meeting notes
* Handles missing information using `Not specified`
* Protects the API key using Google Colab Secrets

---

## Technologies Used

* **Python**
* **Google Colab**
* **OpenAI API**
* **OpenAI Python Library**
* **Prompt Engineering**
* **GitHub**

---

## How It Works

The application follows this workflow:

```text
Unstructured Meeting Notes
            ↓
Interactive Python Input
            ↓
Structured AI Prompt
            ↓
OpenAI API
            ↓
AI Analysis
            ↓
Organized Meeting Summary
            ↓
Updates, Decisions, Action Items, and Deadlines
```

---

## Input

Users paste their meeting notes directly into the Google Colab notebook.

Example:

```text
The sales team met to review monthly performance.

Amina reported that sales increased by 12 percent compared with the previous month.

The team agreed to focus more on repeat customers during the next campaign.

Bilal will prepare a customer retention plan by August 9.

The sales manager will review the plan and provide feedback by August 12.

The next sales meeting is scheduled for August 16.
```

After entering the notes, the user presses **Enter on an empty line** to finish the input.

---

## Example Output

 
## Meeting Overview

The sales team reviewed monthly performance and discussed strategies for improving customer retention.

## Key Updates

- Sales increased by 12% compared with the previous month.

## Main Discussion Points

- Monthly sales performance
- Customer retention
- The next sales campaign

## Key Decisions

- The team will focus more on repeat customers during the next campaign.

## Action Items

| Task | Responsible Person | Deadline |
|---|---|---|
| Prepare a customer retention plan | Bilal | August 9 |
| Review the customer retention plan and provide feedback | Sales Manager | August 12 |

## Follow-Up Items

- Review the customer retention plan.
- Discuss feedback during the next sales meeting.

## Next Meeting

- August 16
 

> The exact output may vary because AI-generated responses are dynamic.

---

## Project Structure

```text
02_AI_Meeting_Notes_Summarizer/
│
├── AI_Meeting_Notes_Summarizer.ipynb
└── README.md
```

---

## Installation and Setup

### 1. Open the Google Colab Notebook

Open:

```text
AI_Meeting_Notes_Summarizer.ipynb
```

### 2. Install the OpenAI Python Library

Run:

```python
!pip install -q openai
```

### 3. Create an OpenAI API Key

Create an API key through the OpenAI API Platform.

### 4. Add the API Key to Google Colab Secrets

In Google Colab:

1. Open the **Secrets** section from the left sidebar.
2. Click **Add a new secret**.
3. Enter:

```text
OPENAI_API_KEY
```

4. Paste the API key into the value field.
5. Enable **Notebook access**.

### 5. Load the API Key Securely

The notebook retrieves the API key using:

```python
from google.colab import userdata

api_key = userdata.get("OPENAI_API_KEY")
```

The actual API key is not stored in the notebook.

---

## How to Use

1. Open the Google Colab notebook.
2. Run the setup cells.
3. Paste meeting notes into the interactive input section.
4. Press **Enter on an empty line** after the final note.
5. Run the prompt-generation cell.
6. Run the AI-generation cell.
7. Review the structured meeting summary.
8. Use the extracted action items and deadlines for follow-up.

---

## Prompt Engineering Approach

The project uses a structured prompt containing:

1. **AI Role**
   Defines the AI as an expert business meeting analyst.

2. **Task**
   Instructs the AI to analyze and summarize meeting information.

3. **Meeting Notes**
   Provides the raw meeting content.

4. **Extraction Rules**
   Defines which information the AI should identify.

5. **Accuracy Rules**
   Instructs the AI not to invent names, dates, deadlines, or decisions.

6. **Action-Item Requirements**
   Requests the task, responsible person, and deadline.

7. **Output Structure**
   Organizes the result into consistent business sections.

The prompt structure is:

```text
AI Role
   ↓
Task
   ↓
Meeting Notes
   ↓
Extraction Rules
   ↓
Accuracy Requirements
   ↓
Required Output Format
```

This approach improves consistency and makes the generated summaries easier to review.

---

## Sample Use Cases

This tool can be used for:

* Project meetings
* Marketing team meetings
* Sales meetings
* Product development meetings
* Customer support meetings
* Client meetings
* Team progress updates
* Weekly business meetings
* Project status reviews
* Internal planning sessions

---

## Skills Demonstrated

This project demonstrates:

* Python programming
* AI automation
* Prompt engineering
* OpenAI API integration
* Multi-line user input handling
* Text processing
* AI-powered information extraction
* Meeting summarization
* Action-item extraction
* Deadline identification
* Responsible-person tracking
* AI output evaluation
* Prompt refinement
* Business communication
* GitHub project organization
* Secure API key management

---

## Testing

The application was tested using multiple business scenarios:

### Product Development Meeting

The AI successfully identified:

* Completed user-registration development
* Payment integration progress
* The decision to add password-reset functionality
* Ayesha’s requirements task
* Development deadlines
* Final testing plans
* The next meeting date

### Customer Support Meeting

The AI successfully identified:

* Customer response-time improvement
* Delivery-related customer complaints
* The decision to create an FAQ page
* Fatima’s FAQ preparation task
* Hassan’s complaint-analysis task
* Relevant deadlines
* The next meeting date

---

## Challenges and Learning Outcomes

During this project, I learned how to:

* Store unstructured meeting notes in Python
* Collect multi-line user input
* Use loops to process user-provided text
* Combine multiple input lines into one text block
* Create structured prompts for information extraction
* Connect Python applications to the OpenAI API
* Generate AI-powered meeting summaries
* Extract decisions, action items, responsibilities, and deadlines
* Separate completed work from future tasks
* Reduce AI hallucinations through explicit prompt instructions
* Test AI outputs using different business scenarios
* Improve output quality through prompt refinement
* Build an interactive AI automation workflow

---

## Future Improvements

Possible future enhancements include:

* Add a Streamlit web interface
* Upload meeting notes as `.txt`, `.docx`, or `.pdf` files
* Upload meeting transcripts
* Add meeting-title and meeting-date inputs
* Export summaries to PDF
* Export action items to Excel or CSV
* Add automated action-item reminders
* Send summaries by email
* Add multiple language support
* Create a searchable meeting-history database
* Add a meeting-summary dashboard
* Integrate with calendar applications
* Add speaker identification for meeting transcripts

---

## Security

The OpenAI API key is stored securely using **Google Colab Secrets**.

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
## Author

**Bakht Zamin**

AI Automation & Prompt Engineering | Data Analytics & Business Intelligence | Python | AI-Enabled Business Workflows



## License

This project was created for educational and portfolio purposes.

