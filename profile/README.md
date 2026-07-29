<div align="center">

<!-- The mark is white-and-chrome on a dark field, so it would vanish on
     GitHub's light theme. <picture> swaps in a dark card there instead. -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/logo-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="./assets/logo-light.png">
  <img alt="Midalaxy" src="./assets/logo-dark.png" width="500">
</picture>

<br/>

**AI that survives production**

Voice agents, RAG systems and clinical AI running under real load —<br/>
not demos that break the week after launch.

<br/>

[![Website](https://img.shields.io/badge/midalaxy.com-0B0B10?style=for-the-badge&logo=googlechrome&logoColor=A78BFA)](https://midalaxy.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0B0B10?style=for-the-badge&logo=linkedin&logoColor=A78BFA)](https://www.linkedin.com/company/midalaxy/)
[![Email](https://img.shields.io/badge/hello@midalaxy.com-0B0B10?style=for-the-badge&logo=maildotru&logoColor=A78BFA)](mailto:hello@midalaxy.com)

<sub>Bangalore, India — delivering worldwide</sub>

</div>

<br/>

---

## Systems in production

Every number below was measured by the business running the system.

<table>
<tr><th align="left">System</th><th align="left">Measured</th></tr>

<tr><td valign="top">

**Voice intelligence platform**<br/>
<sub>Real-time STT→LLM→TTS with agentic decision loops, post-call automation and Kubernetes auto-scaling</sub>

</td><td valign="top">

`10,000+` concurrent calls<br/>
`<500ms` end-to-end<br/>
`99.9%` uptime · `45%` lower opex

</td></tr>

<tr><td valign="top">

**NHS-grade clinical AI**<br/>
<sub>Deep-learning CT analysis with role-based clinical workflows and automated reporting for lung nodule risk</sub>

</td><td valign="top">

`>0.85` Dice coefficient<br/>
`92%` classification accuracy<br/>
`85%` faster reporting

</td></tr>

<tr><td valign="top">

**Discovery & ranking engine**<br/>
<sub>Multi-phase ranking with GRU event encoding and natural-language search on a real-time vector store</sub>

</td><td valign="top">

`<50ms` retrieval<br/>
`9` prediction heads<br/>
`128-D` embedding search

</td></tr>

<tr><td valign="top">

**Multi-tenant restaurant SaaS**<br/>
<sub>POS, kitchen displays, QR ordering, inventory, reservations and analytics with an embedded booking agent</sub>

</td><td valign="top">

`132` API endpoints<br/>
`53` pages · `9` languages (RTL)<br/>
`23` RBAC scopes

</td></tr>

<tr><td valign="top">

**Agentic video production**<br/>
<sub>LLM-directed pipelines turning declarative manifests into finished video</sub>

</td><td valign="top">

`11` pipeline types<br/>
`0-code` provider swapping

</td></tr>

<tr><td valign="top">

**SiteChat & Estimate256**<br/>
<sub>Zero-code website chatbot platform plus a domain-tuned ML estimation engine</sub>

</td><td valign="top">

`Any URL` → chatbot<br/>
`3` domain-tuned XGBoost models

</td></tr>
</table>

<div align="right"><a href="https://midalaxy.com/work"><b>Full case studies →</b></a></div>

---

## Where the 500ms goes

The latency budget is the whole problem in real-time voice. Above roughly 800ms callers start talking over the agent; below 500ms they simply talk. Every hop is streamed, and nothing waits for the hop before it to finish.

```mermaid
flowchart LR
    A["📞 Caller"] -->|audio| B["Streaming STT<br/><i>partial hypotheses</i>"]
    B -->|"tokens, not utterances"| C["LLM<br/><i>tool-calling</i>"]
    C -->|"first sentence"| D["Streaming TTS"]
    D -->|audio| A
    C <-->|"during generation"| E[("CRM · calendar<br/>knowledge base")]
    C -.->|"barge-in / escalation"| F["Human handoff"]

    style A fill:#0b0b10,stroke:#8b5cf6,color:#f4f4f8
    style B fill:#0b0b10,stroke:#8b5cf6,color:#f4f4f8
    style C fill:#12101c,stroke:#a78bfa,color:#f4f4f8
    style D fill:#0b0b10,stroke:#8b5cf6,color:#f4f4f8
    style E fill:#0b0b10,stroke:#3f3f52,color:#c3cbd9
    style F fill:#0b0b10,stroke:#3f3f52,color:#c3cbd9
```

The hard part was never one call. It was holding that budget while auto-scaling to ten thousand of them.

---

## What we build

<table>
<tr>
<td width="50%" valign="top">

#### [AI Voice Agents](https://midalaxy.com/services/ai-voice-agents)
Phone and web agents that sound human and never sleep. Sub-500ms pipelines, multi-turn memory, CRM and calendar automation.

#### [RAG Chatbots](https://midalaxy.com/services/rag-chatbot-development)
Grounded in your own data, with retrieval you can evaluate and guardrails you can audit.

#### [AI Avatars & Digital Humans](https://midalaxy.com/services/ai-avatar-development)
Lifelike presenters that speak for your brand in real time.

#### [Healthcare AI](https://midalaxy.com/services/healthcare-ai-development)
Clinical-grade imaging, workflows and reporting that clinicians will actually trust.

</td>
<td width="50%" valign="top">

#### [Recommendation & Search](https://midalaxy.com/services/recommendation-engines)
Ranking tuned to conversions and verified outcomes, not clicks.

#### [AI-Powered SaaS](https://midalaxy.com/services/ai-saas-development)
Full-stack multi-tenant platforms with AI built in, shipped to production.

#### [Agentic Workflow Automation](https://midalaxy.com/services/ai-workflow-automation)
Tool-calling agents that remove the busywork between your systems.

#### [AI Video Production](https://midalaxy.com/services/ai-video-production)
Instruction-driven pipelines that turn scripts into finished video at scale.

</td>
</tr>
</table>

---

## How we work

| | |
| :--- | :--- |
| **Fixed milestones, weekly demos** | Working software at every checkpoint, not a big-bang delivery. |
| **The engineers who scope it, build it** | No handoff to juniors after the sales call. |
| **You own everything** | Code, models and documentation transfer to you. Built for handover, not lock-in. |
| **We scope to your budget** | No price list — cost depends entirely on scope. Tell us your budget and we'll say honestly what fits inside it. |
| **We'll talk you out of it** | If an off-the-shelf tool suits you better, we say so. |

---

## Engineering we care about

<div align="center">

![Python](https://img.shields.io/badge/Python-0B0B10?style=flat-square&logo=python&logoColor=A78BFA)
![TypeScript](https://img.shields.io/badge/TypeScript-0B0B10?style=flat-square&logo=typescript&logoColor=A78BFA)
![PyTorch](https://img.shields.io/badge/PyTorch-0B0B10?style=flat-square&logo=pytorch&logoColor=A78BFA)
![LangChain](https://img.shields.io/badge/LangChain-0B0B10?style=flat-square&logo=langchain&logoColor=A78BFA)
![Next.js](https://img.shields.io/badge/Next.js-0B0B10?style=flat-square&logo=nextdotjs&logoColor=A78BFA)
![FastAPI](https://img.shields.io/badge/FastAPI-0B0B10?style=flat-square&logo=fastapi&logoColor=A78BFA)
![Postgres](https://img.shields.io/badge/PostgreSQL-0B0B10?style=flat-square&logo=postgresql&logoColor=A78BFA)
![Redis](https://img.shields.io/badge/Redis-0B0B10?style=flat-square&logo=redis&logoColor=A78BFA)
![Kubernetes](https://img.shields.io/badge/Kubernetes-0B0B10?style=flat-square&logo=kubernetes&logoColor=A78BFA)
![Docker](https://img.shields.io/badge/Docker-0B0B10?style=flat-square&logo=docker&logoColor=A78BFA)

</div>

<br/>

Open problems we're actively working on — latency budgets under load, retrieval measured against real support transcripts rather than benchmarks, and decision loops that survive production — are written up at **[midalaxy.com/labs](https://midalaxy.com/labs)**.

---

<div align="center">

<br/>

### Building something that has to work under load?

**[Start a conversation →](https://midalaxy.com/contact)**

<br/>

<sub>Led by <a href="https://www.linkedin.com/in/mohammed-affaan-khan-048954174">Mohammed Affaan Khan</a><br/>GenAI &amp; Agentic AI engineer · previously JP Morgan Chase</sub>

</div>
