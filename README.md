### Hi, I'm Yakov 👋

Information Systems student. I build complete products end to end: requirements and design documents, the code, tests, CI and a live deployment.

## Featured: WiFi-Doctor, network root cause analysis

<a href="https://github.com/yakov-ashgar27/wifi-doctor"><img src="https://github.com/yakov-ashgar27/wifi-doctor/raw/main/docs/dashboard.png" alt="WiFi-Doctor dashboard diagnosing bufferbloat" width="760"></a>

"The Internet is slow" can mean weak Wi-Fi, a saturated link, a congested ISP or a slow DNS server. WiFi-Doctor probes every layer of the path every 1.5 seconds and names the one that is failing, in plain English, with a confidence score and the fix.

- **Explainable RCA engine:** a deterministic decision tree over gateway, WAN and DNS latency, jitter and loss. It is combined with adaptive baselines (a robust median/MAD z-score per hop), so it catches degradations that are abnormal *for this network* even below the static thresholds.
- **Physical-layer evidence:** reads RSSI, band and channel from `netsh` (locale-tolerant, works on Hebrew Windows), `iw` and macOS, then cites them in the diagnosis: *"weak Wi-Fi signal (−78 dBm) on 2.4 GHz channel 6: switch to 5 GHz"*.
- **Active bufferbloat test:** an 8-second load test that compares loaded and unloaded latency and grades the connection A+ to F. It has a concurrency guard and a hard timeout.
- **Validated on a real laptop, not just in CI:** the test graded the home network **C** in 3 of 3 runs (+71 to +107 ms under load), and all four fault simulations were diagnosed correctly. Field testing found 5 bugs that 60+ unit tests missed; each is fixed and documented with a regression test.

**Stack:** Python 3.13 · FastAPI · WebSockets · asyncio · NumPy · scapy / ICMP / ping fallback chain · SQLite · React · TypeScript · Tailwind · Recharts · Docker · GitHub Actions

[**View the repo →**](https://github.com/yakov-ashgar27/wifi-doctor) · [**Release notes →**](https://github.com/yakov-ashgar27/wifi-doctor/releases/tag/v1.1.1)

## Featured: GuardStream, real-time fraud detection

<a href="https://github.com/yakov-ashgar27/guardstream"><img src="https://github.com/yakov-ashgar27/guardstream/raw/main/docs/dashboard.jpg" alt="GuardStream SOC dashboard" width="760"></a>

A streaming system that scores every card transaction as it arrives and decides APPROVE, REVIEW or BLOCK, with a live dashboard for fraud analysts.

- **Hybrid engine:** business rules over Redis sliding windows (velocity, impossible travel, high amount) plus an Isolation Forest, with a guard I added for its blind spot: values outside the training range.
- **Measured on the running stack:** about 98% of simulated fraud flagged, about 1.2% false positives, and an average of about 14 ms per decision.
- **Built like production:** Redis Streams consumer group with crash recovery, PostgreSQL audit trail for analyst decisions, CI on every push, and one-command setup with Docker Compose.

**Stack:** Python 3.13 · FastAPI · WebSockets · Redis Streams · PostgreSQL · scikit-learn · React · TypeScript · Tailwind · Recharts · Docker · GitHub Actions

[**View the repo →**](https://github.com/yakov-ashgar27/guardstream)

## More projects

| Project | What it is | Stack | Try it |
| --- | --- | --- | --- |
| [**FitVision AI**](https://github.com/yakov-ashgar27/fitvision-ai) | Final project. The phone camera tracks your skeleton, counts reps and corrects your technique in real time, and trainers get analytic reports. The video never leaves the device. | React PWA · TypeScript · MediaPipe (Web Worker) · FastAPI · SQLAlchemy · PostgreSQL / SQL Server · Redis + RQ · GitHub Actions | [Live app](https://fitvision-ai-naoj.onrender.com) |
| [**yakov.LLM**](https://github.com/yakov-ashgar27/yakov.LLM) | An AI assistant that has read all of my repos. Every answer cites the exact file and lines, and it re-indexes itself when I push. Search engine written from scratch (BM25, Hebrew + code tokenizer): the right file is in the top 5 for 87% of test questions. | Python (no dependencies) · JavaScript · LLM APIs (Groq, Claude) · SSE · GitHub Actions | [Try it](https://yakov-ashgar27.github.io/yakov.LLM/) |
| [**The Map Lies**](https://github.com/yakov-ashgar27/the-map-lies) | A puzzle-stealth game where the minimap always lies. Seeded procedural levels and a validator that proves every lie can be found without guessing. | React · TypeScript · Vite · PWA | [Play](https://yakov-ashgar27.github.io/the-map-lies/) |
| [**Bomberman**](https://github.com/yakov-ashgar27/Bomberman) | Software-engineering course project: a full Bomberman clone with a BFS-chasing enemy, chain reactions, 5 levels, Hebrew and English, plus SRS, presentation and work plan. | Python · Pygame · pytest (84 tests) | Run `python main.py` |

## What I focus on

- **Engineering beyond the code:** requirements (user stories, ERD, DFD), RBAC, migrations, offline sync, CI that tests on several databases, and real-device testing that feeds back into calibration.
- **Data and real-time systems:** streaming pipelines, explainable scoring that combines rules with ML, and metrics measured against ground truth instead of guessed.
- **Systems and networking:** active network probing with graceful privilege fallbacks, statistical anomaly detection, and testing on real hardware to find the bugs that CI can't.
- **Shipping:** each project can be opened or installed with one click, as a PWA, a Windows shortcut or a cloud deployment.
