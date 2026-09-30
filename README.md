<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0F0C29,30:302B63,60:24243E,100:0E75B6&height=260&section=header&text=PURNA%20VENKATA%20PRASANTH&fontSize=46&fontColor=00F5D4&fontAlignY=40&animation=twinkling&desc=I%20build%20AI%20systems%20that%20talk%20to%20each%20other%20%E2%80%94%20and%20the%20cloud%20they%20run%20on&descSize=17&descColor=FEE440&descAlignY=63" alt="header" />

<a href="https://github.com/prasanth1218">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=2800&pause=800&color=F15BB5&center=true&vCenter=true&width=820&lines=%24+whoami+%E2%86%92+GenAI+%2F+LLM+Application+Engineer;%24+building+%E2%86%92+multi-agent+systems+that+work+in+production;%24+shipping+%E2%86%92+RAG+apps+that+refuse+to+hallucinate;%24+provisioning+%E2%86%92+AWS+infra+with+Terraform;%24+status+%E2%86%92+open+to+relocation+%26+ready+to+own+real+systems" alt="Typing SVG" />
</a>

<br/><br/>

<a href="https://purnaprasanth.netlify.app/"><img src="https://img.shields.io/badge/🌐_PORTFOLIO-00F5D4?style=for-the-badge&labelColor=0F0C29" alt="Portfolio"/></a>
<a href="https://www.linkedin.com/in/purna-venkata-prasanth-meesala-274790256/"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0F0C29" alt="LinkedIn"/></a>
<a href="mailto:prasanthmeesala2@gmail.com"><img src="https://img.shields.io/badge/EMAIL-F15BB5?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0F0C29" alt="Email"/></a>
<img src="https://komarev.com/ghpvc/?username=prasanth1218&color=FEE440&style=for-the-badge&label=VISITORS&labelColor=0F0C29" alt="Visitors"/>

</div>

<br/>

## ⚡ 30-Second Recruiter Scan

<div align="center">

| 🎯 Looking for | 🧠 Core strength | ☁️ Infrastructure | 🎓 Education | 🌍 Location |
|:---:|:---:|:---:|:---:|:---:|
| **Entry-level GenAI / Cloud Engineer** | **Multi-agent LLMs + RAG** | **AWS + Terraform (IaC)** | **B.Tech AI & DS, 2026** | **India · Open to relocation** |

</div>

> 💡 **What sets me apart:** I don't just call an LLM API. I design the whole system: agents, retrieval, validation, streaming, deployment and the infrastructure underneath, and I make it **explainable** and **safe against hallucination**.

<br/>

## 👨‍💻 `about_me.py`

```python
class Prasanth:
    name      = "Purna Venkata Prasanth"
    role      = "GenAI / LLM Application Engineer"
    education = "B.Tech, AI & Data Science (2026), Dhanalakshmi Srinivasan University"

    builds = [
        "Multi-agent LLM platforms with real-time SSE streaming",
        "RAG pipelines that refuse instead of hallucinate",
        "AWS infrastructure as code with Terraform",
    ]

    philosophy = "Build it, break it, fix it, ship it."

    currently = {
        "exploring": ["Agentic AI", "Production-grade RAG", "AWS + Terraform"],
        "seeking":   "Entry-level GenAI or Cloud Engineering role with real ownership",
        "relocation": True,
    }

    def contact(self):
        return "prasanthmeesala2@gmail.com"
```

<br/>

## 🧬 How My Projects Actually Work

### 🧠 NexusAI: Multi-Agent LLM Platform *(simplified flow)*

```mermaid
flowchart LR
    U([👤 User Task]) --> F[⚛️ React + Vite<br/>Vercel]
    F -->|request| B[⚡ FastAPI<br/>Render]
    B --> P{{🗺️ Planner}}
    P --> C[💻 Coder]
    P --> W[✍️ Writer]
    P --> R[🔎 Researcher]
    C --> V{{✅ Reviewer}}
    W --> V
    R --> V
    V -->|SSE stream| F
    B -.->|Groq API + LLaMA-3| P

    style U fill:#F15BB5,stroke:#fff,color:#fff
    style F fill:#0E75B6,stroke:#fff,color:#fff
    style B fill:#009688,stroke:#fff,color:#fff
    style P fill:#7B42BC,stroke:#fff,color:#fff
    style V fill:#FF6B6B,stroke:#fff,color:#fff
    style C fill:#302B63,stroke:#00F5D4,color:#fff
    style W fill:#302B63,stroke:#00F5D4,color:#fff
    style R fill:#302B63,stroke:#00F5D4,color:#fff
```

Five specialized agents coordinate on one task and stream results back live. I also solved the unglamorous parts: agent-to-agent message passing, CORS, and dev-vs-prod config. The architecture was written up as a **co-authored research paper**.

[![Repo](https://img.shields.io/badge/⭐_VIEW_REPO-multi--agent--nexus-00F5D4?style=for-the-badge&labelColor=0F0C29)](https://github.com/prasanth1218/multi-agent-nexus)

<br/>

### 🏢 Enterprise AI Research Agent: 4-Step Explainable RAG

```mermaid
flowchart LR
    Q([❓ Policy Question]) --> S1[1️⃣ Query<br/>Understanding]
    S1 --> S2[2️⃣ Retrieval<br/>ChromaDB]
    S2 --> S3{3️⃣ Validation<br/>Is context relevant?}
    S3 -->|✅ Yes| S4[4️⃣ Generation<br/>Groq LLaMA 3.1]
    S3 -->|❌ No| X([🚫 Refuse to answer<br/>no hallucination])
    S4 --> A([💬 Grounded Answer])
    S4 -.-> DB[(🐘 PostgreSQL<br/>audit log)]

    style Q fill:#F15BB5,stroke:#fff,color:#fff
    style S1 fill:#302B63,stroke:#00F5D4,color:#fff
    style S2 fill:#FF6446,stroke:#fff,color:#fff
    style S3 fill:#FEE440,stroke:#333,color:#000
    style S4 fill:#F55036,stroke:#fff,color:#fff
    style X fill:#D00000,stroke:#fff,color:#fff
    style A fill:#00B894,stroke:#fff,color:#fff
    style DB fill:#4169E1,stroke:#fff,color:#fff
```

I skipped LangChain on purpose and hand-built each step, so every decision the system makes stays **explainable**. A self-healing ingestion job re-indexes documents on startup, so data survives free-tier restarts.

[![Repo](https://img.shields.io/badge/⭐_VIEW_REPO-enterprise--ai--research--agent-FEE440?style=for-the-badge&labelColor=0F0C29)](https://github.com/prasanth1218/Generative-AI-Projects/tree/main/enterprise-ai-research-agent)

<br/>

### ☁️ AWS + Terraform: Environment as Code

```mermaid
flowchart TB
    TF[📜 Terraform Config] --> VPC[🌐 VPC Networking]
    TF --> SG[🛡️ Security Groups]
    TF --> IAM[🔑 IAM Roles]
    TF --> EC2[🖥️ EC2 Instances]
    VPC --> EC2
    SG --> EC2
    IAM --> EC2
    EC2 -.->|terraform destroy / apply| TF

    style TF fill:#7B42BC,stroke:#fff,color:#fff
    style VPC fill:#FF9900,stroke:#fff,color:#000
    style SG fill:#FF9900,stroke:#fff,color:#000
    style IAM fill:#FF9900,stroke:#fff,color:#000
    style EC2 fill:#232F3E,stroke:#FF9900,color:#fff
```

The whole environment can be torn down and rebuilt from code instead of clicked together by hand, with reusable templates that stay consistent across dev and prod.

[![Repo](https://img.shields.io/badge/⭐_VIEW_REPO-Terraform--projects-7B42BC?style=for-the-badge&labelColor=0F0C29)](https://github.com/prasanth1218/Terrraform-projects)

<br/>

## 🗂️ More Projects

<table>
<tr>
<td width="50%" valign="top">

### 🩺 Medical Chatbot
**RAG-based Question Answering**

Answers medical queries from grounded context in **Pinecone** instead of letting the LLM answer unaided. I built the PDF ingestion myself: chunking plus **HuggingFace sentence-transformers** embeddings, chained with **LangChain**, served by a **Flask** app with a real-time chat UI.

![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

[![Repo](https://img.shields.io/badge/VIEW_REPO-4ECDC4?style=for-the-badge&logo=github&logoColor=black)](https://github.com/prasanth1218/Generative-AI-Projects/tree/main/End-to-end-Medical-Chatbot-Generative-AI-main)

</td>
<td width="50%" valign="top">

### 📉 Hushh Drop-Off Detection
**Hackathon · Team ZeroDrops**

Flags users dropping off mid-flow on e-commerce/SaaS platforms and re-engages them automatically with push notifications and email recovery flows. Built with a small team: **React** dashboard, **Node/Express/Firebase** backend and a **React Native** app.

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Node](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![RN](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)

[![Repo](https://img.shields.io/badge/VIEW_REPO-F15BB5?style=for-the-badge&logo=github&logoColor=white)](https://github.com/prasanth1218/hushh-dropoff-dashboard)

</td>
</tr>
</table>

<br/>

## 🛠️ Tech Arsenal

<div align="center">

**🤖 Generative AI**<br/>
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=for-the-badge&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)

**☁️ Cloud & DevOps**<br/>
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![CloudFormation](https://img.shields.io/badge/CloudFormation-E7157B?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**💻 Build**<br/>
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=FFD43B)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

**📈 ML & Data**<br/>
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

</div>

<br/>

## 🧩 How I Work

```mermaid
mindmap
  root((Prasanth))
    Build
      Multi-agent LLMs
      RAG pipelines
      Full-stack apps
    Ship
      Vercel and Render
      AWS EC2
      Terraform IaC
    Principles
      Explainable over magic
      Refuse over hallucinate
      Rebuild from code
```

<br/>

## 🎓 Education & Certifications

<div align="center">

| | |
|:---|:---|
| 🎓 **B.Tech, AI & Data Science** | Dhanalakshmi Srinivasan University, Trichy · 2022 – 2026 · CGPA 7.73 / 10 |
| 🏅 **Oracle Certified Foundations Associate: Agentic AI** | Oracle University · Aug 2026 |
| ☁️ **Cloud Computing (AWS)** | LaunchED Global |
| 💻 **Full Stack Web Development** | Skolar |
| 🤝 **Certificate of Membership** | NSPE |

</div>

<br/>

## 📊 GitHub Analytics

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=prasanth1218&show_icons=true&theme=synthwave&hide_border=true&count_private=true" alt="Stats" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=prasanth1218&layout=compact&theme=synthwave&hide_border=true" alt="Top Languages" />

<img src="https://streak-stats.demolab.com?user=prasanth1218&theme=synthwave&hide_border=true" alt="Streak" />

<img src="https://github-profile-trophy.vercel.app/?username=prasanth1218&theme=onedark&no-frame=true&no-bg=true&row=1&column=6" alt="Trophies" />

</div>

<br/>

## 🤝 Let's Build Something

<div align="center">

**I'm looking for an entry-level Generative AI or Cloud Engineering role where I can own real systems.**
*Relocation welcome.*

<br/>

<a href="mailto:prasanthmeesala2@gmail.com"><img src="https://img.shields.io/badge/📩_HIRE_ME-F15BB5?style=for-the-badge&labelColor=0F0C29" alt="Hire me"/></a>
<a href="https://www.linkedin.com/in/purna-venkata-prasanth-meesala-274790256/"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0F0C29" alt="LinkedIn"/></a>
<a href="https://purnaprasanth.netlify.app/"><img src="https://img.shields.io/badge/PORTFOLIO-00F5D4?style=for-the-badge&labelColor=0F0C29" alt="Portfolio"/></a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0E75B6,50:302B63,100:0F0C29&height=130&section=footer&text=Thanks%20for%20visiting%20%F0%9F%9A%80&fontSize=22&fontColor=00F5D4&fontAlignY=68" alt="footer" />

</div>
