# 🚀 VertexAlpha 🔺📈

<img width="1387" height="891" alt="Screenshot 2025-11-18 210708" src="https://github.com/user-attachments/assets/e8344be5-2bc3-4001-b4b5-290a66d4d3ac" />

Smarter, AI powered investing for everyone.  
VertexAlpha brings **Google Gemini** to the world of investing, turning it into your personal **AI–powered portfolio copilot**. ✨🤖💼

This project blends a silky smooth landing page with an **in page financial advisor chatbot** that:
- Speaks Markdown 📝
- Explains trade offs like a real advisor ⚖️  
- Guides your investment decisions in real time 📊  
- Looks way too clean for a hackathon project 😎🔥  

---

## ✨ What is VertexAlpha? 💡

VertexAlpha is a next generation **robo-advisor demo experience** 🎯.

It shows how a cutting edge LLM like **Gemini** can sit atop a real world investment flow and feel like a polished fintech product.  
The landing page walks users through the value, the chatbot gives personalized guidance, and the entire UX feels cohesive, modern, and fun 🌈⚡

This is not another “AI playground” —  
**It feels like a product.** 🏆

---

## 💼 Product Story 📚❤️

Modern investors want advice that is:
- Smart 🧠  
- Personalized 🎯  
- Easy to understand 💬  

Most tools fail by being either way too simple or unnecessarily complex. VertexAlpha fills that gap by marrying beautiful UX with conversational intelligence.

The project focuses on:
- **High quality product copy** ✍️  
- **Smooth animations** 🎞️  
- **A helpful AI advisor** that talks like a real human 🌟  

The result is a fintech prototype your judges will *definitely* think is a real product 🚀🔥

---

## 🧠 Core Features 🌟

### 1. 🎨 Stunning Marketing Grade Landing Page

- Bold hero banner with strong branding 💥  
- Clean typographic hierarchy ✨  
- Mobile responsive (because professionalism matters) 📱  
- Red accent theme for consistent brand identity ❤️🟥  

### 2. 💡 Intelligent Investment Solutions

Three core product cards:

- 📊 **Data Driven Insights**  
  Advanced algorithms analyze market trends for smarter decisions.

- 🛡️ **Risk Management**  
  Modern protection tools built for volatile markets.

- 🎯 **Portfolio Optimization**  
  Automated rebalancing keeps your portfolio aligned with your goals.

### 3. 🧭 How VertexAlpha Works

A simple 3-step journey:

1. 🔍 **Define Your Goals**  
   Share preferences, timeline, and risk tolerance.

2. ⚙️ **AI Portfolio Creation**  
   Gemini designs a tailored, diversified portfolio.

3. 🔄 **Automated Management**  
   Continuous monitoring + adjustments for optimal performance.

### 4. 🤖 Embedded AI Financial Advisor Chatbot

- Floating chat bubble 💬✨  
- Animations powered by Framer Motion ⚡  
- Uses Markdown for beautiful structured responses 📝  
- Three dot loading animation (the vibes matter) 🔴🔴🔴  
- Helps with:
  - Investment strategies  
  - Retirement planning  
  - Risk assessment  
  - Portfolio optimization  
  …all in a friendly, natural tone 😄

### 5. 🔮 Google Gemini Integration

- Powered by `gemini-2.5-flash` ⚡  
- System prompt crafted for clear financial guidance 🧭  
- Responses are always structured, clean, and useful 📐  
- Model remembers context for full conversation threads 💬🔁  

---

## 🏗 Tech Stack 🧰⚙️

- **Framework:** Next.js + React  
- **Styling:** Tailwind CSS ✨  
- **Animation:** Framer Motion 🎞️  
- **AI Engine:** Google Gemini 🧠🔮  
- **Icons:** lucide-react  
- **Markdown Rendering:** `react-markdown`  

Fast. Clean. Modern. Hackathon optimized 🏎️💨

---

## 🔌 Gemini API Usage 🤝⚡

The chatbot calls Gemini using a simple REST endpoint.

```ts
const GEMINI_API_KEY = "YOUR_API_KEY"

const response = await fetch(
  "https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=" + GEMINI_API_KEY,
  {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({
      contents,
      generationConfig: {
        temperature: 0.7,
        maxOutputTokens: 500,
      },
    }),
  }
)
