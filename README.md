<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Prafull%20Narang&fontSize=56&fontColor=ffffff&fontAlignY=36&desc=MCA%20%40%20NIT%20Warangal%20%C2%B7%20Class%20of%202027&descAlignY=58&descSize=18&animation=fadeIn" width="100%"/>

<div align="center">

<a href="https://github.com/prafullf"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=620&lines=Backend+%26+Distributed+Systems+Engineer;GenAI+%2F+RAG+Builder;Multi-threaded+C%2B%2B+Developer;Open+to+SDE+%26+ML+roles+%E2%80%94+2027+batch" alt="Typing SVG"/></a>

<a href="https://www.linkedin.com/in/prafull-narang-02a61b247"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:prafullnarang03@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://leetcode.com/u/wGm6kK22FK/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>
<img src="https://komarev.com/ghpvc/?username=prafullf&label=Profile%20views&color=58a6ff&style=for-the-badge" alt="Profile views"/>

</div>

---

### 👨‍💻 About me

```yaml
name:      Prafull Narang
education: MCA, NIT Warangal (2024–2027)
research:  Research Intern @ NIT Warangal — statistical model checking on 670K+ real COVID-19 cases
building:  distributed backends · RAG systems · high-throughput C++ pipelines
looking:   SDE / Backend / ML Engineer roles (full-time, 2027)
fun_fact:  AIR 1956 in NIMCET 2024
```

---

### 📈 Numbers I'm proud of

<div align="center">

| ⚡ **2.7 M/s** | 🎯 **99.8%** | 🚀 **p95 240 ms** | ✅ **86 tests** |
|:---:|:---:|:---:|:---:|
| samples processed by my C++17 telemetry agent, zero loss | DDoS detection accuracy, attacks blocked in 1.6 s | sandboxed code-run turnaround at 200 runs/min | in CodeSync, plus E2E, load tests and CI |

</div>

---

### 🛠️ Featured projects

<table>
<tr>
<td colspan="2">

#### 🟦 [CodeSync — Real-time Collaborative Code Editor](https://github.com/prafullf/codesync)
Live multi-user editing with cursors, plus a **Run** button that executes Python / JS / C++ in a fresh, network-less Docker sandbox. Everyone in the room sees the output.

<img src="https://raw.githubusercontent.com/prafullf/codesync/main/docs/demo.gif" alt="CodeSync demo" width="100%"/>

**Yjs CRDT** · **Fastify → BullMQ → 3 workers → isolated container** · Redis sliding-window rate limiter · 600/600 runs at 200/min, 0% errors · 86 tests + Playwright + k6 · deployed on Azure

<img src="https://skillicons.dev/icons?i=ts,react,nodejs,redis,postgres,prisma,docker,azure,githubactions&perline=9" height="34"/>

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🤖 [RAG Document Q&A](https://github.com/prafullf/rag-document-qa)
Ask questions about your own PDFs. Answers come **only** from retrieved passages, with numbered citations to file and page.

- pgvector top-k search over Gemini embeddings
- Relevance gate: no LLM call when nothing matches
- Content-hash chunk IDs, so re-uploads never duplicate

<img src="https://skillicons.dev/icons?i=py,postgres,docker" height="30"/> &nbsp;`LangChain` `Gemini` `Streamlit`

</td>
<td width="50%" valign="top">

#### ⚙️ [Optical Telemetry & Alarm Agent](https://github.com/prafullf/optical-telemetry-agent)
Multi-threaded **C++17** agent that raises network alarms like real optical gear: hysteresis, debouncing, root-cause masking.

- **~2.7 M samples/s**, p99 **289 µs** decision latency
- Port-affinity sharding means no locks on per-port state
- CI under **TSan, ASan and UBSan**; 35 tests

<img src="https://skillicons.dev/icons?i=cpp,cmake,linux,githubactions" height="30"/>

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🛡️ [ML DDoS Detection for IoT (SDN)](https://github.com/prafullf/ml-ddos-detection-iot-sdn)
A Random Forest inside a Ryu controller classifies every IoT flow each second and installs OpenFlow drop rules.

- **99.8%** accuracy, false positives **2.7% → 0.1%**
- **99.5%** legit traffic delivered under attack (vs 73.9%)
- Blocked 4/4 attacks in **1.6 s**

<img src="https://skillicons.dev/icons?i=py,sklearn,linux,docker" height="30"/> &nbsp;`Ryu` `Mininet`

</td>
<td width="50%" valign="top">

#### 📊 [COVID-19 Statistical Model Checking](https://github.com/prafullf/covid19-smc-telangana)
**Research internship, NIT Warangal.** Agent-based SIR Monte Carlo model on 609 days of Telangana data.

- **670K+** real cases used to estimate β and γ
- Chernoff–Hoeffding bound → **737 runs** for ±0.05 at 95%
- Vaccination cut outbreak probability **0.998 → 0.936**

<img src="https://skillicons.dev/icons?i=py" height="30"/> &nbsp;`NumPy` `Pandas` `Monte Carlo`

</td>
</tr>
</table>

---

### 🧰 Tech stack

<div align="center">

**Languages**<br/>
<img src="https://skillicons.dev/icons?i=py,cpp,ts,js,mysql&perline=8"/>

**Backend & frontend**<br/>
<img src="https://skillicons.dev/icons?i=fastapi,nodejs,react,redis,postgres&perline=8"/>

**AI / ML**<br/>
<img src="https://skillicons.dev/icons?i=pytorch,sklearn&perline=8"/> &nbsp; <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" height="40"/> <img src="https://img.shields.io/badge/RAG%20%C2%B7%20pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white" height="40"/>

**DevOps & tools**<br/>
<img src="https://skillicons.dev/icons?i=docker,azure,githubactions,linux,git,cmake&perline=8"/>

</div>

---

<div align="center">

### 🤝 Let's connect

Open to **SDE · Backend · ML/GenAI** roles for the 2027 batch.<br/>
The fastest way to reach me is **[prafullnarang03@gmail.com](mailto:prafullnarang03@gmail.com)** or **[LinkedIn](https://www.linkedin.com/in/prafull-narang-02a61b247)**.

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" width="100%"/>
