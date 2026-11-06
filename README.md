<h1 align="center">Hi, I'm Prafull Narang 👋</h1>

<p align="center">
  <b>MCA @ NIT Warangal (2024–2027)</b> · I build distributed backends, GenAI/RAG systems and fast multi-threaded C++.<br/>
  Open to <b>SDE · Backend · ML/GenAI Engineer</b> roles (full-time, 2027 batch).
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/prafull-narang-02a61b247"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:prafullnarang03@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://leetcode.com/u/wGm6kK22FK/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>
</p>

---

### ⚡ At a glance

- 🔬 **Research Intern, NIT Warangal**: statistical model checking of COVID-19 spread on 670K+ real cases
- 🏗️ Built a **real-time collaborative code editor**: 600/600 sandboxed runs at 200 runs/min, p95 **240 ms**, 86 tests, deployed on Azure
- 🚀 Wrote a **C++17 telemetry agent** that processes **~2.7 M samples/s** with zero loss, verified under TSan/ASan/UBSan
- 🛡️ Built an **ML-based DDoS filter** for IoT that blocks floods in **1.6 s** with **99.8%** accuracy
- 🏆 **AIR 1956** in NIMCET 2024 · **124+** LeetCode problems solved

---

### 🛠️ Featured projects

#### 🟦 [CodeSync: Real-time Collaborative Code Editor](https://github.com/prafullf/codesync)
Several people edit one file with live cursors. Anyone can hit **Run**, and the code runs in a fresh, network-less Docker sandbox while everyone in the room sees the output.

<img src="https://raw.githubusercontent.com/prafullf/codesync/main/docs/demo.gif" alt="CodeSync demo: two users edit and run code together" width="640"/>

- Conflict-free editing with a **Yjs CRDT** over WebSockets; works offline and syncs on reconnect
- Execution pipeline: **Fastify → BullMQ (Redis) → 3 stateless workers → isolated container** (128 MB RAM, 0.5 CPU, 5 s limit) for Python, JS and C++
- k6 load tests: **600/600 runs** at 200 runs/min, **0% HTTP errors**, enqueue p95 **16 ms**
- Hardened API: JWT auth, owner/editor/viewer roles, hand-written Redis sliding-window rate limiter
- **86 tests** (sandbox tests use real Docker), Playwright two-user E2E, GitHub Actions CI

`TypeScript` `React` `Yjs` `Fastify` `Socket.IO` `Redis` `BullMQ` `PostgreSQL` `Prisma` `Docker` `Azure`

#### 🤖 [RAG-based Document Q&A Assistant](https://github.com/prafullf/rag-document-qa)
Ask questions about your own PDFs and notes. Answers come **only** from retrieved passages and carry numbered citations to file and page.

- Chunking + Gemini embeddings indexed in **PostgreSQL pgvector**, with top-k cosine search
- **Hallucination guards:** a relevance gate skips the LLM call when nothing relevant is found, plus a strict citation-only prompt
- Content-hash chunk IDs, so re-uploading a file never duplicates chunks; covered by pytest tests

`Python` `LangChain` `Gemini API` `pgvector` `Streamlit` `Docker`

#### ⚙️ [Optical Transceiver Telemetry & Alarm Agent](https://github.com/prafullf/optical-telemetry-agent)
A multi-threaded **C++17** agent that polls optical-port telemetry (Rx/Tx power, OSNR, pre-FEC BER, temperature) and raises alarms the way real network gear does, with hysteresis, debouncing and root-cause masking.

- **~2.7 M samples/s** with zero loss; capture-to-decision latency p50 **30 µs**, p99 **289 µs**
- Port-affinity sharding means **lock-free per-port state**; bounded queues give back-pressure
- A trend detector warns **12–26 samples before** a threshold alarm fires
- 29 GoogleTest + 6 end-to-end tests; CI runs under **ThreadSanitizer, AddressSanitizer and UBSan**

`C++17` `Multithreading` `CMake` `GoogleTest` `GitHub Actions`

#### 🛡️ [ML-based DDoS Detection for IoT using SDN](https://github.com/prafullf/ml-ddos-detection-iot-sdn)
A Random Forest inside a Ryu SDN controller classifies every IoT flow each second and installs OpenFlow drop rules for attacks.

- **99.8% accuracy** from 9 engineered per-flow features; compared 4 ML models on 25K+ samples
- False positives cut from **2.7% → 0.1%** (F1 0.67 → 0.98) compared with a static threshold
- **99.5%** legitimate traffic delivered under attack (73.9% unprotected); blocked 4/4 attacks in **1.6 s**

`Python` `scikit-learn` `Ryu` `Mininet` `Open vSwitch` `Docker`

#### 📊 [COVID-19 Statistical Model Checking: NIT Warangal Research Internship](https://github.com/prafullf/covid19-smc-telangana)
- Agent-based SIR Monte Carlo model built on **609 days** of Telangana data (670K+ cases)
- Chernoff–Hoeffding bound → **737 runs** for ±0.05 accuracy at 95% confidence
- Found that only faster recovery (vaccination) lowered outbreak probability: **0.998 → 0.936**

`Python` `NumPy` `Pandas` `Monte Carlo` `Statistical Model Checking`

---

### 🧰 Tech stack

**Languages:** ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)

**Backend:** ![Fastify](https://img.shields.io/badge/Fastify-000000?logo=fastify&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB) ![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?logo=socketdotio&logoColor=white)

**AI / ML:** ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?logo=langchain&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)

**Data & infra:** ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?logo=microsoftazure&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)

---

### 🌱 Right now

- 📚 Final-year MCA at NIT Warangal, graduating 2027
- 🧠 Practicing DSA daily in C++ and going deeper into LLM evaluation and system design
- 📫 Reach me at **prafullnarang03@gmail.com** or on [LinkedIn](https://www.linkedin.com/in/prafull-narang-02a61b247)

<p align="center"><i>Building things that are fast, tested and actually deployed.</i></p>
