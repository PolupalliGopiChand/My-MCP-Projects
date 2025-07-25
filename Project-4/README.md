# ☎️ Project-4: Tech Updates Phone Calling

This project uses **Eleven Labs** and **Twilio** to create a conversational AI voice agent that makes outbound calls and delivers daily **tech updates**. Integrated with the **Cursor IDE MCP server**, the setup allows users to simulate or initiate real phone calls using AI-generated voices to share curated tech news.

---

## 🔧 Prerequisites

- **Eleven Labs Account** – For generating voice AI and managing call agents.
- **Twilio Account** – For buying numbers and handling phone call operations.
- **Cursor IDE** – To interact with the MCP configuration and run terminal commands.
- **Python 3.10+** – Ensure Python is installed and the environment is properly set up.

---

## 🚀 Setup Instructions

### ✅ Step 1: Eleven Labs API Configuration

1. Go to [Eleven Labs](https://www.elevenlabs.io) and **create an account**.
2. Click your profile icon (bottom left) → Select **API Keys**.
3. **Create API Key** → Uncheck **Restrict Key** → Copy and save it for later use.

---

### ✅ Step 2: Twilio Configuration

1. Go to [Twilio](https://www.twilio.com) and **sign up or log in**.
2. Verify your phone number via OTP.
3. Navigate to **Phone Numbers → Manage → Buy a Number**.
4. Choose and purchase a number using free trial credits.
5. Go to **Phone Numbers → Configure**:
   - Under **Voice Configuration**, update **"A call comes in"** URL with:
     ```
     https://api.us.elevenlabs.io/twilio/inbound_call
     ```
   - Save the configuration.

---

### ✅ Step 3: Connect Twilio to Eleven Labs

1. In Eleven Labs → Go to **Conversational AI** → Click **Phone Numbers**.
2. Click **Import Number** → Choose **Twilio**.
3. Provide a **label**, paste your **Twilio number**.
4. Go back to Twilio → Copy your **Account SID** and **Auth Token**.
5. Paste them into Eleven Labs and complete the integration.

---

### ✅ Step 4: Install MCP Dependencies

1. Open **Cursor IDE** terminal and run:
```
pip install elevenlabs-mcp
python -m elevenlabs_mcp --api-key={{paste your elevenlabs api key}} --print
```
2. Check Response: After running the command, you will get a response.
3. Set Up MCP Server in Cursor: Copy and paste the above JSON into the Cursor MCP JSON file. This will configure the server.

---

### ✅ Step 5: Create a Tech Update Agent

🤖 Agent Creation & Outbound Call <br>
🗣️ Prompt 1: Create the Tech Update Agent <br>
Paste this in the MCP chat panel: <br>
```
Create an agent that makes an outbound call to update someone about recent tech news
-> Use a confident, friendly tone — like a helpful colleague
-> Deliver updates about the latest in AI, programming, and cybersecurity
-> Keep the explanation short, clear, and jargon-free
-> Use my voice (female) for the call
-> The agent should sound like a tech-savvy friend, not a sales rep
-> First message: "Hey, I’ve got some quick tech updates for you — should I go ahead?"
You don’t have to make a call. Create an agent in the ElevenLabs simply
```
✅ This will create the agent in Eleven Labs.

📞 Prompt 2: Initiate a Call <br>
Paste this next: <br>
```
Now make an outbound call to {my number}.
```
It will ask for your number. A call will be triggered to your Twilio-verified number.
