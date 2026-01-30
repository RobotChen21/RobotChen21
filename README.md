<div align="center">
  <h1>Hi there, I'm Chen Yongsai 👋</h1>

  <p>
    <a href="mailto:chenys53@mail2.sysu.edu.cn">
      <img src="https://img.shields.io/badge/SYSU_Mail-chenys53@mail2.sysu.edu.cn-red?style=flat-square&logoColor=white" alt="SYSU Mail"/>
    </a>
    <a href="mailto:yongsaich@foxmail.com">
      <img src="https://img.shields.io/badge/QQ_Mail-yongsaich@foxmail.com-blue?style=flat-square&logo=tencentqq&logoColor=white" alt="QQ Mail"/>
    </a>
    <a href="mailto:nalalyx845@gmail.com">
      <img src="https://img.shields.io/badge/Gmail-nalalyx845@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Gmail"/>
    </a>
    <a href="https://github.com/RobotChen21">
      <img src="https://img.shields.io/badge/GitHub-RobotChen21-black?style=flat-square&logo=github&logoColor=white" alt="GitHub"/>
    </a>
  </p>

  <p>
    <i>Currently debugging life on branch: <code>feat/learn-large-models</code> | PR Status: pending ⏳</i>
  </p>
</div>

<br/>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=RobotChen21&color=blueviolet&style=flat-square&label=Profile+Views" alt="Profile views" />
</div>

<br/>

- 🏫 **M.S. in CS** @ Sun Yat-sen University (2025-2028)
- 🎯 **B.E. in Network Eng.** @ Xidian University (2021-2025)
- 🔭 **Focus**: LLM Fine-tuning (SFT/DPO) & Model Alignment (RLHF)
- 💡 **Passion**: Clean Arch & DDD

<br/>

```java
public class Developer {
    private String name = "Chen Yongsai";
    private String[] roles = { "Backend Engineer", "LLM Application Developer" };
    
    public String[] getLocation() {
        return new String[]{"Guangzhou", "Shenzhen"};
    }
}
```

<div align="center">
  <h2>🛠️ Tech Stack</h2>

  <h3>Backend & Microservices</h3>
  <p>
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
    <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
    <img src="https://img.shields.io/badge/Spring_Cloud-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
    <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
    <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
    <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" />
    <br/>
    <img src="https://img.shields.io/badge/MyBatis-DC382D?style=for-the-badge&logo=databricks&logoColor=white" />
    <img src="https://img.shields.io/badge/Apache_Dubbo-FE7A16?style=for-the-badge&logo=apache&logoColor=white" />
  </p>

  <h3>LLM & AI Stack</h3>
  <p>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
    <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
    <br/>
    <img src="https://img.shields.io/badge/vLLM-6366F1?style=for-the-badge&logo=v&logoColor=white" />
    <img src="https://img.shields.io/badge/LLaMA_Factory-FFA500?style=for-the-badge&logo=meta&logoColor=white" />
    <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
    <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
    <img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white" />
  </p>

  <h3>Tools & DevOps</h3>
  <p>
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
    <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" />
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
    <img src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" />
  </p>
</div>

## 🚀 Featured Projects

### 🎯 [Cloud-Native Campus](https://github.com/RobotChen21/cloud-native-campus)
> **Microservices Architecture Design & High-Concurrency Community Optimization** | *Refactoring & Performance Tuning*

A comprehensive microservices-based online education platform. Focused on performance bottleneck analysis and system refactoring for the interactive community (comments & likes) and promotion modules.

**Highlights:**
- 🔄 **Interaction Refactoring**: Designed **Hot/Cold Data Separation**: hot data (3 months) in Redis ZSet for ms-level response; cold data in DB with **Bloom Filter** to block invalid queries (latency 200ms+ → 10ms). Solved high-concurrency write bottlenecks using **MQ + Local Write-Behind**.
- 🛡️ **Concurrency Optimization**: Implemented **Redisson + Lua** double atomic validation to prevent overselling/over-claiming. Used **Sequence Space Mapping** for massive redemption code generation and **BitMap** for deduplication, reducing memory by **98%** with O(1) checks.
- ⚙️ **System Governance**: Built **Hotspot Dual-Mode Engine** (Global Aggregation + Local Caffeine Downgrade). Designed application-layer **CDC simulation** for **ES partial updates** to avoid data coverage risks. efficiently handled **BigKeys** via **xxl-job sharded broadcasting** and async deletion.

**Tech Stack**: `Spring Boot` `Spring Cloud` `MySQL` `Redis` `RabbitMQ` `xxl-job` `Elasticsearch` `Caffeine` `Redisson`

---

### 💘 [Digital Matchmaker](https://github.com/RobotChen21/digital-matchmaker-recommand)
> **AI-Native Dating Recommendation Engine** | *Solo Full-Stack Project*

*Because `SELECT * FROM users WHERE perfect_match = true` never finds true love 😄*

An AI-powered dating platform replacing forms with conversational profiling.

**Key Innovations:**
- 🤖 **Agentic Workflow**: LangGraph-orchestrated multi-turn dialogue with state persistence
- 🧠 **Model Alignment**: DeepSeek → SFT/DPO distilled fine-tuning for natural tone
- 🚀 **Inference**: vLLM + Multi-LoRA (90% cost reduction vs API)
- 🔍 **Hybrid Retrieval**: MongoDB (Filter) → ElasticSearch (KNN/BM25) → RAG (Psych Ranking)

**Tech Stack**: `Python` `FastAPI` `LangGraph` `vLLM` `LLaMA Factory` `Elasticsearch` `MongoDB`

---

## 📊 GitHub Stats

<div align="center">   
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=RobotChen21&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="GitHub Stats" />   
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RobotChen21&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="Top Languages" /> 
</div> 
<br/> 
<div align="center">   
  <img width="70%" src="https://github-readme-activity-graph.vercel.app/graph?username=RobotChen21&theme=tokyo-night&hide_border=true&bg_color=0d1117&color=70a5fd&line=bf91f3&point=38bdae" alt="Activity Graph" /> 
</div>

## 🏆 Achievements

- 🥇 **MCM/ICM Finalist** (Top 3% globally in Mathematical Contest in Modeling)
- 📜 **CET-4/6 Certificates**
- 🏅 University Scholarships (4×)

## 💭 Philosophy

> "Code is poetry written in logic. I don't just implement features — I architect solutions, optimize performance, and obsess over clean design patterns."

- 🔬 **Deep Diver**: Digging into source code & principles
- 📚 **Documentation**: Official docs > Tutorials
- 🎯 **Quality**: Strict adherence to standards
- 🤝 **Collaboration**: Git Flow & Code Review advocate

## 📈 Current Learning Path

```mermaid
graph TD
    %% 定义样式类
    classDef ai fill:#e1f5fe,stroke:#01579b,stroke-width:2px,color:#01579b;
    classDef be fill:#fff3e0,stroke:#e65100,stroke-width:2px,color:#e65100;
    classDef goal fill:#e8f5e9,stroke:#1b5e20,stroke-width:4px,color:#1b5e20;

    subgraph LLM_Path [🤖 AI & LLM Specialization]
        direction TB
        A[LLM Fundamentals]:::ai --> B[Fine-tuning SFT/DPO]:::ai
        B --> C[Model Alignment RLHF]:::ai
        C --> D[RAG & Vector DB]:::ai
        D --> E[Agentic Workflows]:::ai
    end

    subgraph Backend_Path [🛠️ Backend & Architecture]
        direction TB
        F[Business Logic & CRUD]:::be --> G[Microservices & RPC]:::be
        G --> H[DDD & Clean Arch]:::be
        H --> I[High Concurrency/Performance]:::be
        I --> J[Distributed System Design]:::be
    end

    %% 两条路最终汇聚的目标
    E --> K[Build AI-Native Applications]:::goal
    J --> K
```
