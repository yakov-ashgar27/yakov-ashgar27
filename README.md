<div align="center">

# Yakov Ashgar · יעקב אשגר

**Information Systems student (AI specialization) at the University of Haifa.<br>I turn a business need into a working, tested, deployed system, and I lead the people who build it.**

[![Portfolio](https://img.shields.io/badge/Portfolio-yakov--ashgar27.github.io-0f172a?style=for-the-badge&logo=githubpages&logoColor=white)](https://yakov-ashgar27.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Yakov%20Ashgar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yakov-ashgar-650271392)
[![Email](https://img.shields.io/badge/Email-ykhn563%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ykhn563@gmail.com)
[![Ask my AI](https://img.shields.io/badge/Ask%20yakov.LLM-about%20my%20code-7c3aed?style=for-the-badge&logo=openai&logoColor=white)](https://yakov-ashgar27.github.io/yakov.LLM/)

**9 complete projects** · **500+ automated tests** · **DFD + ERD for every data-driven system** · **5 live apps you can open right now**

</div>

---

## About me

- 🎓 Third-year **B.Sc. in Information Systems, AI specialization**, University of Haifa (graduating 2027–28).
- 🛠️ I work across the **whole lifecycle**: requirements and data model (user stories, DFD, ERD), architecture, code, tests, CI and a live deployment. Each data-driven project has its DFD and ERD next to the code.
- 📏 My projects report **measured results**, not just feature lists: detection rates, retrieval accuracy, statistical power, real-hardware validation.
- 🪖 Former **combat soldier and commander, Haruv Reconnaissance Unit**. Still on active reserve duty, with 5 deployments completed alongside my studies.

> 💡 **Short on time?** Ask [**yakov.LLM**](https://yakov-ashgar27.github.io/yakov.LLM/), an AI assistant I built that has read all my repositories. It answers questions about any project and cites the exact file and lines.

---

## ⭐ Featured projects

<table>
<tr>
<td width="42%" valign="top">
<a href="https://fitvision-ai-naoj.onrender.com"><img src="https://github.com/yakov-ashgar27/fitvision-ai/raw/main/diagrams/wireframes/screens-1-3-trainee.png" alt="FitVision AI: live rep counting and technique feedback" width="100%"></a>
</td>
<td valign="top">

### [🏋️ FitVision AI](https://github.com/yakov-ashgar27/fitvision-ai)
**Final degree project · team of 4 · my role: lead full-stack developer**

The phone camera tracks the trainee's skeleton, counts reps and corrects technique in real time. Trainers get analytic progress reports.

- Pose estimation runs **on the device** (Web Worker): video never reaches the server.
- Full spec: 20 user stories, DFD, ERD and a normalized **17-table** schema, RBAC.
- Offline-first sync via IndexedDB; **66 tests** in CI on **SQLite, PostgreSQL and SQL Server**.

`React PWA` `MediaPipe` `FastAPI` `SQL Server / PostgreSQL` `Redis + RQ`

**[▶ Live app](https://fitvision-ai-naoj.onrender.com)** · [📐 DFD & ERD](https://github.com/yakov-ashgar27/fitvision-ai/blob/main/docs/04-%D7%A0%D7%99%D7%AA%D7%95%D7%97-%D7%95%D7%AA%D7%9B%D7%9F.md) · [Code](https://github.com/yakov-ashgar27/fitvision-ai)

</td>
</tr>

<tr>
<td width="42%" valign="top">
<a href="https://github.com/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar"><img src="https://github.com/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar/raw/main/docs/img/demo-sunset.png" alt="FeatureLedger: Safe Sunset pipeline" width="100%"></a>
</td>
<td valign="top">

### [💰 FeatureLedger](https://github.com/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar)
**SaaS product · FinOps for product teams · solo**

Gives every product feature a monthly **profit & loss** statement (engineering effort from Git, support load, cloud and LLM spend against usage and ARR), then safely retires the features that lose money.

- **Token-Bleed Radar** finds AI features whose LLM costs eat their revenue.
- **Safe Sunset:** a guarded state machine that drives the feature flag, opens the dead-code PR itself and keeps a hash-chained audit log.
- Multi-tenant with **Postgres Row-Level Security**, OIDC SSO, RBAC; **170+ tests**; ledger checked to the cent in CI.

`FastAPI` `PostgreSQL 16 + pgvector` `Next.js 15` `Docker` `GitHub Actions`

**[▶ Run in 1 click (Codespaces)](https://codespaces.new/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar?quickstart=1)** · [📐 DFD & ERD](https://github.com/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/FeatureLedger-Feature-P-L-Safe-Deprecation-Radar)

</td>
</tr>

<tr>
<td width="42%" valign="top">
<a href="https://yakov-ashgar27.github.io/DocMind/"><img src="https://github.com/yakov-ashgar27/DocMind/raw/main/docs/screenshots/15_desktop_en.png" alt="DocMind assistant finding documents" width="100%"></a>
</td>
<td valign="top">

### [📂 DocMind](https://github.com/yakov-ashgar27/DocMind)
**Personal document assistant · web, Android and server · solo**

*"I need the documents for my reserve-duty benefits."* DocMind finds what you already have, remembers what each process requires, and helps you get what's missing.

- On-device **Hebrew/English OCR** and classification into 30 document types.
- Security by design: **AES-256-GCM** per-file keys, RSA-3072 PIN vault, two-step verification. Documents stay on your own phone or server.
- Phone and server editions share one knowledge base; CI proves they classify identically. **~80 tests**.

`Python` `FastAPI` `Tesseract OCR` `WebCrypto` `PWA` `Android`

**[▶ Open the app](https://yakov-ashgar27.github.io/DocMind/app/)** · [Android APK](https://yakov-ashgar27.github.io/DocMind/DocMind.apk) · [📐 DFD & ERD](https://github.com/yakov-ashgar27/DocMind/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/DocMind)

</td>
</tr>

<tr>
<td width="42%" valign="top">
<a href="https://yakov-ashgar27.github.io/PulsePort-Analytics/"><img src="https://github.com/yakov-ashgar27/PulsePort-Analytics/raw/main/docs/screenshots/ab-lab.png" alt="PulsePort A/B Testing Lab" width="100%"></a>
</td>
<td valign="top">

### [📊 PulsePort Analytics](https://github.com/yakov-ashgar27/PulsePort-Analytics)
**Product analytics & statistics · solo**

Funnels, A/B tests and AI-model evaluations on your own data, with the statistical test behind every claim and a clear **GO / NO-GO** verdict.

- Stops teams from shipping noise: flags a "+2.9% win" with p = 0.18 as **KEEP RUNNING** (63% power).
- Frequentist + Bayesian A/B, FDR control, segment-level drop-off detection.
- SciPy engine and an in-browser TypeScript port that agree in **22 parity test groups**. Data never leaves the browser.

`Python` `SciPy` `FastAPI` `PostgreSQL 16` `React` `TypeScript`

**[▶ Live app](https://yakov-ashgar27.github.io/PulsePort-Analytics/)** · [📐 DFD & ERD](https://github.com/yakov-ashgar27/PulsePort-Analytics/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/PulsePort-Analytics)

</td>
</tr>

<tr>
<td width="42%" valign="top">
<a href="https://yakov-ashgar27.github.io/yakov.LLM/"><img src="https://github.com/yakov-ashgar27/yakov.LLM/raw/main/docs/screenshot-home.png" alt="yakov.LLM home screen" width="100%"></a>
</td>
<td valign="top">

### [🤖 yakov.LLM](https://github.com/yakov-ashgar27/yakov.LLM)
**AI / retrieval-augmented generation · solo**

An AI assistant that has read every one of my repositories. Each answer cites the exact file and lines, and it re-indexes itself when I push.

- **BM25 search engine written from scratch**, with one tokenizer for both Hebrew and code.
- Fact cards generated from the code (via `ast`) for every function, class, route and table.
- Measured: the right file reaches the model for **89%** of test questions and **95% of 750** auto-generated ones. CI fails if accuracy drops.

`Python (zero dependencies)` `JavaScript` `LLM APIs` `SSE streaming` `GitHub Actions`

**[▶ Try it](https://yakov-ashgar27.github.io/yakov.LLM/)** · [📐 DFD & data model](https://github.com/yakov-ashgar27/yakov.LLM/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/yakov.LLM)

</td>
</tr>
</table>

---

## ⚡ Real-time systems & networking

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/yakov-ashgar27/wifi-doctor"><img src="https://github.com/yakov-ashgar27/wifi-doctor/raw/main/docs/dashboard.png" alt="WiFi-Doctor dashboard" width="100%"></a>

### [🩺 WiFi-Doctor](https://github.com/yakov-ashgar27/wifi-doctor)
Probes Wi-Fi, ISP and DNS every 1.5 s and names **which layer is failing**, with a confidence score and the fix. Adaptive z-score baselines per hop, Wi-Fi signal readings and a real bufferbloat test.

**Proof:** validated on a real laptop, all 4 fault types diagnosed; field testing caught 5 bugs CI missed. **65 tests**.

`Python` `asyncio` `NumPy` `FastAPI` `React` `Docker`

[Quick start](https://github.com/yakov-ashgar27/wifi-doctor#quickstart) · [📐 DFD & ERD](https://github.com/yakov-ashgar27/wifi-doctor/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/wifi-doctor)
</td>
<td width="50%" valign="top">
<a href="https://github.com/yakov-ashgar27/guardstream"><img src="https://github.com/yakov-ashgar27/guardstream/raw/main/docs/dashboard.jpg" alt="GuardStream SOC dashboard" width="100%"></a>

### [🛡️ GuardStream](https://github.com/yakov-ashgar27/guardstream)
Scores every card transaction as it arrives (**APPROVE / REVIEW / BLOCK**) with explainable business rules plus an Isolation Forest, and streams it to a live analyst dashboard.

**Proof:** flags **~98%** of simulated fraud with **~1.2%** false positives, in **~14 ms** per decision.

`FastAPI` `Redis Streams` `PostgreSQL` `scikit-learn` `React` `Docker`

[Quick start (1 command)](https://github.com/yakov-ashgar27/guardstream#quick-start) · [📐 DFD & ERD](https://github.com/yakov-ashgar27/guardstream/blob/main/docs/DIAGRAMS.md) · [Code](https://github.com/yakov-ashgar27/guardstream)
</td>
</tr>
</table>

## 🎮 Games

<table>
<tr>
<td width="50%" valign="top">
<a href="https://yakov-ashgar27.github.io/the-map-lies/"><img src="https://github.com/yakov-ashgar27/the-map-lies/raw/main/docs/screenshot.png" alt="The Map Lies gameplay" width="100%"></a>

### [🗺️ The Map Lies](https://github.com/yakov-ashgar27/the-map-lies)
A puzzle-stealth game where the minimap always lies. Seeded procedural levels, plus a validator that **proves every lie can be found without guessing**, checked on 500 generated levels.

`React 19` `TypeScript` `Vite` `PWA`

**[▶ Play](https://yakov-ashgar27.github.io/the-map-lies/)** · [Code](https://github.com/yakov-ashgar27/the-map-lies)
</td>
<td width="50%" valign="top">
<a href="https://github.com/yakov-ashgar27/Bomberman"><img src="https://github.com/yakov-ashgar27/Bomberman/raw/main/docs/images/architecture.png" alt="Bomberman architecture" width="100%"></a>

### [💣 Bomberman](https://github.com/yakov-ashgar27/Bomberman)
Software-engineering course project (team of 4): a full clone with BFS-chasing enemies, chain reactions and 5 levels, in Hebrew and English. Logic fully separated from the display. **84 tests**, ~95% logic coverage, plus SRS and presentation.

`Python` `Pygame` `pytest`

[Install & run](https://github.com/yakov-ashgar27/Bomberman#install--run) · [Code](https://github.com/yakov-ashgar27/Bomberman)
</td>
</tr>
</table>

---

## 🧭 How I work

| Principle | In practice |
|---|---|
| **Requirements first** | User stories, DFD, ERD and business rules that a team can build from. The diagrams are drawn from the real schema, so they match the code. |
| **Proof, not claims** | Projects report measured numbers against ground truth, and CI runs the tests on every push. |
| **Security & data by design** | Row-Level Security, RBAC, encryption at rest, data that stays on the device. |
| **Real-world testing** | I test on real hardware and real data, and feed what I find back into the code. |
| **Easy to try** | Every project is one step away: a live web app, a Codespace, a PWA, a Windows launcher or a single Docker command. |

## 🧰 Tech stack

**Languages:** Python · TypeScript · JavaScript · SQL<br>
**Backend:** FastAPI · asyncio · REST & WebSockets · Redis / Redis Streams · RQ / ARQ workers<br>
**Data & AI:** PostgreSQL · SQL Server · pgvector · SciPy · NumPy · scikit-learn · MediaPipe · LLM APIs / RAG · OCR<br>
**Frontend:** React · Next.js · Tailwind · PWA · Vite<br>
**DevOps & quality:** Docker · GitHub Actions CI · pytest · Codespaces · Render · GitHub Pages<br>
**Process:** Systems analysis · SDLC · Agile / Scrum · project leadership

---

<div align="center">

**Let's talk:** [ykhn563@gmail.com](mailto:ykhn563@gmail.com) · [LinkedIn](https://www.linkedin.com/in/yakov-ashgar-650271392) · [Portfolio](https://yakov-ashgar27.github.io/)

</div>
