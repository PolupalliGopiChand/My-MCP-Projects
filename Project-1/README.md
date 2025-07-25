# 🚀 Project-1: LinkedIn Post Creation with Image

This project demonstrates how to create a LinkedIn post (including an image) using an MCP server connected through Cursor IDE.

---

## 🛠️ Prerequisites

### ✅ LinkedIn MCP Server via Pipedream
- Set up a LinkedIn MCP server on [Pipedream](https://pipedream.com).
- Authenticate your LinkedIn account.

📺 **Installation Guide:**  
Watch the full step-by-step tutorial here: [YouTube Tutorial](https://youtu.be/4Zz-vqP3nvM?si=UA9AcBlx7Kx_yI0y)

### ✅ Cursor IDE
- Install and open **Cursor IDE**.
- Be familiar with the **MCP tab** in the interface.

---

## ⚙️ Process

### 📌 Step 1: Set Up LinkedIn MCP Server
- Go to [Pipedream](https://pipedream.com) and create a new LinkedIn MCP server.
- Click on **Authenticate** to connect your LinkedIn account.

---

### 📌 Step 2: Paste the MCP Server URL in Cursor IDE
- Open Cursor IDE and click on the **MCP tab**.
- Paste the MCP Server URL obtained from Pipedream into the designated input field.

---

### 📌 Step 3: Post Content

#### ✏️ Post Text
> text your post description and add tags for the post

#### 🖼️ Image URL
> upload your own image via Cloudinary for the post:  

##### How to Upload to Cloudinary:
1. **Create a Cloudinary Account:** [cloudinary.com](https://cloudinary.com)
2. **Upload Your Image:**
   - Navigate to the **Assets tab** → **Assets Home**.
   - Click **Upload** (top-right) and select your image.
3. **Get Image URL:**
   - Go to **Assets** → **Folders**.
   - Right-click on the uploaded image → **Copy URL** → Click **Original** for the direct link.

---

### 📌 Step 4: Prepare Post Prompt in Cursor IDE
Open the **MCP chat panel** and write your prompt:

```
Create an image post on LinkedIn with the following text:
{Your post text}
Image link: {Image link}
```
---

### 📌 Step 5: Send Prompt to MCP
- Hit **Enter** to submit your prompt.
- The MCP server will generate and publish your LinkedIn post.
- If additional information is requested, reply directly in the chat panel.

---

### 📌 Step 6: Verify Your LinkedIn Post
- Go to your LinkedIn profile or company page.
- 🎉 **You’ll see your post successfully created and live!**

---

## ✅ Outcome
A fully automated and AI-assisted LinkedIn post, created with:
- Authentic LinkedIn account integration
- Real-time prompt generation
- Custom image upload and use
