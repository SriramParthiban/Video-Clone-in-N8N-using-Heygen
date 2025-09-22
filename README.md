## 🎥 AI Clone Video Generator (n8n + OpenAI + HeyGen)

This repository contains an **n8n workflow** that automatically generates **AI avatar videos** from chat inputs.  
It is designed for **creators, marketers, and businesses** who want to **turn ideas into short-form video content** instantly.

---

## 🚀 What It Does

**1. Chat Trigger**  
- Workflow starts when a **chat message** is received.  

**2. Transcript Creation**  
- Uses **OpenAI GPT models** to create a short, engaging transcript (45–60 sec).  
- Optimized for **YouTube Shorts, TikTok, or Instagram Reels**.  

**3. Catchy Title Generation**  
- AI suggests a **short, clean, and attention-grabbing title** for the video.  

**4. AI Video Generation (HeyGen)**  
- Sends the transcript to **HeyGen API**.  
- Uses a pre-selected **AI avatar** and **voice clone** to generate a realistic video.  

**5. Polling & Video Retrieval**  
- Workflow waits until the video is ready.  
- Once available, the video is automatically **downloaded**.  

---

## 🛠️ Tech Stack

- **n8n** (workflow automation)  
- **OpenAI GPT (gpt-4.1-mini)** for transcript & title generation  
- **HeyGen API** for AI avatar video creation  

---

## 📂 Workflow Overview

**When Chat Message Received → Transcript AI Agent → Title AI Agent → Generate Video → Wait → Get Video → Check If Ready → Download Video**

---

## 🔑 Requirements

- **OpenAI API Key**  
- **HeyGen API Key**  
- **n8n (self-hosted or cloud)**  

---

## ⚡ How to Use

**1.** Import the JSON workflow (`AI clone video Gen.json`) into your **n8n** instance.  
**2.** Configure credentials for:  
- **OpenAI**  
- **HeyGen (API Key)**  
**3.** Update the **avatar_id** and **voice_id** in the `Generate Video` node if you want different avatars/voices.  
**4.** Run the workflow → Send a chat input → Receive a **generated AI video**.  

---

## 📌 Example Flow

| **Input (Chat Message)**       | **Transcript Output**                        | **Title Output**          | **Video Link**   |
|--------------------------------|----------------------------------------------|---------------------------|------------------|
| "How AI saves hours daily"     | "AI can save you 5 hours a week by…"         | "Save 5 Hours with AI"    | [download.mp4]   |

---

## 🎯 Use Case

Perfect for:  
- **YouTube Shorts / TikTok / Instagram Reels creators**  
- **Businesses automating explainer content**  
- **Personal branding & fast content creation**  

---
