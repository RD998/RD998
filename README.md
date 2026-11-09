<div align="center">

<!-- DYNAMIC HEADER GRAPHIC -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1e1b4b,100:06b6d4&height=200&section=header&text=RACHIT%20DHERI&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Frontend%20Architecture%20%E2%80%A2%20Computer%20Vision%20%E2%80%A2%20Python%20Pipelines&descAlignY=58&descSize=18" alt="Rachit Dheri Banner" />

<!-- ANIMATED TYPING TAGLINE (URL-Encoded for 100% Reliability) -->
<a href="https://github.com/RD998">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=1000&color=06B6D4&center=true&vCenter=true&multiline=false&width=850&height=45&lines=%3E+Non+existent+entity+%F0%9F%AA%A6;%3E+Frontend+Engineering+%26+Browser-Based+ML+%7C+SRM+IST;%3E+REST+API+Integration+%26+Client-Side+State+Caching;%3E+Building+Reactive+Web+Systems+%26+Data+Pipelines" alt="Typing SVG" />
</a>

<br/>

<!-- TELEMETRY PILLS -->
![SRM IST](https://img.shields.io/badge/SRM_IST_KTR-Engineering-06b6d4?style=for-the-badge&labelColor=0d1117)
![Stack](https://img.shields.io/badge/Focus-JS_ES6+_%7C_Python_%7C_Flask_%7C_Web_ML-8b5cf6?style=for-the-badge&labelColor=0d1117)
[![GitHub Followers](https://img.shields.io/github/followers/RD998?style=for-the-badge&logo=github&color=10b981&labelColor=0d1117)](https://github.com/RD998)

<br/>

<!-- VISUAL TECH STACK ICONS -->
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=js,py,html,css,flask,firebase,bootstrap,git,github,vscode,visualstudio&theme=dark" alt="Tech Stack" />
</a>

</div>

---

### ⚡ System Telemetry // `whoami`

```yaml
entity: "Rachit Dheri (@RD998)"
tagline: "Non existent entity 🪦"
institution: "SRM Institute of Science and Technology"
core_arsenal:
  frontend_&_integration: ["JavaScript (ES6+)", "REST API Integration (fetch)", "localStorage State Caching", "HTML5/CSS3"]
  python_&_cloud:         ["Python", "Flask", "CSV Data Pipelines", "Firebase Realtime Database"]
  computer_vision_ar:     ["ml5.js (PoseNet)", "p5.js Canvas Engine", "Teachable Machine", "Real-Time Keypoint Math"]
```

---

### 🏗️ Interactive Project Blueprints
*Click on any module below to toggle its system architecture diagram.*

<details open>
<summary><b>🏥 01 // PATHFINDER — Client Architecture & API Integration Layer</b></summary>
<br/>

> **My Role (Frontend & API Integration):** Engineered the client-side web application and asynchronous data layer for a multi-page medical appointment platform (interfacing with a teammate's FastAPI/PostgreSQL backend). Built a custom `localStorage` state cache capable of storing 1,000+ time-slot payloads across page transitions with zero redundant network requests, alongside dynamic UI handling for `HTTP 409` waitlist conflicts.

```mermaid
flowchart LR
    subgraph CLIENT ["Client Architecture (My Focus)"]
        UI["ES6+ Client UI"] -->|"URLSearchParams"| FETCH["Async Fetch Layer"]
        FETCH -->|"JSON Stream"| CACHE{"localStorage Cache"}
        CACHE -->|"Zero-Latency Render"| BOOK["Dynamic Booking UI"]
    end
    subgraph SERVER ["Backend Server (Teammate)"]
        API["FastAPI Gateway"] <--> DB[("PostgreSQL DB")]
    end
    FETCH <-->|"REST API + HTTP 409"| API
    style UI fill:#0d1117,stroke:#06b6d4,stroke-width:2px,color:#fff
    style FETCH fill:#0d1117,stroke:#06b6d4,stroke-width:2px,color:#fff
    style CACHE fill:#06b6d4,stroke:#0d1117,stroke-width:2px,color:#000
    style BOOK fill:#0d1117,stroke:#06b6d4,stroke-width:2px,color:#fff
    style API fill:#1e1b4b,stroke:#8b5cf6,stroke-width:2px,color:#fff
    style DB fill:#0d1117,stroke:#10b981,stroke-width:2px,color:#fff
```

- **My Stack:** `JavaScript (ES6+)` • `Async/Await fetch()` • `URLSearchParams` • `HTML5/CSS3`
- **Key Mechanics:** Multi-criteria accessibility filtering, real-time slot state locking, conflict-aware waitlist queuing, and Google Maps coordinate navigation.
</details>

<details open>
<summary><b>🧪 02 // EARTH CORE CHEMICALS — Flask ERP & Automated CSV Pipeline</b></summary>
<br/>

> **The Architecture:** A full-stack enterprise ordering and inventory portal built in **Python (Flask)**. Parses and mutates live `.csv` datasets (`products.csv` and `purchases.csv`) to validate stock availability, compute order totals, trigger an automated 10th-order loyalty discount (`countig`), and generate server-side HTML data tables for administrators.

```mermaid
flowchart LR
    USER["Customer Order POST"] --> FLASK["Flask Route: place_order"]
    FLASK -->|"Read Stream"| PROD[("products.csv")]
    PROD -->|"Validate Stock"| LOGIC{"Loyalty Engine: countig"}
    LOGIC -->|"Order #10"| FREE["100% Loyalty Discount"]
    LOGIC -->|"Standard"| CALC["Quantity x Unit Price"]
    FREE --> PURCH[("purchases.csv")]
    CALC --> PURCH
    PURCH -->|"Dynamic HTML Table"| ADMIN["Admin Portal"]
    style FLASK fill:#1e1b4b,stroke:#8b5cf6,stroke-width:2px,color:#fff
    style LOGIC fill:#06b6d4,stroke:#0d1117,stroke-width:2px,color:#000
    style ADMIN fill:#0d1117,stroke:#10b981,stroke-width:2px,color:#fff
```

- **Stack:** `Python` • `Flask` • `CSV File I/O` • `Jinja2 Templates` • `HTML5/CSS3`
</details>

<details>
<summary><b>👁️ 03 // Modified Filer app — Real-Time Computer Vision & Spatial Scaling</b></summary>
<br/>

> **The Architecture:** A browser-based Augmented Reality filter app built with **p5.js** and **ml5.js (PoseNet)**. Tracks 2D skeletal keypoints (`nose`, `leftEye`, `rightEye`, `leftWrist`, `rightWrist`) in real time and computes pixel coordinate deltas so superhero masks and wrist-mounted spell effects dynamically scale as the user moves toward or away from the webcam.

```mermaid
flowchart LR
    CAM["Webcam Video (p5.js)"] --> ML["ml5.js PoseNet"]
    ML -->|"Skeletal Keypoints"| MATH{"Coordinate Delta Math"}
    MATH -->|"rightEye.x - leftEye.x"| MASK["Dynamic Mask Scaling"]
    MATH -->|"leftWrist.x - rightWrist.x"| SPELL["Wrist Spell Overlays"]
    MASK --> CANVAS["650x650 AR Canvas"]
    SPELL --> CANVAS
    style ML fill:#1e1b4b,stroke:#8b5cf6,stroke-width:2px,color:#fff
    style MATH fill:#06b6d4,stroke:#0d1117,stroke-width:2px,color:#000
    style CANVAS fill:#0d1117,stroke:#10b981,stroke-width:2px,color:#fff
```

- **Stack:** `JavaScript` • `ml5.js (PoseNet)` • `p5.js` • `HTML5 Canvas`
</details>

<details>
<summary><b>💬 04 // QWITTER — Real-Time Cloud Social & Multi-Room Chat Platform</b></summary>
<br/>

> **The Architecture:** A live social messaging web app powered by **Google Firebase Realtime Database**. Uses persistent WebSocket listeners (`on('value')`) to synchronize room creation, stream live chat messages, and update post like counters instantaneously across connected clients.

```mermaid
flowchart LR
    AUTH["localStorage Auth"] --> ROOMS["Room Directory"]
    ROOMS -->|"Create or Join"| FB[("Firebase Realtime DB")]
    FB <-->|"WebSocket on(value)"| CHAT["Live Chat Stream"]
    CHAT -->|"Atomic Like Update"| FB
    style FB fill:#f59e0b,stroke:#0d1117,stroke-width:2px,color:#000
    style CHAT fill:#0d1117,stroke:#06b6d4,stroke-width:2px,color:#fff
    style ROOMS fill:#1e1b4b,stroke:#8b5cf6,stroke-width:2px,color:#fff
```

- **Stack:** `JavaScript` • `Firebase Realtime Database` • `Bootstrap` • `HTML5/CSS3`
</details>

<details>
<summary><b>🌐 05 // FRONTEND UI & CIVIC-TECH SUITE — YouthVoice AI & Technesia G20</b></summary>
<br/>

- **YouthVoice AI:** A civic-awareness platform delivering interactive policy recommendations, custom `.parallax` scrolling effects, and viewport animations via **ScrollReveal.js**.
- **Technesia G20:** An interactive web portal featuring a live case-insensitive DOM card search engine (`searchWebsite()`), a custom programmatic DOM modal prompt backed by `sessionStorage`, and animated navigation drawers.
</details>

---

### 📈 Contribution Map & Live Activity Monitor

<div align="center">

<!-- 52-WEEK CONTRIBUTION HEATMAP -->
<img width="98%" src="https://ghchart.rshah.org/RD998" alt="RD998's GitHub Contribution Map" />

<br/><br/>

<!-- COMMIT STREAK TELEMETRY -->
<img width="65%" src="https://streak-stats.demolab.com?user=RD998&theme=tokyonight&hide_border=true&background=0D1117&stroke=06B6D4&ring=8B5CF6&fire=10B981&currStreakLabel=06B6D4" alt="GitHub Streak Monitor" />

<br/><br/>

<!-- REAL-TIME ACTIVITY MONITOR GRAPH -->
<!--  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=RD998&bg_color=0d1117&color=06b6d4&line=8b5cf6&point=10b981&area=true&hide_border=true" alt="RD998 Real-Time Activity Monitor" />-->

</div>

---

<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:06b6d4,50:1e1b4b,100:0d1117&height=100&section=footer" alt="Footer" />
  <sub>Architected by <b>Rachit Dheri (@RD998)</b> • SRM IST</sub>
</div>
