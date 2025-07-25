# 🚆 Project-3: Railway Train Schedule

This project enables users to interact with Indian Railways data using [Cursor AI IDE](https://www.cursor.sh/) and an MCP (Multi-Channel Processor) server setup. Users can query train schedules, seat availability, and live statuses directly via AI-powered prompts in Cursor IDE.

---

## 🛠️ Prerequisites

### 1. MCP Server Configuration
- Ensure you have deployed and configured the **Indian Railways MCP Server**.
- Add the server’s URL to the MCP tab in Cursor IDE.

### 2. Cursor AI Setup
- You must have access to [Cursor IDE](https://www.cursor.sh/).
- Be familiar with using the **MCP** tab inside the interface.

---

## 🚀 Process

### ✅ Step 1: Set Up the Prompt in Cursor IDE
- Open **Cursor IDE** → Go to the **MCP tab**.
- Enter the following prompt to fetch train schedules:

### ✅ Step 2: Use the following Prompts
After entering the prompt, press Enter. <br>
Description: You will receive the all trains schedule on that date directly in Cursor. <br>
Prompt Example: <br>
```
Give me the {from place} to {to place} scheduled trains list on {date}.
```

Description: Get complete route and schedule of a specific train. <br>
Prompt Example: <br>
```
Get the train info: {Train name and number}
```

Description: Checks upcoming seat availability between stations for a specific train. <br>
Prompt Example: <br>
```
Get seat availability of {Train name and number}
```

Description: Real-time status including current location, delay info, and ETA. <br>
Prompt Example: <br>
```
Get train live status on date: {date}
train number: {Train name and number}
```
