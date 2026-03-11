<p align="center">
  <img src="assets/banner.png" width="100%" alt="Utkarsh Singh Banner" />
</p>

<h1 align="center">Utkarsh Singh</h1>
<p align="center">
  <b>Full Stack Engineer • Backend Systems Architect • AI Integration Specialist</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/utkarsh-singh"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://utkarsh-singh.dev"><img src="https://img.shields.io/badge/Portfolio-FF4B4B?style=for-the-badge&logo=react&logoColor=white" /></a>
  <a href="https://twitter.com/utkarsh_singh"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" /></a>
</p>

---

### 🏛️ Engineering Philosophy
I design and build production-grade systems where **scalability, reliability, and security** are first-class citizens. My approach focuses on modular architectures that handle real-world complexities—such as atomic state management in distributed systems, high-throughput AI pipelines, and real-time media orchestration.

- **Distributed Systems:** Designing for eventual consistency and high availability.
- **AI Infrastructure:** Scaling LLM and Generative AI workflows with robust job orchestration.
- **Cloud Native:** Leveraging serverless and containerized environments for elastic scaling.
- **Security First:** Implementing Row Level Security (RLS), encrypted storage, and secure identity linking.

---

### 💻 Technical Stack

<details open>
<summary><b>Languages & Core</b></summary>
<p align="left">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white" />
</p>
</details>

<details open>
<summary><b>Backend & Infrastructure</b></summary>
<p align="left">
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>
</details>

---

### 🚀 Featured Architectural Projects

> [!TIP]
> **Technical Deep Dive:** For a comprehensive breakdown of my engineering principles and system design patterns, check out the [**ARCHITECTURE.md**](./ARCHITECTURE.md) guide.

#### 1. StudioX — Enterprise AI Media Generation Engine
A full-stack orchestration platform for scalable image and video generation workflows, handling the complete lifecycle from prompt to persistent storage.

**Technical Deep Dive:**
- **Unified API Gateway:** Implemented a consolidated gateway handling authentication, routing, and job orchestration, reducing architectural complexity.
- **Atomic Credit Ledger:** Developed a fail-safe credit system using PostgreSQL RPCs to ensure atomic transactions between job creation and balance deduction, preventing race conditions.
- **Distributed Job Orchestration:** Built a provider-agnostic engine that interfaces with RunPod, Nano Banana, and OpenAI, including robust webhook normalization.
- **Media Pipeline:** A secure, server-side pipeline that fetches transient provider outputs, processes them, and stores them in private cloud buckets to ensure 100% data durability.

```mermaid
graph TD
    A[Client UI] -->|JWT Auth| B[Unified API Gateway]
    B -->|RPC: deduct_credits| C[(PostgreSQL/Supabase)]
    B -->|Dispatch| D[Job Orchestrator]
    D --> E[Provider: RunPod]
    D --> F[Provider: Nano Banana]
    D --> G[Provider: OpenAI]
    E & F & G -->|Webhook| H[Result Handler]
    H -->|Download/Process| I[Storage Pipeline]
    I -->|Store| J[Cloud Storage]
    H -->|Update Status| C
```

---

#### 2. Vibie — High-Throughput Music Streaming Platform
A scalable audio delivery system designed for low-latency streaming and automated media processing.

**Technical Highlights:**
- **Transcoding Pipeline:** Leveraged FFmpeg for high-fidelity audio processing and multi-format transcoding.
- **Streaming Optimization:** Implemented chunked delivery and byte-range request support for seamless playback across variable network conditions.
- **Metadata Indexing:** Optimized PostgreSQL schema for real-time track indexing and lightning-fast search capabilities.

---

#### 3. VaultX — Secure Anonymous File Distribution
An ephemeral file-sharing system optimized for high-performance uploads and secure, encrypted distribution.

**Technical Highlights:**
- **Distributed File Shredding:** Implemented upload chunking to handle multi-gigabyte files efficiently over standard HTTP.
- **Lifecycle Management:** Automated expiration-based file cleanup with secure, deterministic download endpoints.
- **Infrastructure:** Designed to scale horizontally using serverless compute (Cloud Run) and object storage.

---

### 📈 GitHub Metrics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=utkarsh-singh&show_icons=true&theme=tokyonight&count_private=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=utkarsh-singh&layout=compact&theme=tokyonight&hide=css,html" alt="Top Languages" />
</p>

---

### ⚡ Real-Time & Event-Driven Systems
Experienced in building high-concurrency applications using:
- **WebSockets & Socket.IO** for bi-directional live updates.
- **Firestore Realtime Listeners** for seamless UI synchronization.
- **Event-Driven Architectures** utilizing Pub/Sub and Message Queues for asynchronous processing.

---

### 📫 Let's Connect
I'm always open to discussing system design, AI architectures, or full-stack engineering.

- 📧 **Email:** [hello@utkarsh-singh.dev](mailto:hello@utkarsh-singh.dev)
- 💼 **LinkedIn:** [linkedin.com/in/utkarsh-singh](https://linkedin.com/in/utkarsh-singh)
- 🌍 **Web:** [utkarsh-singh.dev](https://utkarsh-singh.dev)

---
<p align="center">
  <i>"The best systems are the ones that work so well, they become invisible."</i>
</p>
