# 📧 Project-2: Gmailing via MCP Integration

This project enables users to automate the job application process by leveraging Gmail and LinkedIn data through MCP (Multi-Channel Prompting) integration. It uses Pipedream as the backend server and Cursor IDE as the user interface for AI prompt execution. The system fetches personal LinkedIn details, generates a cover letter, and sends everything to a specified email address—all from a single prompt.

---

## 🚀 Prerequisites

### ✅ MCP Server Setup
- Create and deploy the Gmail & LinkedIn MCP Server on [Pipedream](https://pipedream.com/).
- Authenticate:
  - Your Gmail account for sending emails.
  - Your LinkedIn account for fetching profile information.

### ✅ Cursor IDE Setup
- Access [Cursor IDE](https://www.cursor.sh/) and make sure the MCP tab is visible and usable.
- You must be familiar with the AI Prompt Panel within Cursor.

---

## 🔧 Process

### 🔹 Step 1: Configure the MCP Server
- Visit [Pipedream](https://pipedream.com/) and deploy:
  - **Gmail MCP Server**
  - **LinkedIn MCP Server**
- Authenticate both your Gmail and LinkedIn accounts in the respective servers.
- Copy the MCP endpoint URL(s) once setup is complete.

### 🔹 Step 2: Connect MCP with Cursor IDE
- Open **Cursor IDE**.
- Navigate to the **MCP** tab.
- Paste the **MCP server URL** obtained from Pipedream into the designated field in Cursor.

### 🔹 Step 3: Create Your Prompt
- Open the **AI Panel** in Cursor IDE and input the following prompt:

```text
Get my details from LinkedIn, apply for a job at {company name}, write a short cover letter, and send everything to {mail}.
