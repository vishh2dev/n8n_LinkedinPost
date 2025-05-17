# 🧠 Free Automated LinkedIn AI Digest Workflow (n8n)

This is a 100% **free, no-code AI workflow** built with [n8n](https://n8n.io/) that automatically creates and posts a weekly AI digest to your personal LinkedIn profile.

It fetches the latest AI news, summarises the most relevant stories for small business owners using free AI models, and optionally sends the draft for approval via email before publishing to LinkedIn.

---

## 🎯 Use Case

Help busy SMB founders and marketers stay updated on the most impactful AI news — **automatically**. This workflow:
- 🧠 Picks the top 2 stories from a trusted AI RSS feed
- ✍️ Writes engaging LinkedIn-ready content
- ✅ Sends it to your inbox for approval (with a simple form)
- 📤 Posts it directly to your personal LinkedIn account

> Best part? It's fully free — no OpenAI credits, no Zapier fees, no paid n8n plan required.

---

## 🔥 Highlights

- ⚙️ 100% no-code (built entirely with n8n)
- 🆓 Uses **free Groq-hosted LLaMA 3 70B** for AI summarization
- ✅ Includes optional **approval workflow via Gmail**
- 🧑‍💼 Posts directly to **your personal LinkedIn profile**
- 📄 Completely customizable to your writing style

---

## 📦 What's Inside

| Feature                      | Tool/Service       | Free? |
|-----------------------------|--------------------|-------|
| AI Summarization            | Groq               | ✅ Yes |
| Workflow Orchestration      | n8n                | ✅ Yes |
| Email Approval Flow         | Gmail OAuth        | ✅ Yes |
| Social Media Posting        | LinkedIn API       | ✅ Yes |
| Custom Style Prompting      | LangChain          | ✅ Yes |

---

## 🛠️ Setup Instructions

### 1. Prerequisites

You need free accounts for:
- [n8n](https://n8n.io/)
- [Groq](https://console.groq.com/)
- [LinkedIn Developer Portal](https://www.linkedin.com/developers/)
- [Google Cloud Console](https://console.cloud.google.com/) (for Gmail API setup)

---

### 2. Add Required Credentials in n8n

| Credential         | Description                            |
|--------------------|----------------------------------------|
| **Groq API Key**   | For LLaMA 3 70B-powered text generation |
| **LinkedIn OAuth2**| For posting to your personal profile   |
| **Gmail OAuth2**   | For approval form email                |

---

### 3. Import Workflow

1. Open your **n8n** dashboard.
2. Go to **Workflows → Import**.
3. Upload the `Linkedin_post.json` file provided.

---

### 4. Customize It

- 🧑‍🎤 **Writing Style**: Modify the "Writing style" node to reflect your tone or voice.
- ✉️ **Approval Email**: Update the email address in the Gmail node.
- 🧑‍💼 **LinkedIn Profile**: Confirm your `person` ID is set correctly in the final LinkedIn node.

---

## 📤 Example Output

> **Here is everything that happened in AI this week**  
> AI is transforming industries. Here’s what SMBs need to know.  
>  
> 🔹 *Startup Raises $100M to Simplify AI Integration*  
> Why it matters: Affordable AI tools could now be within reach for small businesses.  
> 👉 [Read more](https://...)  
>  
> 🔹 *New AI Tool Improves SEO by 300%*  
> Why it matters: Use AI to boost organic traffic and leads.  
> 👉 [Read more](https://...)

---

## 🖼️ Approval Flow

You’ll receive an email with:
- A dropdown: ✅ “Yes” / ❌ “No – I’ll add change requests”
- A textarea for edits (if needed)

Once approved, the post is auto-published to LinkedIn.

---

## ✅ Tech Stack

- n8n (Open Source Automation)
- LangChain (Free LLM workflow layer)
- Groq API (Free access to LLaMA 3 70B)
- Gmail API
- LinkedIn API

---



### ⭐ Bonus Tip

You can host n8n for free on [Render](https://render.com), [Fly.io](https://fly.io), or [Railway](https://railway.app) to keep this running 24/7 for $0/month.


