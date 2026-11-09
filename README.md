
<div align="center">

<!-- DYNAMIC HEADER WAVE & BANNER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e1b4b,100:06b6d4&height=220&section=header&text=RACHIT%20DHERI%20//%20RD998&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Full-Stack%20Engineering%20%E2%80%A2%20Applied%20Computer%20Vision%20%E2%80%A2%20Systems%20Architecture&descAlignY=58&descSize=18" alt="Rachit Dheri Banner" />

<!-- ANIMATED TYPING TAGLINE (Customize your exact GitHub tagline in the 'lines=' parameter below!) -->
<a href="https://github.com/RD998">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=3000&pause=1000&color=06B6D4&center=true&vCenter=true&multiline=false&width=850&height=45&lines=%3E+ Non+ existent+entity+(%F0%9F%AA%A6);%3E+Full-Stack+Web+%26+Browser-Based+ML+%7C+SRM+IST;%3E+Architecting+FastAPI+Backends+%26+Real-Time+Client+Engines;%3E+Breaking+monoliths.+Building+for+scale." alt="Typing SVG" />
</a>

<br/>

<!-- STATUS & TELEMETRY PILLS -->
![Institution](https://img.shields.io/badge/SRM_IST_KTR-Engineering-06b6d4?style=for-the-badge&logo=academia&logoColor=white&labelColor=0f172a)
![Focus](https://img.shields.io/badge/Focus-Systems_&_Applied_AI-8b5cf6?style=for-the-badge&logo=fastapi&logoColor=white&labelColor=0f172a)

[![GitHub Followers](https://img.shields.io/github/followers/RD998?style=for-the-badge&logo=github&color=3b82f6&labelColor=0f172a)](https://github.com/RD998)

</div>

---

### `whoami` // System Telemetry

```yaml
developer: "Rachit Dheri (@RD998)"
location: "SRM Institute of Science and Technology, KTR"
philosophy: "Don't just build static pages—engineer stateful, reactive systems that solve bottlenecks."
architecture_focus:
  - Full-Stack Web Applications (Vanilla JS ES6+, FastAPI, PostgreSQL, MongoDB)
  - Client-Side Machine Learning & AR (PoseNet, Teachable Machine, Web ML)
  - Algorithmic Load-Balancing & Scientific Computing (Python, Cheminformatics, CSV Pipelines)
currently_leveling_up: ["React", "TypeScript", "Docker & Containerization", "Event-Driven Systems"]
```

---

### 🛠️ Interactive Project Blueprints
*Click on any system module below to expand its live architecture diagram and technical breakdown.*

<details open>
<summary><b>🏥 01 // PATHFINDER — Healthcare Routing & Waitlist Engine</b> <i>(Click to toggle architecture)</i></summary>
<br/>

> **The Engineering Problem:** Standard appointment portals fail when schedules fill up and struggle with heavy multi-page payload transfers.  
> **The Solution:** A full-stack medical booking system featuring accessibility filtering, dynamic slot locks, an automated conflict-aware waitlist (`HTTP 409` handling), and a custom client-side `localStorage` state cache that eliminates redundant database reads across page transitions.

```mermaid
graph LR
    A[Client UI: ES6+ JS] -->|URLSearchParams Filter| B(FastAPI Gateway)
    B -->|Query Facilities & Slots| C[(PostgreSQL DB)]
    C -->|1000+ Slot Payload| B
    B -->|JSON Stream| D{Client State Cache}
    D -->|Instant Render| E[Slot Booking & Waitlist UI]
    E -->|POST /waitlist| B
    style A fill:#0f172a,stroke:#06b6d4,stroke-width:2px,color:#fff
    style B fill:#1e1b4b,stroke:#8b5cf6,stroke-width:2px,color:#fff
    style C fill:#0f172a,stroke:#10b981,stroke-width:2px,color:#fff
    style D fill:#06b6d4,stroke:#0f172a,stroke-width:2px,color:#000
    style E fill:#0f172a,stroke:#06b6d4,stroke-width:2px,color:#fff
```

- **Stack:** `JavaScript (ES6+)` • `FastAPI` • `PostgreSQL` • `HTML5/CSS3` • `Render Cloud`
- **Key Mechanics:** Asynchronous `fetch()` orchestration, dynamic query parameterization, geolocation-linked navigation, and real-time waitlist state toggling.
</details>

<details>
<summary><b>🖨️ 02 // ECO-SPOOL — Smart Campus Algorithmic Print Load-Balancer</b> <i>(Click to toggle architecture)</i></summary>
<br/>

> **The Engineering Problem:** Campus printers suffer from massive physical queues and unexpected ink/paper depletion while nearby nodes sit idle.  
> **The Solution:** An IoT-simulated resource router that parses uploaded PDFs in memory, calculates hardware penalty weights across campus nodes, and issues cryptographic/QR claim tickets to route students to the optimal machine.

```mermaid
flowchart TD
    PDF[User Uploads PDF] -->|FormData Stream| API[FastAPI UploadFile Endpoint]
    API -->|PyMuPDF / fitz| META[Extract Page Count & Metadata]
    META --> ALG{Penalty Weighting Engine}
    ALG -->|Node 1: Queue High +25| P1[Library Printer]
    ALG -->|Node 2: Ink Low +40| P2[Hostel Printer]
    ALG -->|Node 3: Optimal Score +5| P3[Tech Park Printer]
    P3 --> QR[Generate Instant QR Claim Ticket]
    style ALG fill:#8b5cf6,stroke:#fff,stroke-width:2px,color:#fff
    style P3 fill:#10b981,stroke:#0f172a,stroke-width:2px,color:#000
    style QR fill:#06b6d4,stroke:#0f172a,stroke-width:2px,color:#000
```

- **Stack:** `Python` • `FastAPI` • `PyMuPDF` • `JavaScript FormData API` • `QRCode.js`
</details>

<details>
<summary><b>👁️ 03 // VISION-SOCIAL SUITE — AR Snapchat & Twitter Clones</b> <i>(Click to toggle architecture)</i></summary>
<br/>

> **The Engineering Problem:** Running computer vision on a backend server introduces massive video latency and high cloud compute costs.  
> **The Solution:** Browser-based Augmented Reality and social platforms running real-time **Pose Estimation** and classification directly on the client's GPU/CPU via Web ML.

```mermaid
sequenceDiagram
    participant Cam as Browser MediaDevices (Webcam)
    participant ML as PoseNet / Teachable Machine
    participant DOM as Canvas & AR Overlay Engine
    Cam->>ML: 30 FPS Video Stream (Client-Side)
    ML->>ML: Real-Time Landmark Keypoint Detection
    ML->>DOM: Mathematical Coordinate Array (X, Y, Confidence)
    DOM->>DOM: Render Dynamic Filters & Social Feed Actions
```

- **Stack:** `Vanilla JavaScript` • `PoseNet` • `Google Teachable Machine` • `WebRTC / MediaDevices API`
</details>

<details>
<summary><b>🧪 04 // ENTERPRISE DATA & COMPUTATIONAL SCIENCE — Earth Core & Cheminformatics</b> <i>(Click to toggle details)</i></summary>
<br/>

- **Earth Core Chemicals Web Utility:** Engineered a custom CSV data processing pipeline and web interface for parsing, structuring, and filtering enterprise chemical datasets.
- **Ammonia Synthesis & Cheminformatics Lab:** Developed Python-based computational models for a **Gibbs Reactor (Ammonia Synthesis)** alongside **SMILES molecular structure parsing** and property visualization scripts.
- **AI Tools Directory & Mobile Suite:** Built curated AI competition platforms and cross-platform mobile utilities using **Thunkable**.
</details>

---

### ⚡ The Technical Arsenal

<div align="center">

| Architectural Layer | Technologies & Tooling |
| :--- | :--- |
| **Frontend & Web ML** | ![JS](https://skillicons.dev/icons?i=js,html,css,ts,react&theme=dark) <br/> *ES6+ DOM Manipulation, Async Fetch, PoseNet, Teachable Machine* |
| **Backend & Data Pipelines** | ![Backend](https://skillicons.dev/icons?i=py,fastapi,postgres,mongodb&theme=dark) <br/> *REST APIs, Algorithmic Routing, CSV Pipelines, Scientific Computing* |
| **DevOps, Security & IDEs** | ![Tools](https://skillicons.dev/icons?i=git,github,vscode,visualstudio,docker&theme=dark) <br/> *Git Workflows, Snyk Security, Render Deployment* |

</div>

---

### 📊 Live GitHub Telemetry & Contribution Matrix

<div align="center">
  <img height="175em" src="https://github-readme-stats.vercel.app/api?username=RD998&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0f172a&title_color=06b6d4&icon_color=8b5cf6" alt="Rachit's GitHub Stats" />
  <img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RD998&layout=compact&theme=tokyonight&hide_border=true&bg_color=0f172a&title_color=06b6d4" alt="Top Languages" />
</div>

<div align="center">
  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=RD998&bg_color=0f172a&color=06b6d4&line=8b5cf6&point=10b981&area=true&hide_border=true" alt="RD998 Activity Graph" />
</div>

---

<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:06b6d4,50:1e1b4b,100:0f172a&height=110&section=footer&text=Let's%20Build%20Something%20Scalable.&fontSize=20&fontColor=ffffff&fontAlignY=65" alt="Footer" />
</div>
