# AI Content Calendar Generator

## Project Overview

The **AI Content Calendar Generator** is an AI-powered marketing automation project that uses **Python, Prompt Engineering, and the OpenAI API** to create structured, platform-specific social media content calendars.

Users enter business information, industry details, target-audience information, marketing goals, a social media platform, and the desired calendar duration. The AI then generates a practical content strategy and a day-by-day content calendar.

Each calendar includes content pillars, topics, recommended formats, content ideas, calls to action, and relevant hashtags.

This project demonstrates how AI can support digital marketing and e-commerce workflows by reducing the time required to plan, organize, and develop social media content.

---

## Features

* Collects business and marketing information through interactive user input
* Generates one content idea for each requested day
* Creates a short content strategy overview
* Identifies relevant content pillars
* Suggests platform-appropriate content formats
* Generates business-specific content topics
* Creates practical content ideas
* Includes clear calls to action
* Suggests 3 to 5 relevant hashtags for each post
* Balances educational, engaging, trust-building, brand-awareness, and promotional content
* Avoids repetitive content topics and formats
* Adapts content to the selected social media platform
* Supports different industries, businesses, audiences, and marketing goals
* Avoids inventing unsupported product claims, discounts, or customer results
* Protects the API key using Google Colab Secrets

---

## Technologies Used

* **Python**
* **Google Colab**
* **OpenAI API**
* **OpenAI Python Library**
* **Prompt Engineering**
* **Digital Marketing**
* **Content Strategy**
* **GitHub**

---

## How It Works

The application follows this workflow:

```text
Business Information
        ↓
Marketing Requirements
        ↓
Interactive Python Input
        ↓
Structured AI Prompt
        ↓
OpenAI API
        ↓
Content Strategy Generation
        ↓
Platform-Specific Content Calendar
```

---

## Input

Users enter the following information:

* Business or brand name
* Industry or niche
* Target audience
* Primary marketing goal
* Social media platform
* Content-calendar duration

Example:

```text
Business Name: UrbanCraft Store

Industry: Handmade home decor and personalized gifts

Target Audience:
Adults aged 25 to 45 who are interested in unique home decor,
thoughtful gifts, and supporting small businesses

Marketing Goal:
Increase product awareness, build customer trust,
and encourage visits to the online store

Platform: Instagram

Duration: 7 days
```

---

## Example Output

```text
## Content Strategy Overview

The strategy combines product storytelling, behind-the-scenes content,
home-decor education, customer-focused content, and product promotion.
The content is designed to increase awareness, build trust, and encourage
visits to the UrbanCraft Store online shop.

## 7-Day Content Calendar

| Day | Content Pillar | Topic | Format | Content Idea | Call to Action | Hashtags |
|---|---|---|---|---|---|---|
| Day 1 | Brand Awareness | Brand Story | Instagram Reel | Introduce the story and purpose behind UrbanCraft Store | Follow for handmade decor ideas | #HandmadeDecor #SmallBusiness #HomeDecor |
| Day 2 | Education | Home Styling | Carousel | Share simple ways to use handmade decor in a living space | Save these ideas for later | #HomeStyling #DecorIdeas #HandmadeHome |
| Day 3 | Trust Building | Creation Process | Reel | Show part of the process used to create a handmade product | Comment with your favorite design | #BehindTheScenes #HandmadeBusiness #Craftsmanship |
| Day 4 | Engagement | Personalized Gifts | Story | Ask followers which personalized gift they would choose | Vote in the poll | #GiftIdeas #PersonalizedGifts #InstagramStories |
| Day 5 | Product Awareness | Product Details | Carousel | Highlight the design and customization options of a featured item | Visit the online store to explore more | #UniqueGifts #HandmadeProducts #ShopSmall |
| Day 6 | Community | Customer Inspiration | Image Post | Share a customer-inspired home-decor idea without making unsupported claims | Tag a friend who would like this style | #HomeInspiration #DecorCommunity #SupportSmallBusiness |
| Day 7 | Promotion | Featured Product | Instagram Reel | Showcase a popular product and explain how it can be personalized | Visit the online store to view the collection | #HandmadeGifts #CustomDecor #ShopOnline |
```

> The exact output may vary because AI-generated content is dynamic.

---

## Project Structure

```text
03_AI_Content_Calendar_Generator/
│
├── AI_Content_Calendar_Generator.ipynb
└── README.md
```

---

## Installation and Setup

### 1. Open the Google Colab Notebook

Open:

```text
AI_Content_Calendar_Generator.ipynb
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
2. Run the installation and setup cells.
3. Enter the business or brand name.
4. Enter the industry or niche.
5. Describe the target audience.
6. Enter the primary marketing goal.
7. Enter the social media platform.
8. Enter the content-calendar duration.
9. Run the refined prompt cell.
10. Run the AI-generation cell.
11. Review the content strategy and calendar.
12. Adapt the generated ideas to the business’s actual brand voice and content resources.

---

## Prompt Engineering Approach

The project uses a structured prompt containing:

1. **AI Role**
   Defines the AI as an expert social media strategist, digital marketer, and content planner.

2. **Task**
   Instructs the AI to create a strategic and platform-specific content calendar.

3. **Business Information**
   Provides the business name, industry, target audience, and marketing goal.

4. **Platform Requirements**
   Instructs the AI to adapt content formats and ideas to the selected platform.

5. **Content Rules**
   Requires content variety, relevance, practicality, and alignment with business goals.

6. **Content Pillars**
   Balances educational, engaging, trust-building, brand-awareness, and promotional content.

7. **Accuracy Rules**
   Prevents unsupported claims about products, discounts, customer results, or business facts.

8. **Output Structure**
   Organizes the results into a strategy overview and a structured content calendar.

The prompt structure is:

```text
AI Role
   ↓
Task
   ↓
Business Information
   ↓
Marketing Goal
   ↓
Platform Requirements
   ↓
Content Rules
   ↓
Content Pillars
   ↓
Required Output Format
```

---

## Sample Use Cases

This tool can support:

* Small businesses
* E-commerce stores
* Digital marketers
* Content creators
* Personal brands
* Online education businesses
* Local businesses
* Service-based businesses
* Product launches
* Social media campaigns
* Brand-awareness campaigns
* Content-planning workflows

---

## Skills Demonstrated

This project demonstrates:

* Python programming
* AI automation
* Prompt engineering
* OpenAI API integration
* Interactive user input
* Digital marketing strategy
* Social media content planning
* Target-audience analysis
* Marketing-goal alignment
* Platform-specific content creation
* Content-pillar development
* Call-to-action generation
* Hashtag generation
* AI-output evaluation
* Prompt refinement
* E-commerce marketing
* GitHub project organization
* Secure API key management

---

## Testing

The application was tested using multiple business scenarios.

### GlowNaturals — TikTok

The AI generated content focused on:

* Beginner-friendly skincare education
* Product awareness
* Ingredient explanations
* Skincare routines
* Trust-building content
* Online-store visits

### TechStart Academy — LinkedIn

The AI generated content focused on:

* Technology and AI education
* Beginner learning tips
* Career-development content
* Professional engagement
* Course awareness
* Course registrations

### UrbanCraft Store — Instagram

The AI generated content focused on:

* Handmade home decor
* Personalized gifts
* Product storytelling
* Behind-the-scenes creation
* Home-styling ideas
* Customer trust
* Online-store visits

---

## Challenges and Learning Outcomes

During this project, I learned how to:

* Store business and marketing information in Python variables
* Collect interactive user input
* Convert user input into structured AI prompts
* Use a reusable prompt template for different businesses
* Connect Python applications to the OpenAI API
* Generate AI-powered marketing strategies
* Create platform-specific content calendars
* Use content pillars to organize marketing ideas
* Align content with target audiences and business goals
* Generate practical calls to action
* Generate relevant hashtags
* Reduce generic AI output through detailed prompt instructions
* Reduce unsupported business claims through accuracy rules
* Test AI outputs across industries and platforms
* Improve AI results through prompt refinement
* Build an interactive AI marketing automation workflow

---

## Future Improvements

Possible future enhancements include:

* Add a Streamlit web interface
* Add a calendar-style visual layout
* Allow users to select specific start dates
* Generate 30-day content calendars
* Add multiple social media platforms in one workflow
* Add brand-voice settings
* Add content-tone options
* Generate complete post captions
* Generate image or video prompts
* Export calendars to CSV or Excel
* Export calendars to PDF
* Add Google Calendar integration
* Add content scheduling
* Add competitor-content analysis
* Add content-performance tracking
* Create a marketing analytics dashboard

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

## License

This project was created for educational and portfolio purposes.

