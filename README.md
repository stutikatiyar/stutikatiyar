<!-- HEADER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&color=0:FF1493,50:8A2BE2,100:FF8C00&height=230&section=header&text=Stuti%20Katiyar&fontSize=60&fontColor=FFFFFF&animation=fadeIn&fontAlignY=38&desc=AI%20%7C%20Speech%20%7C%20Computer%20Vision%20%7C%20Full-Stack&descAlignY=58&descSize=18" width="100%" alt="Stuti Katiyar banner" />
</p>

<!-- TYPING ANIMATION -->
<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=FF1493&center=true&vCenter=true&width=650&height=45&lines=AI+%2B+Speech+Recognition+Engineer;Computer+Vision+%2B+Deep+Learning;Full-Stack+AI+Systems+Builder;Currently+building+CapFlow+%2B+DermaLens" alt="Typing SVG" />
  </a>
</p>

<!-- BADGES -->
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=stutikatiyar&color=FF1493&style=for-the-badge&label=PROFILE+VIEWS" alt="Profile Views" />
  <img src="https://img.shields.io/github/followers/stutikatiyar?label=FOLLOWERS&style=for-the-badge&color=8A2BE2" alt="Followers" />
  <img src="https://img.shields.io/badge/Graduating-2027-FF8C00?style=for-the-badge" alt="Graduating 2027" />
</p>

<p align="center">
  <a href="mailto:stutikatiyarof@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://linkedin.com/in/stutikt"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://leetcode.com/STUTIKATIYAR"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
</p>

---

## 🌸 About Me

> **"Build robust pipelines. Validate before trusting."**

I'm an AI & ML undergraduate at **CMR Institute of Technology, Bengaluru**, building systems that bridge the gap between *"works in the lab"* and *"works in production"*, across noisy speech and messy visual data.

| | |
|---|---|
| 🚀 **Building** | **CapFlow**: a Hinglish code-switching captioning pipeline (`faster-whisper` + dynamic transliteration + Groq/Llama 3 post-processing) |
| 🔬 **Researching** | **DermaLens**: domain-aware AI middleware for dermatological image enhancement and quality assessment (Restormer, Real-ESRGAN) |
| 🌱 **Deep diving** | ASR, multilingual code-switching, speech separation, image restoration |
| 🤝 **Happy to chat about** | PyTorch, Whisper, Groq/LLM pipelines, OpenCV, FastAPI, React, noisy audio/visual signals |

### 🏆 Highlights

- 📜 Patent filed: Indian Patent App. No. `202641024127`
- 🥇 Finalist, **MSME IDEA Hackathon 4.0**
- 🎓 Student Placement Coordinator at CMRIT

---

## 💻 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,pytorch,js,ts,react,nextjs,fastapi,nodejs,express,mongodb,tailwind,opencv,docker,git,github,vscode" alt="Tech Stack" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Whisper-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
</p>

---

## 🚀 Featured Projects

<table>
  <tr>
    <td width="50%" valign="top">

### 🎙️ CapFlow
*Intelligent Code-Switching (Hinglish) Captioning Pipeline*

Turns mixed Hindi + English speech into production-ready **Romanized Hinglish** captions, with no phonetic degradation and no Devanagari lock-in.

- **ASR:** CTranslate2-optimized `faster-whisper-large-v3` with VAD pre-filtering and word-level timestamps
- **LLM correction:** multi-model failover layer on Groq (Llama 3.3 70B) for zero-shot loanword normalization
- **Export:** `.srt`, `.vtt` and structured `.json`

![Status](https://img.shields.io/badge/Status-Active%20Development-FF1493?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Speech%20%26%20NLP-8A2BE2?style=flat-square)
![Stack](https://img.shields.io/badge/Stack-Whisper%20%7C%20Groq%20%7C%20FastAPI-FF8C00?style=flat-square)

</td>
    <td width="50%" valign="top">

### 🧠🩺 DermaLens
*Domain-Aware AI Middleware for Dermatological Image Enhancement*

Adaptively corrects blur, noise and lighting defects in smartphone-captured skin images **before** downstream medical classification.

- **Core:** PyTorch, OpenCV, Restormer, Real-ESRGAN
- **Validation:** objective PSNR and SSIM evaluation built into the processing steps
- **Architecture:** FastAPI microservice with a clean React frontend

![Status](https://img.shields.io/badge/Status-Active%20Research-FF1493?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Medical%20CV-8A2BE2?style=flat-square)
![Stack](https://img.shields.io/badge/Stack-PyTorch%20%7C%20FastAPI%20%7C%20React-FF8C00?style=flat-square)

</td>
  </tr>
</table>

### 🔧 How they work

```mermaid
flowchart LR
    subgraph CapFlow
        A[Video / Audio] --> B[VAD filter]
        B --> C[faster-whisper large-v3]
        C --> D[Transliteration]
        D --> E[Groq Llama 3.3 70B correction]
        E --> F[SRT / VTT / JSON]
    end
```

```mermaid
flowchart LR
    subgraph DermaLens
        G[Smartphone skin image] --> H[Quality assessment]
        H --> I[Restormer / Real-ESRGAN]
        I --> J[PSNR + SSIM validation]
        J --> K[Downstream classifier]
    end
```

---

## 📈 Analytics & Activity

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=stutikatiyar&show_icons=true&theme=transparent&title_color=FF1493&text_color=808080&icon_color=8A2BE2&border_color=FF1493&hide_border=false" alt="GitHub stats" />
  <img height="170" src="https://streak-stats.demolab.com/?user=stutikatiyar&theme=transparent&ring=FF1493&fire=FF8C00&currStreakLabel=FF1493&currStreakNum=808080&sideNums=808080&sideLabels=808080&dates=808080&stroke=8A2BE2&border=FF1493" alt="GitHub streak" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=stutikatiyar&layout=compact&theme=transparent&title_color=FF1493&text_color=808080&border_color=FF1493" alt="Top languages" />
</p>

<p align="center">
  <img width="97%" src="https://github-readme-activity-graph.vercel.app/graph?username=stutikatiyar&theme=react-dark&bg_color=0D1117&hide_border=false&border_color=FF1493&line=FF1493&color=8A2BE2&point=FFFFFF&area=true" alt="Activity graph" />
</p>

<details>
<summary>🐍 Contribution snake</summary>
<br />
<p align="center">
  <img src="https://raw.githubusercontent.com/stutikatiyar/stutikatiyar/output/github-contribution-grid-snake-dark.svg" alt="Snake animation" />
</p>
</details>

---

## 🌐 Let's Connect

<p align="center">
  Open to <b>placements and off-campus roles</b> in AI/ML, speech and computer vision.<br /><br />
  <a href="mailto:stutikatiyarof@gmail.com">📧 Email</a> &nbsp;•&nbsp;
  <a href="https://linkedin.com/in/stutikt">💼 LinkedIn</a> &nbsp;•&nbsp;
  <a href="https://github.com/stutikatiyar">🐙 GitHub</a> &nbsp;•&nbsp;
  <a href="https://leetcode.com/STUTIKATIYAR">🧩 LeetCode</a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF1493,50:8A2BE2,100:FF8C00&height=120&section=footer" width="100%" alt="footer" />
