<div align="center">

# Hi, I'm Sreenivasa Raju Konduru 👋

### Software Engineer · Backend & Distributed Systems

Building reliable backend systems that move work through pipelines without losing it — from enterprise Java services in production to a self-built distributed job-processing platform.

<br>

![Open to SDE roles](https://img.shields.io/badge/Open%20to-SDE%20Roles-12A150?style=for-the-badge)
![Available now](https://img.shields.io/badge/Availability-Now-4338CA?style=for-the-badge)
![Location](https://img.shields.io/badge/US-Remote%20%2F%20Hybrid%20%2F%20On--site-555?style=for-the-badge)

[![Portfolio](https://img.shields.io/badge/Portfolio-4338CA?style=for-the-badge&logo=google-chrome&logoColor=white)](https://sreenivasarajukonduru.github.io/Portfolio)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kondurusreenivasaraju)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kondurusreenivasaraju1@gmail.com)

</div>

---

## 🧑‍💻 About Me

- 🔭 **Software Engineer** with **3+ years** building backend services, REST APIs, and database-driven applications.
- ⚙️ Currently a **Web Application Developer** at the **University of Florida — Transportation & Parking Services**, building Python automation, backend integrations, and internal tools.
- 🏦 Previously **Assistant Systems Engineer | Java Backend Developer** at **Tata Consultancy Services (Client: USAA)**, shipping Java/Spring Boot microservices for enterprise claims systems.
- 🎓 **M.S. in Computer Science**, University of Florida (2025).
- 🚀 Most interested in **distributed systems, event-driven architecture, and backend reliability** — see the **Distributed Intelligence Runtime** below.

---

## 🛠️ Tech Stack

**Languages**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Backend & APIs**

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST%20APIs-4338CA?style=flat-square)
![Microservices](https://img.shields.io/badge/Microservices-5B6472?style=flat-square)

**Distributed Systems & Messaging**

![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![IBM MQ](https://img.shields.io/badge/IBM%20MQ-052FAD?style=flat-square&logo=ibm&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Observability & Security**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

---

## 🚀 Featured Projects

### 🧩 Distributed Intelligence Runtime — *Distributed Job Processing Platform*
A self-built platform for submitting, scheduling, and executing asynchronous, long-running work — designed around reliability and end-to-end observability.
- **Event-driven core:** independently scalable **FastAPI** API and worker services communicating through **Kafka**.
- **Reliable publishing:** **PostgreSQL → Kafka** via the transactional **outbox pattern**, with consumer groups, idempotent processing, retries, **dead-letter queues**, and controlled replay.
- **Job lifecycle:** PostgreSQL-tracked states (pending → queued → running → retrying → completed / failed / dead-lettered), with **Redis** for caching, coordination, and distributed rate limiting.
- **Security & delivery:** **JWT**, **RBAC**, audit trails, circuit breakers; deployed behind **NGINX** + **Kubernetes** with health checks and horizontal scaling.
- **Observability:** **OpenTelemetry, Jaeger, Prometheus, Grafana** — validated with load and failure-simulation testing.

`Python` · `FastAPI` · `Apache Kafka` · `PostgreSQL` · `Redis` · `pgvector` · `Docker` · `Kubernetes` · `OpenTelemetry`

### ⚡ Distributed Reddit Backend Engine
A multithreaded **C++ and PostgreSQL** backend modeling core Reddit-style features — posts, voting, threaded comments, communities, and feeds — built to explore concurrency and throughput.
- Thread-safe data structures, synchronization controls, and connection management.
- Tested up to **1,000 concurrent connections** with sub-50 ms response times on benchmarked operations in a local test environment.

`C++` · `PostgreSQL` · `Multithreading` · `Concurrency`

> 🔎 More projects — Task Manager, LLM Portfolio, Crime Data Analysis, GatorLibrary, SkillArcade, Semantic Segmentation — on my [**portfolio**](https://sreenivasarajukonduru.github.io/Portfolio).

---

## 💼 Experience

| Role | Company | When |
| --- | --- | --- |
| **Web Application Developer** | University of Florida — Transportation & Parking Services | Sep 2024 – Present |
| **Assistant Systems Engineer \| Java Backend Developer** | Tata Consultancy Services (Client: USAA) | Apr 2021 – Aug 2023 |

**Highlight:** reduced API response latency **~35% (850 ms → 550 ms)** on business-critical USAA claims services by optimizing Oracle SQL queries, indexes, and connection-pool configuration.

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

I'm open to backend, full-stack, and platform SDE roles — happy to talk through any project here, especially the Distributed Intelligence Runtime.

[![Portfolio](https://img.shields.io/badge/Portfolio-4338CA?style=for-the-badge&logo=google-chrome&logoColor=white)](https://sreenivasarajukonduru.github.io/Portfolio)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kondurusreenivasaraju)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kondurusreenivasaraju1@gmail.com)

</div>
