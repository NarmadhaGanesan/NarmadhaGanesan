<!-- ════════════════════════════════  HEADER  ════════════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:6D28D9,100:A855F7&height=230&section=header&text=Narmadha%20Ganesan&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=I%20teach%20LLMs%20to%20read%20documents%2C%20compare%20contracts%20%26%20count%20their%20own%20cost&descAlignY=58&descSize=16" width="100%"/>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&duration=2600&pause=900&color=A855F7&center=true&vCenter=true&width=760&lines=%3E+messy+PDF+in%2C+clean+JSON+out.;%3E+two+documents+in%2C+one+honest+diff+out.;%3E+40%2B+models+priced%2C+audited+every+week.;%3E+one+API.+OpenAI+%E2%80%A2+Anthropic+%E2%80%A2+Gemini.;%3E+agents+that+know+when+to+hand+off+to+a+human." alt="Typing SVG"/>
</a>

<br/>

<a href="https://www.linkedin.com/in/narmadha-g-794015228"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
<a href="https://medium.com/@narmadhaganesan1"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white"/></a>
<a href="mailto:narmadhaganesan1@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
<img src="https://img.shields.io/badge/📍_Coimbatore,_India-1C1C1C?style=flat-square"/>
<img src="https://img.shields.io/badge/she%2Fher-A855F7?style=flat-square"/>
<img src="https://komarev.com/ghpvc/?username=NarmadhaGanesan&style=flat-square&color=A855F7&label=visitors"/>

</div>

<br/>

<!-- ════════════════════════════════  TERMINAL INTRO  ════════════════════════════════ -->
```console
narmadha@workhall:~$ whoami
Associate Software Engineer @ Workhall — building the AI layer of a no-code enterprise platform

narmadha@workhall:~$ cat ./day_job.txt
📄  Document extraction  — POs, invoices, PAN cards, MCA certificates, compliance docs
🤖  Agent Studio         — agent builder with tools, guardrails, KB/RAG & human handoff
🔀  Multi-provider LLMs  — one interface over OpenAI, Anthropic & Gemini
💸  Cost tracking        — knowing what every token costs, before finance asks

narmadha@workhall:~$ ./status --now
✔ shipping   ✔ benchmarking OCR models   ✔ writing on Medium
```

<!-- ════════════════════════════════  ASK THE MODEL  ════════════════════════════════ -->
## 🤖 &nbsp;If You Asked an LLM About Me…

```json
{
  "prompt": "Describe Narmadha in structured output. No hallucinations.",
  "response": {
    "superpower": "turning unstructured chaos into validated JSON",
    "favourite_question": "does retrieval actually make this answer better?",
    "pet_peeve": "a model that confidently invents a field that isn't in the document",
    "unpopular_opinion": "not every problem needs RAG",
    "off_screen": "on stage with a mic — hackathons, paper presentations, conferences",
    "confidence": 0.97
  },
  "usage": { "input_tokens": 42, "output_tokens": 108, "cost_usd": "tracked, obviously" }
}
```

<!-- ════════════════════════════════  HOW I THINK  ════════════════════════════════ -->
## 🧭 &nbsp;How I Build

Most AI demos stop at *"the model answered."* I care about what happens next — **is it right, is it cheap, and can someone trust it?**

```mermaid
flowchart LR
    A[📄 Raw input<br/>PDF · scan · web page] --> B[🔎 Read<br/>OCR · parsing · scraping]
    B --> C[🧠 Reason<br/>LLM · agents · RAG]
    C --> D[✅ Verify<br/>rules · validation · diffs]
    D --> E[📦 Ship<br/>FastAPI · MongoDB]
    E -. traces & cost .-> F[📈 Observe<br/>LangSmith · Grafana · ClickHouse]
    F -. feedback .-> C
    style C fill:#6D28D9,color:#fff,stroke:#A855F7
    style D fill:#1C1C1C,color:#fff,stroke:#A855F7
```

<!-- ════════════════════════════════  PROJECTS  ════════════════════════════════ -->
## 🚀 &nbsp;Featured Projects

<table>
<tr>
<td width="33%" valign="top">

### 🔍 ContextIQ
**AI document comparator**

Upload two documents — PDF, DOCX, CSV, Markdown or an image — and get a summary, similarity score, categorised differences and a recommendation.

**Under the hood:** a 3-layer pipeline
1. deterministic diff (`redlines`)
2. TF-IDF semantic alignment
3. LLM interpretation

`FastAPI` `Python` `LLMs`

</td>
<td width="33%" valign="top">

### 💸 LLM Cost Tracker
**Know what every token costs**

Monitors and visualises API usage and spend across OpenAI, Anthropic and Gemini.

Backed by a pricing audit of **40+ models** — refreshed weekly, and it has already caught a 10× cached-price understatement.

`Python` `FastAPI` `MongoDB`

</td>
<td width="33%" valign="top">

### 🌐 Automating Web Intel
**AI-powered web intelligence**

A fully asynchronous service that searches, scrapes and structures web data in real time, built to scale with batch processing.

`FastAPI` `Tavily API` `AsyncIO` `MongoDB`

</td>
</tr>
</table>

<details>
<summary><b>🧪 More from the lab — click to expand</b></summary>
<br/>

| Experiment | What I did |
|---|---|
| **OCR shoot-out** | Benchmarked Baidu Unlimited-OCR vs Azure Document Intelligence vs Mistral OCR; built a reusable `UnlimitedOCRClient` |
| **PO extraction eval** | Two-step (Mistral OCR → GPT-4.1) vs single-step vision models, with field-by-field accuracy scoring and cost calculators |
| **`reasoning_effort` everywhere** | One provider-agnostic enum mapped onto each vendor's thinking controls, incl. Gemini's `thinking_budget` |
| **Agent guardrails** | A guardrail config schema: scope, blocked categories, regex rules, redact / escalate / log-only actions |
| **Multi-Agent ChatBot** | Stateful LangGraph agents with tools, memory and RAG |
| **Excel-driven tests** | pytest parametrised straight from spreadsheets via `openpyxl` |

</details>

<!-- ════════════════════════════════  TECH STACK  ════════════════════════════════ -->
## 🧰 &nbsp;Toolbox

<div align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/LangSmith-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
<br/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/Anthropic-D97757?style=for-the-badge&logo=anthropic&logoColor=white"/>
<img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white"/>
<img src="https://img.shields.io/badge/Mistral_OCR-FA520F?style=for-the-badge&logo=mistralai&logoColor=white"/>
<img src="https://img.shields.io/badge/Tavily-0F172A?style=for-the-badge&logoColor=white"/>
<br/>
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
<img src="https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge&logo=clickhouse&logoColor=black"/>
<img src="https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white"/>
<img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black"/>

</div>

<!-- ════════════════════════════════  JOURNEY  ════════════════════════════════ -->
## 🛤️ &nbsp;The Journey So Far

```text
2021 ──●── B.E. Computer Science · Bannari Amman Institute of Technology
       │     🏆 BITSHACK '22 winner   🏆 Code-GitFest '22 winner
       │     🎤 Jury Choice Award — Driver Drowsiness Detection
       │     📜 Patent filed — "ODOR ALERT: Everyday Citizens' Abetment"
       │     🎙️ Hosted national conference Impellz '23 · trained 50+ students
       │
2024 ──●── ML Engineer Trainee @ Workhall
       │     first agentic workflows wired into business automation
       │
2025 ──●── Associate Software Engineer @ Workhall · graduated, CGPA 8.52
       │     extraction pipelines · FastAPI services · LangSmith tracing
       │
2026 ──●── Agent Studio · ContextIQ · LLM Cost Tracker · Web Intel
       │     ✍️ "Rethinking RAG: When Retrieval Helps and When It Hurts"
       │
  now ─◉── 🔁 still learning, still shipping — see you in the commits
```

<!-- ════════════════════════════════  WRITING  ════════════════════════════════ -->
## ✍️ &nbsp;Latest from My Medium

<!-- BLOG-POST-LIST:START -->
- [Rethinking RAG: When Retrieval Helps and When It Hurts](https://medium.com/@narmadhaganesan1)
<!-- BLOG-POST-LIST:END -->

<sub>↻ auto-updated from my Medium feed</sub>

<!-- ════════════════════════════════  STATS  ════════════════════════════════ -->
## 📊 &nbsp;On GitHub

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=NarmadhaGanesan&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0D1117&title_color=A855F7&icon_color=A855F7"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=NarmadhaGanesan&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=A855F7"/>

<img src="https://streak-stats.demolab.com?user=NarmadhaGanesan&theme=tokyonight&hide_border=true&background=0D1117&ring=A855F7&fire=A855F7&currStreakLabel=A855F7" width="55%"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=NarmadhaGanesan&bg_color=0D1117&color=C4B5FD&line=A855F7&point=FFFFFF&area=true&hide_border=true" width="100%"/>

<img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" width="70%"/>

</div>

<!-- ════════════════════════════════  CONNECT  ════════════════════════════════ -->
## 🤝 &nbsp;Let's Talk

<div align="center">

**Document AI · agent design · RAG trade-offs · LLM pricing rabbit holes** — I'm always up for these conversations.

<a href="https://www.linkedin.com/in/narmadha-g-794015228"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="https://medium.com/@narmadhaganesan1"><img src="https://img.shields.io/badge/Read_my_writing-000000?style=for-the-badge&logo=medium&logoColor=white"/></a>

<sub><i>intelligent + resilient + performant — and always explainable.</i></sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:A855F7,50:6D28D9,100:0D1117&height=120&section=footer" width="100%"/>
