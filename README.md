<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=24&pause=1000&color=6366F1&center=true&vCenter=true&width=520&lines=Hi%2C+I'm+Sabina+Ruzieva;Student+%C2%B7+AI+Integration+%26+Automation;Connecting+AI+to+workflows+that+actually+ship" alt="Typing intro" />

<br />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-sabina--ruzieva-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sabina-ruzieva/)
[![Email](https://img.shields.io/badge/Email-sabinaruzieva04%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sabinaruzieva04@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-sabinova-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sabinova)

</div>

---

I'm a student focused on **AI integration, automation, and data** — building systems that connect LLMs and ML models to the tools teams already use. I care about prompt design, reliable pipelines, and human-in-the-loop workflows, not just demos.

Currently finishing my capstone: an [AI Email Triage & Auto-Responder](https://github.com/rimshatahir/ai-capstone-email-triage) that classifies inbox traffic and drafts replies for human review.

## Featured Project

### [Email Triage & Auto-Responder](https://github.com/rimshatahir/ai-capstone-email-triage)

An AI-powered assistant for teams drowning in email — it classifies incoming messages by category and urgency, generates draft replies, and routes everything through a review dashboard so nothing important gets lost.

| | |
|---|---|
| **Problem** | Email overload buries urgent messages and slows routine responses. |
| **My role** | **Component 2 — Auto Response Drafting:** designed the LLM prompt, built the Flowise chain (Groq Llama 3.3 70B), and wired the n8n workflow that polls Airtable, generates drafts, and writes them to a human review queue. |
| **Outcome** | 13 classified emails processed end-to-end; category-aware drafts with safety guardrails (`[insert …]` placeholders, no false promises, spam filtered via `NO_DRAFT_NEEDED`). |
| **Links** | [Capstone repo](https://github.com/rimshatahir/ai-capstone-email-triage) · [My component](https://github.com/rimshatahir/ai-capstone-email-triage/tree/main/component_2_Sabina_auto-response) · Demo video *coming soon* |

<details>
<summary><strong>How my component fits in</strong></summary>

<br />

```mermaid
flowchart LR
    A["Airtable\nStatus: Classified"] --> B["n8n\npoll every 5 min"]
    B --> C["Flowise LLM Chain\nGroq Llama 3.3 70B"]
    C --> D{"Draft needed?"}
    D -->|yes| E["Response Drafts\nNEEDS_REVIEW"]
    D -->|no| F["Status updated\nno draft"]
    E --> G["Human reviewer"]
```

</details>

## What I Work With

**Automation & integration** · n8n · Flowise · Airtable · Groq · Hugging Face · GitHub

**Data & code** · Python · SQL *(actively building)*

## Currently Learning

- **AI/ML & model evaluation** — understanding when to trust a model's output vs. route to human review
- **Data engineering & analysis** — stronger Python and SQL for building and testing data pipelines

## Get in Touch

Open to internships, collaborations, and conversations about AI integration and data projects.

- **LinkedIn:** [linkedin.com/in/sabina-ruzieva](https://www.linkedin.com/in/sabina-ruzieva/)
- **Email:** [sabinaruzieva04@gmail.com](mailto:sabinaruzieva04@gmail.com)
- **Portfolio:** in progress *(not deployed yet)*
