<!-- Animated header banner -->
<p align="center">
  <img src="https://raw.githubusercontent.com/benoumessad-mohamed-el-amine/benoumessad-mohamed-el-amine/main/assets/header.svg" alt="Mohamed El Amine - AI Engineer | Security-focused" width="100%" />
</p>

<!-- Typing animation -->
<h1 align="center">Hi there, I'm Mohamed El Amine 👋</h1>

<p align="center">
  <img src="https://raw.githubusercontent.com/benoumessad-mohamed-el-amine/benoumessad-mohamed-el-amine/main/assets/typing.svg" alt="Typing animation" />
</p>

<h3 align="center">AI Engineer | ML Systems &amp; Multi-Agent | Security-focused</h3>

<p align="center">
  📍 Based in Algeria &nbsp;|&nbsp; 🚀 Specializing in multi-agent runtime security, deterministic execution firewalls, and defensive ML systems.
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=benoumessad-mohamed-el-amine&label=Profile%20views&color=00ff9c&style=for-the-badge" />
</p>

---

## 👨‍💻 About Me

I am an AI Engineer specializing in multi-agent system security, AI runtime governance, and defensive ML systems. I design and build deterministic execution firewalls, tool-call interception proxies, and high-performance network triage systems that protect agentic workflows and critical infrastructure. My work bridges the gap between autonomous agent capabilities and rigorous, low-overhead system defense.

I specialize in:
- 🤖 **Agentic AI & Runtime Safety:** Intercepting and securing tool calls across multi-agent frameworks (LangGraph, CrewAI, AutoGen, MCP) with deterministic policy enforcement and taint tracking.
- 🛡️ **Defensive Systems:** Developing high-throughput packet triage engines, stateful network monitoring, and system-level integrity verification.
- ⚙️ **Systems & Infrastructure:** Building zero-dependency tooling, Linux-native daemons, and cryptographic audit trails for automated environments.
- 🎓 **Technical Leadership:** Mentoring and instructing peers through hands-on technical workshops at the DevUp Scientific Club.

---

## 🛠️ Technologies & Tools

### 🧠 AI Engineering, Multi-Agent & Data Stack
<p>
  <img src="https://img.shields.io/badge/LangGraph-00ff9c?style=for-the-badge&logoColor=black" />
  <img src="https://img.shields.io/badge/Model_Context_Protocol_(MCP)-000000?style=for-the-badge&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/CrewAI-FF4B4B?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/AutoGen-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <br>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
</p>

### 💻 Languages & Runtimes
<p>
  <img src="https://skillicons.dev/icons?i=python,js,ts,java,bash&theme=dark" />
</p>

### 🌐 Backend & Infrastructure
<p>
  <img src="https://skillicons.dev/icons?i=nodejs,express,react,vite,linux,docker,mongodb,postgres,git,github&theme=dark" />
</p>

### 🔐 Defensive & Systems Security
<p>
  <img src="https://img.shields.io/badge/Auditd-1f425f?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Inotify-333333?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" />
  <img src="https://img.shields.io/badge/Nmap-4682B4?style=for-the-badge&logo=nmap&logoColor=white" />
  <img src="https://img.shields.io/badge/Metasploit-2596cd?style=for-the-badge&logo=metasploit&logoColor=white" />
  <img src="https://img.shields.io/badge/Hping3-black?style=for-the-badge" />
</p>

---

## 🚀 Key Projects

### 🤖 AI & Multi-Agent Systems

#### [firewall-warden](https://github.com/benoumessad-mohamed-el-amine/firewall-warden)
* **What / Why:** A deterministic, offline firewall and proxy that intercepts and neutralizes dangerous tool calls in autonomous AI agent workflows.
* **Approach:** Multi-layer security pipeline combining heuristic risk classification, homoglyph normalization, cross-call parameter taint tracking, and an offline stdio proxy for the Model Context Protocol (MCP); governs agent execution across LangGraph, CrewAI, AutoGen, and the OpenAI Agents SDK without calling an LLM.
* **Evaluation:** 100% recall at 100% precision on a 298-sample, 25-family attack corpus; ~58 µs sub-millisecond verdict latency; 400 unit tests passing.
* **How It Runs:** Standalone CLI (`node src/cli.mjs check`), drop-in stdio MCP proxy (`warden-mcp` via `npx` or local Node.js), or imported ES module library.
* **Role:** Repository maintainer and author of integration docs; ported codebase to `firewall-warden`, verified test battery, structured demo scenarios, and authored threat model documentation (`SECURITY.md`).
* **Repository:** [benoumessad-mohamed-el-amine/firewall-warden](https://github.com/benoumessad-mohamed-el-amine/firewall-warden)

#### [NetSpector Pro / Sentinel Flow](https://github.com/benoumessad-mohamed-el-amine/NetSpector-Pro)
* **What / Why:** An automated offline network traffic triage engine designed for high-throughput packet capture analysis and threat detection.
* **Approach:** Bounded LRU flow engine (200,000 capacity) using lightweight slot-based packet indexing (`PacketRef`), stateful TCP tracking, JA3 TLS fingerprinting, and MITRE ATT&CK kill-chain heuristics, paired with a binary ML classification tier <<TODO: add model architecture and library, e.g., Random Forest via Scikit-Learn>>.
* **Evaluation:** Zero external dependencies (100% Python standard library in a ~413 KB `.pyz` binary); <<TODO: add dataset name (e.g. CIC-IDS2017), test accuracy, F1 score, and packet throughput latency>>.
* **How It Runs:** Self-contained executable archive (`netspector.pyz`) via CLI and local browser-based REST triage dashboard.
* **Role:** Solo architect and backend engineer (designed packet indexing engine, flow tracker, and forensic triage modules).
* **Repository:** [benoumessad-mohamed-el-amine/NetSpector-Pro](https://github.com/benoumessad-mohamed-el-amine/NetSpector-Pro)

#### Product Intelligence System
* **What / Why:** An automated market analysis engine designed to extract product signals from commercial documents and synthesize structured intelligence.
* **Approach:** Multi-agent pipeline processing unstructured PDF documents to generate structured insights and 3D visual representations <<TODO: verify agent framework (e.g. LangGraph) and LLM API used>>.
* **Evaluation:** <<TODO: add evaluation benchmark, document processing accuracy, or sample throughput>>.
* **How It Runs:** <<TODO: specify execution mode: CLI, API, or Docker>>.
* **Role:** <<TODO: specify solo vs team contribution and codebase location>>.
* **Repository:** <<TODO: publish or link project repository>>

### 🔒 Security Engineering

#### Silent Fracture (SOAR Platform)
* **What / Why:** A security orchestration, automation, and response (SOAR) platform designed for centralized alert triage and automated incident response workflows.
* **Approach:** Coordinated incident response backend handling alert ingestion and containment automation.
* **Evaluation:** Architected and implemented in a 38-hour development sprint during the InnoByte 2.0 Hackathon; <<TODO: add benchmark metrics, e.g., mean time to remediate (MTTR) or simulated alert volume handled>>.
* **How It Runs:** <<TODO: specify deployment architecture: Docker containers, CLI, or web service>>.
* **Role:** Co-developer and backend architect in a team of 4 (led backend service implementation and system design).
* **Repository:** <<TODO: link repository or submission demo>>

#### [File Integrity Monitor (FIM)](https://github.com/benoumessad-mohamed-el-amine/file-monitoring-integrity-FIM-)
* **What / Why:** A Linux host-based file integrity monitoring utility that detects unauthorized file system modifications and correlates changes to specific users and processes.
* **Approach:** POSIX Bash engine combining real-time `inotifywait` filesystem hooks, Linux `auditd` kernel event logging for PID/user attribution, and cryptographic hash baseline comparisons.
* **Evaluation:** Real-time recursive directory monitoring with desktop notification dispatch; zero third-party compiled dependencies.
* **How It Runs:** Local Linux shell script executed with root privileges (`sudo bash monitor.sh [target_dir]`).
* **Role:** Solo developer.
* **Repository:** [benoumessad-mohamed-el-amine/file-monitoring-integrity-FIM-](https://github.com/benoumessad-mohamed-el-amine/file-monitoring-integrity-FIM-)

---

## 🏆 Achievements & Leadership

*   **3rd Place Podium Finish** ── Shellmates miniCTF at ESI (2025).
*   **Cybersecurity Instructor** ── Designed syllabus and directed 10+ hands-on technical workshops for 23 active members at the DevUp Scientific Club.
*   **Active CTF Competitor** ── Competed in defensive and offensive challenges, including the pentesting-focused Hackini 2.0.

---

## 📊 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=benoumessad-mohamed-el-amine&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=benoumessad-mohamed-el-amine&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=benoumessad-mohamed-el-amine&theme=tokyonight&hide_border=true&background=0d1117&ring=00ff9c&fire=00ff9c&currStreakLabel=00ff9c" alt="GitHub Streak" />
</p>

<!-- Snake: generated by .github/workflows/snake.yml (branch "output") -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/benoumessad-mohamed-el-amine/benoumessad-mohamed-el-amine/output/github-contribution-grid-snake-dark.svg" />
    <img alt="snake animation" src="https://raw.githubusercontent.com/benoumessad-mohamed-el-amine/benoumessad-mohamed-el-amine/output/github-contribution-grid-snake.svg" />
  </picture>
</p>

---

## 🌟 Fun Fact

```python
class Developer:
    def __init__(self):
        self.name = "Mohamed El Amine"
        self.specialties = ["Hybrid NIDS", "Multi-Agent Workflows", "System Security"]
        self.preferred_kernel = "Linux"

    def active_status(self):
        return "Building scalable defensive systems and optimizing agentic AI pipelines. 🚀"

me = Developer()
print(me.active_status())
```

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff9c,50:203a43,100:0f2027&height=120&section=footer" />
</p>
