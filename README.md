<!-- =========================
     PROFILE HEADER
========================== -->

<div align="center">

<img
  width="100%"
  src="https://capsule-render.vercel.app/api?type=waving&color=0:4338CA,50:6366F1,100:12A150&height=210&section=header&text=Sreenivasa%20Raju%20Konduru&fontSize=42&fontColor=ffffff&fontAlignY=36&desc=Backend%20Software%20Engineer%20%C2%B7%20Distributed%20Systems%20%C2%B7%20Platform%20Engineering&descAlignY=58&descSize=17"
/>

<a href="https://git.io/typing-svg">
  <img
    src="https://readme-typing-svg.demolab.com?font=IBM+Plex+Mono&weight=600&size=21&duration=3000&pause=900&color=6366F1&center=true&vCenter=true&width=850&lines=Building+reliable+backend+systems;Designing+event-driven+and+distributed+platforms;Java+%7C+Spring+Boot+%7C+Python+%7C+FastAPI;Kafka+%7C+PostgreSQL+%7C+Redis+%7C+Kubernetes;Turning+complex+workflows+into+production-ready+systems"
    alt="Typing introduction"
  />
</a>

<br>

[![Portfolio](https://img.shields.io/badge/Portfolio-4338CA?style=for-the-badge&logo=googlechrome&logoColor=white)](https://sreenivasarajukonduru.github.io/Portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kondurusreenivasaraju)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SreenivasaRajuKonduru)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kondurusreenivasaraju1@gmail.com)

<br>

![Open to Roles](https://img.shields.io/badge/Open%20to-Backend%20%7C%20Platform%20%7C%20SDE-12A150?style=flat-square)
![Location](https://img.shields.io/badge/Location-Gainesville%2C%20Florida-4338CA?style=flat-square)
![Experience](https://img.shields.io/badge/Experience-3%2B%20Years-5B6472?style=flat-square)
![Education](https://img.shields.io/badge/M.S.%20Computer%20Science-University%20of%20Florida-FA4616?style=flat-square)

</div>

---

## 👨‍💻 About Me

I am a **Backend Software Engineer with 3+ years of experience** building Java and Spring Boot microservices, REST APIs, asynchronous integrations, database-driven applications, workflow automation, and production-support solutions.

My experience spans:

- Enterprise Java backend engineering for **USAA claims systems through Tata Consultancy Services**
- Python automation and internal web and data tools at the **University of Florida**
- Distributed job processing with **FastAPI, Kafka, PostgreSQL, Redis, Kubernetes, and observability tooling**
- Production troubleshooting, database optimization, secure credential management, CI/CD, monitoring, and reliability engineering

I enjoy solving problems where systems must remain **reliable, observable, secure, and recoverable under failure**.

---

## 📌 Engineering Snapshot

<table>
<tr>
<td width="50%" valign="top">

### Current Work

**Web Application Developer**  
University of Florida — Transportation & Parking Services

- Build Python automation and internal operational tools
- Develop PostgreSQL validation and reconciliation workflows
- Automate payment-plan, permit, validator, and account workflows with Python, Selenium, and OpenPyXL
- Replace repetitive, error-prone manual work with reliable, auditable workflows
- Support testing, troubleshooting, deployment validation, and production operations

</td>
<td width="50%" valign="top">

### Previous Production Experience

**Assistant Systems Engineer · Java Backend Developer**  
Tata Consultancy Services — Client: USAA

- Built Java 8 and Spring Boot microservices
- Integrated REST APIs and IBM MQ workflows
- Optimized Oracle SQL and connection-pool behavior
- Reduced API latency by **35%**
- Improved response time from **850 ms to 550 ms**
- Supported business-critical production claims applications

</td>
</tr>
</table>

---

# 🚀 Featured Engineering Projects

## 🧩 Distributed Intelligence Runtime

### Distributed Event-Driven Job Processing Platform

A production-style platform for submitting, scheduling, tracking, and executing asynchronous and long-running workloads through independently scalable API and worker services.

### Core Capabilities

- **Event-driven processing:** FastAPI services communicate through Apache Kafka
- **Reliable publishing:** PostgreSQL-to-Kafka delivery using the transactional outbox pattern
- **Failure recovery:** retries, dead-letter queues, controlled replay, and transient-failure handling
- **Safe consumption:** consumer groups and idempotent processing
- **Job lifecycle management:** pending, queued, running, retrying, completed, failed, dead-lettered, and cancelled states
- **Security:** JWT authentication, RBAC, protected routes, centralized authorization, and audit trails
- **Traffic protection:** rate limiting, circuit breakers, and timeout controls
- **Infrastructure:** Docker, NGINX load balancing, Kubernetes service discovery, health checks, readiness probes, and horizontal scaling
- **Observability:** OpenTelemetry, Jaeger, Prometheus, Grafana, structured logging, metrics, and distributed tracing
- **Validation:** load testing, stress testing, and controlled failure simulations

### Architecture

```mermaid
flowchart LR
    Client[Client / API Consumer]
    NGINX[NGINX Load Balancer]
    API1[FastAPI Instance 1]
    API2[FastAPI Instance 2]
    PG[(PostgreSQL)]
    Outbox[(Transactional Outbox)]
    Kafka[Apache Kafka]
    Worker1[Worker Group A]
    Worker2[Worker Group B]
    Redis[(Redis)]
    DLQ[Dead-Letter Queue]
    Replay[Controlled Replay]
    OTel[OpenTelemetry]
    Jaeger[Jaeger]
    Prometheus[Prometheus]
    Grafana[Grafana]

    Client --> NGINX
    NGINX --> API1
    NGINX --> API2

    API1 --> PG
    API2 --> PG

    PG --> Outbox
    Outbox --> Kafka

    Kafka --> Worker1
    Kafka --> Worker2

    Worker1 --> PG
    Worker2 --> PG

    Worker1 --> Redis
    Worker2 --> Redis

    Worker1 -->|failed workload| DLQ
    Worker2 -->|failed workload| DLQ
    DLQ --> Replay
    Replay --> Kafka

    API1 --> OTel
    API2 --> OTel
    Worker1 --> OTel
    Worker2 --> OTel

    OTel --> Jaeger
    API1 --> Prometheus
    API2 --> Prometheus
    Worker1 --> Prometheus
    Worker2 --> Prometheus
    Prometheus --> Grafana
```

**Stack:** `Python` · `FastAPI` · `Apache Kafka` · `PostgreSQL` · `Redis` · `pgvector` · `Docker` · `Kubernetes` · `NGINX` · `JWT / RBAC` · `OpenTelemetry` · `Jaeger` · `Prometheus` · `Grafana`

---

## ⚡ Distributed Reddit Backend Engine

### Multithreaded C++ / PostgreSQL Backend

A multithreaded backend modeling core Reddit-style social features, built to explore concurrency and throughput under load.

### Core Capabilities

- **Features:** post creation, voting, threaded comments, community membership, and feed generation
- **Concurrency:** thread-safe data structures, synchronization controls, and connection management for parallel request handling
- **Throughput:** tested up to **1,000 concurrent connections** with sub-50 ms response times on benchmarked operations in a local test environment

**Stack:** `C++` · `PostgreSQL` · `Multithreading` · `Concurrency` · `Rate Limiting`

> 🔎 More projects — Task Manager, LLM Portfolio, Crime Data Analysis, GatorLibrary, SkillArcade, and Semantic Segmentation — on my [**portfolio**](https://sreenivasarajukonduru.github.io/Portfolio/).

---

## 🎓 Education & Certifications

- 🎓 **M.S. Computer Science** — University of Florida (2025)
- 🎓 **B.E. Computer Science Engineering** — Sathyabama Institute of Science & Technology
- 📜 **AWS Certified Solutions Architect – Associate**
- 📜 **Salesforce Platform Developer I**

---

## 📊 GitHub Stats

<div align="center">

![Sreenivasa's GitHub stats](https://github-readme-stats.vercel.app/api?username=SreenivasaRajuKonduru&show_icons=true&hide_border=true&title_color=4338CA&icon_color=4338CA)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=SreenivasaRajuKonduru&layout=compact&hide_border=true&title_color=4338CA)

</div>

---

<div align="center">

### 💬 Let's connect

I'm open to **backend, platform, and full-stack SDE roles** — happy to walk through any project here, especially the **Distributed Intelligence Runtime**.

[![Portfolio](https://img.shields.io/badge/Portfolio-4338CA?style=for-the-badge&logo=googlechrome&logoColor=white)](https://sreenivasarajukonduru.github.io/Portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kondurusreenivasaraju)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kondurusreenivasaraju1@gmail.com)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:12A150,50:6366F1,100:4338CA&height=110&section=footer" />

</div>
