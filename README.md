
# 📈 AI-Powered Equity Research Agent

## 📝 Description

The **AI-Powered Equity Research Agent** is an automated, end-to-end workflow designed to accelerate the stock analysis process. Instead of manually scraping financial statements, social sentiment, and news articles, a user simply sends a trigger email with a target company. The agent automatically extracts the company entity, runs parallel deep-dive web searches across major financial and social platforms, synthesizes the findings using LLMs, and delivers a formatted, comprehensive PDF equity report right back to the user's inbox.

This tool is built for investors, financial analysts, and researchers who want to eliminate the manual data-gathering phase of stock picking and focus purely on decision-making.

---

## ✨ Key Features

* **Zero-Friction Trigger:** The entire pipeline initiates the moment an email is sent to the agent.
* **Multi-Source Intelligence:** Aggregates data from Yahoo Finance, LinkedIn, X (Twitter), and general market news.
* **Comprehensive Synthesis:** Uses specialized AI prompts to evaluate fundamentals, corporate sentiment, and technical analyst commentary.
* **Automated Document Generation:** Compiles the research into a Google Doc, converts it to a professional PDF, and emails it back to the user.

---

## 🧠 The Intelligence Engine (Core Prompts)

The agent utilizes three specialized AI prompts to gather and process a 360-degree view of the target asset:

1. **Corporate & Social Intelligence:** > *"Search LinkedIn, X (formerly Twitter), and the web for the latest company information and updates about the following company: size, growth, leadership or executive changes, and any noteworthy news relevant to a stock investment decision. Focus on the most recent and relevant public information..."*
2. **Fundamental & Financial Data:** > *"Search Yahoo Finance and the web for the latest financial data and news about the following company. Include revenue, earnings, P/E ratio, and key performance indicators, and summarize information relevant for making a stock pick decision..."*
3. **Market Sentiment & Technicals:** > *"Search the web for market news, analyst commentary, technical analysis, and any other available information for the following company. Prioritize current trends, market sentiment, and analyst recommendations relevant to an investment decision..."*

---

## ⚙️ Workflow Architecture

This project utilizes a no-code/low-code workflow automation platform to chain together the following steps:

1. **Trigger (Gmail):** Monitors for an outgoing "Email sent" containing the target company.
2. **AI Extraction:** Parses the email content to identify the specific stock ticker or company name.
3. **Parallel Data Collection:**
* Pulls weekly financial data via Yahoo Finance.
* Scrapes weekly company insights via LinkedIn/Socials.
* Aggregates the last 7 days of market news.


4. **Generative AI Synthesis:** Feeds the collected data into an LLM to generate a structured equity research report.
5. **Document Creation (Google Docs):** Drafts the weekly equity report into a formatted Google Document.
6. **PDF Export:** Converts the drafted document into a finalized PDF.
7. **Delivery (Gmail):** Emails the finished PDF report directly back to the user.

---

## 🛠️ Tech Stack & Integrations

* **Automation Platform:** [Insert your platform here, e.g., Relay.app, Zapier, Make]
* **Communication:** Gmail
* **Data Sources:** Yahoo Finance, LinkedIn, Web Search APIs
* **AI/LLM:** [Insert LLM here, e.g., OpenAI GPT-4]
* **Document Management:** Google Docs, Google Drive

---

## 🚀 Potential Future Enhancements

* **Portfolio Tracking:** Allow the agent to process a list of tickers in a single email and return a consolidated market overview.
* **Competitor Analysis:** Automatically trigger secondary workflows to analyze the target company's top 3 competitors for a comparative matrix.
* **Price Alerts:** Integrate technical triggers (e.g., RSI or Moving Average crosses) to initiate the research report autonomously rather than relying on a manual email trigger.
