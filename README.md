### Hi, I'm Yakov 👋

Information Systems student. I build complete products end to end: requirements and design documents, the code, tests, CI and a live deployment.

Every project below has automated tests, CI on every push and a one-click way to run it. Each one also has a measured result rather than just a feature list.

## Projects

| Project | What it does | Proof | Stack | Try it |
| --- | --- | --- | --- | --- |
| [**PulsePort Analytics**](https://github.com/yakov-ashgar27/PulsePort-Analytics) | Analyses funnels, A/B tests and AI-model evaluations on your own data, shows the statistical test behind every claim, and gives a clear GO / NO-GO verdict. | Flags a "+2.9% win" with p = 0.18 as KEEP RUNNING (63% power). Its SciPy engine and in-browser TypeScript port agree in 22 parity test groups. About 80 tests. | Python · FastAPI · SciPy · PostgreSQL 16 · React · TypeScript | [Live app](https://yakov-ashgar27.github.io/PulsePort-Analytics/) |
| [**WiFi-Doctor**](https://github.com/yakov-ashgar27/wifi-doctor) | Probes Wi-Fi, ISP and DNS every 1.5 s, names the layer that is failing, and gives a confidence score and the fix. It uses adaptive z-score baselines, reads the Wi-Fi signal and channel, and runs an active bufferbloat test. | Validated on a real laptop: bufferbloat grade C in 3 of 3 runs and all 4 fault types diagnosed. Field testing found 5 bugs that CI missed. 65 tests. | Python · FastAPI · asyncio · NumPy · React · TypeScript · Docker | [One-click Windows launcher](https://github.com/yakov-ashgar27/wifi-doctor#quickstart) |
| [**GuardStream**](https://github.com/yakov-ashgar27/guardstream) | Scores every card transaction as it arrives (APPROVE, REVIEW or BLOCK) with business rules plus an Isolation Forest, and gives analysts a live dashboard. | Flags about 98% of simulated fraud with about 1.2% false positives, in about 14 ms per decision. | FastAPI · Redis Streams · PostgreSQL · scikit-learn · React · Docker | [Run locally: 1 Docker command](https://github.com/yakov-ashgar27/guardstream#quick-start) |
| [**FitVision AI**](https://github.com/yakov-ashgar27/fitvision-ai) | Final project. The phone camera tracks your skeleton, counts reps and corrects your technique in real time, and trainers get analytic reports. | The video never leaves the device: pose estimation runs in a Web Worker. | React PWA · MediaPipe · FastAPI · PostgreSQL / SQL Server · Redis + RQ | [Live app](https://fitvision-ai-naoj.onrender.com) |
| [**yakov.LLM**](https://github.com/yakov-ashgar27/yakov.LLM) | An AI assistant that has read all of my repos. Every answer cites the exact file and lines; it reads attached files too, remembers returning visitors, and re-indexes itself when I push. | A search engine written from scratch (BM25, Hebrew + code tokenizer) plus fact cards generated from the code for every function and file: the right file reaches the model for 89% of test questions and 95% of 750 auto-generated ones. | Python (no dependencies) · JavaScript · LLM APIs · SSE | [Try it](https://yakov-ashgar27.github.io/yakov.LLM/) |
| [**The Map Lies**](https://github.com/yakov-ashgar27/the-map-lies) | A puzzle-stealth game where the minimap always lies. | Seeded procedural levels, plus a validator that proves every lie can be found without guessing. | React · TypeScript · Vite · PWA | [Play](https://yakov-ashgar27.github.io/the-map-lies/) |
| [**Bomberman**](https://github.com/yakov-ashgar27/Bomberman) | Software-engineering course project: a full Bomberman clone with a BFS-chasing enemy, chain reactions and 5 levels, in Hebrew and English. | 84 tests, plus SRS, presentation and work plan. | Python · Pygame · pytest | [Run locally](https://github.com/yakov-ashgar27/Bomberman#install--run) |

<table>
  <tr>
    <td align="center"><a href="https://yakov-ashgar27.github.io/PulsePort-Analytics/"><img src="https://github.com/yakov-ashgar27/PulsePort-Analytics/raw/main/docs/screenshots/ab-lab.png" alt="PulsePort A/B Testing Lab" width="260"></a><br><sub>PulsePort: A/B Testing Lab</sub></td>
    <td align="center"><a href="https://github.com/yakov-ashgar27/wifi-doctor"><img src="https://github.com/yakov-ashgar27/wifi-doctor/raw/main/docs/dashboard.png" alt="WiFi-Doctor dashboard" width="260"></a><br><sub>WiFi-Doctor: live RCA dashboard</sub></td>
    <td align="center"><a href="https://github.com/yakov-ashgar27/guardstream"><img src="https://github.com/yakov-ashgar27/guardstream/raw/main/docs/dashboard.jpg" alt="GuardStream SOC dashboard" width="260"></a><br><sub>GuardStream: fraud SOC dashboard</sub></td>
  </tr>
</table>

## What I focus on

- **Engineering beyond the code:** requirements (user stories, ERD, DFD), RBAC, migrations, offline sync, CI that tests on several databases, and real-device testing that feeds back into calibration.
- **Data and real-time systems:** streaming pipelines, explainable scoring that combines rules with ML, statistics you can trust, and metrics measured against ground truth instead of guessed.
- **Systems and networking:** active network probing with graceful privilege fallbacks, statistical anomaly detection, and testing on real hardware to find the bugs that CI can't.
- **Shipping:** each project can be opened or installed with one click, as a PWA, a Windows launcher or a cloud deployment.
