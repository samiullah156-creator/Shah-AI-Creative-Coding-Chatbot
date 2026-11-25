<!-- styled:v2 -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1d1726,50:167dfe,100:9533fa&height=180&section=header&text=Shah%20AI%3A%20Creative%20Coding%20Chatbot&fontSize=31&fontColor=ffffff&fontAlignY=36&desc=React%20%E2%80%A2%20TypeScript%20%E2%80%A2%20Gemini&descAlignY=58&descSize=16&animation=fadeIn" width="100%" alt="Shah AI: Creative Coding Chatbot" />

**A multimodal Gemini chatbot that turns ideas, images, documents and voice into step-by-step solutions, visual explanations and working micro-app prototypes.**

<p>
  <img src="https://img.shields.io/badge/React%2019-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Gemini%20API-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" alt="Gemini" />
  <img src="https://img.shields.io/badge/Framer%20Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white" alt="Framer Motion" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
</p>

<p>
  <a href="#overview">Overview</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#features">Features</a> ·
  <a href="#tech-stack">Tech stack</a> ·
  <a href="#project-structure">Project structure</a> ·
  <a href="#getting-started">Getting started</a>
</p>

</div>

---

## Overview

Shah AI accepts text, voice, images, documents or a camera feed, works out the problem and answers with a structured solution, an interactive visual and, in Magic Build mode, a small working app you can try straight away. A calm 3D background and accessibility options keep long sessions comfortable.

## Features

| Mode | What it does |
|:--|:--|
| ✨ **Magic Build** | Builds a functional micro-app prototype from a plain-language idea |
| 🌍 **Global Impact** | Breaks down large real-world problems with diagrams and an action roadmap |
| 🎓 **Educator** | Explains a concept at three levels of difficulty with visual aids |
| ♿ **Accessible** | Voice-first interaction, high-contrast and dyslexia-friendly layout |

- Multimodal input: text, voice, image, document and camera
- Spoken answers with Gemini text-to-speech
- Image generation (Imagen) and short video generation (Veo)
- Insight panel with exportable outputs such as code snippets and scripts
- 3D animated background with soft parallax (Framer Motion)

## How it works

```mermaid
flowchart LR
    I([Text / voice /<br/>image / file]) --> M{Selected mode}
    M --> G[Gemini 2.5 Flash<br/>reasoning]
    G --> O1[Step-by-step<br/>answer]
    G --> O2[Visuals<br/>Imagen / Veo]
    G --> O3[Micro-app<br/>prototype]
    O1 --> T([Read aloud<br/>with TTS])

    classDef box fill:#1d1726,stroke:#167dfe,color:#e5e7eb
    classDef ends fill:#2e1065,stroke:#9533fa,color:#ffffff
    class M,G,O1,O2,O3 box
    class I,T ends
```

## Tech stack

| Area | Tools |
|:--|:--|
| Frontend | React 19, TypeScript, Vite, Framer Motion |
| AI | Google Gen AI SDK: `gemini-2.5-flash`, `gemini-2.5-flash-preview-tts`, Imagen 3, Veo 3.1 |

## Project structure

```
├── App.tsx
├── components/   # Background3D, ChatArea, InsightPanel, Sidebar
├── services/     # geminiService.ts (chat, TTS, image and video calls)
└── types.ts      # Modes and message types
```

## Getting started

```bash
npm install
echo "GEMINI_API_KEY=your_key" > .env.local
npm run dev
```

---

<div align="center">

**Built by [Ch Muhammad Samiullah](https://github.com/samiullah156-creator)** · AI Automation Engineer and Full-Stack Developer at [Lexvaxa](https://lexvaxa.com)

<a href="https://github.com/samiullah156-creator"><img src="https://img.shields.io/badge/More%20projects-181717?style=for-the-badge&logo=github&logoColor=white" alt="More projects" /></a>
<a href="https://lexvaxa.com/contact"><img src="https://img.shields.io/badge/Work%20with%20me-167dfe?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Work with me" /></a>
<a href="https://www.linkedin.com/in/sami-lexvaxa/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

<sub>⭐ Star this repo if you found it useful</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:9533fa,50:167dfe,100:1d1726&height=110&section=footer" width="100%" alt="" />
