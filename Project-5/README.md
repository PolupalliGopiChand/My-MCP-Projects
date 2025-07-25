# 🎯 Project 5: Learning Path Generator

This project is an AI-powered Learning Path Generator that integrates with YouTube, Google Drive, and Notion to generate and deliver customized learning paths based on user input. It utilizes Gemini AI (from Google AI Studio) as the core intelligence layer, and uses Pipedream MCP servers to seamlessly fetch relevant content from your connected services.

---

## ⚙️ Prerequisites

Ensure the following are set up before running the project:

- ✅ Gemini API Key from [Google AI Studio](https://makersuite.google.com/)
- ✅ Authorized Pipedream MCP servers for:
  - YouTube
  - Google Drive
  - Notion
- ✅ Python 3.10+
- ✅ Cursor IDE (or any preferred Python IDE)

---

## 🔐 How to Get Gemini AI Studio API Key

1. Go to [Google AI Studio](https://makersuite.google.com/)
2. Log in using your Google account.
3. Click on **“Get API Key”** from the left sidebar.
4. Click **“Create API Key”** (You can also use an existing project).
5. Once generated, **copy** your API key.

---

## 🔗 How to Set Up Pipedream MCP Servers

1. Visit Pipedream and log in with your Google account.
2. Set up each MCP server below:
   - [YouTube MCP Server](https://pipedream.com/@your-yt-mcp-server)
   - [Google Drive MCP Server](https://pipedream.com/@your-drive-mcp-server)
   - [Notion MCP Server](https://pipedream.com/@your-notion-mcp-server)
3. For each service:
   - Connect your Google/Notion account.
   - Authorize all necessary permissions.
   - Copy the endpoint URL for each service — you'll need it in your app config.

---

## 🧰 Project Setup Guide
Step 1: Navigate to Your Home Directory (Optional, but Recommended Starting Point

---

Step 2: Clone the Repository
[github repo](https://github.com/revanthgopi-nw/mcp-learning-path-demo)

---

Step 3: Open the Project Folder with the Cursor IDE:
- Open the cursor, click on the “file” (left side, top corner)
- Click on the “Open Folder”, select our unzipped folder
- Now, your project file is open in your Cursor IDE

---

Step 4: Create a Virtual Environment
- Run the following command while inside the project directory:
  ```
  python -m venv venv
  ```
- Explanation: This command uses the venv module from Python's standard library to create a virtual environment named venv inside your current directory (project directory).

---

Step 5: Activate the Virtual Environment
- On Ubuntu (or other Linux/macOS):
  ```
  source venv/bin/activate
  ```
- On Windows: Using Command Prompt (cmd.exe):
  ```
  venv\Scripts\activate
  ```
- Verification: After activation, your terminal prompt should change, typically showing (venv) at the beginning, like this:
(venv) yourusername@yourcomputer:~/mcplearningpath_generator$

---

Step 6: Install Requirements
- Install the listed packages using pip. Run this command inside the activated virtual environment:
  ```
  pip install -r requirements.txt
  ```

---

Step 7: Install Requirements
- Run the app.py file from your terminal by using streamlit
  ```
  streamlit run app.py
  ```
- The application will be available at Local Host Streamlit by default.
---
