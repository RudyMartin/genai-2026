## ✅ **MVP1: Automated Text Intelligence Agents**

### 🎯 Objective: Deploy two text-based agents that accelerate operational workflows

* **Agent 1:** 📄 **Documentation Preview Agent** – surface summaries, issues, and flags from risk-related documents.
* **Agent 2:** 🛠️ **Jira Support Triage Agent** – route, tag, and comment on tickets based on historical and contextual patterns.

---

## 🗂️ **Unified 10-Week MVP1 Action Plan**

### **🔹 Week 1 – MVP Kickoff**

* Align with Sonia's team: define **risk doc types** (e.g., model plans, issue logs), and **Jira queues**.
* Establish MVP1 success criteria (e.g., % triaged correctly, preview coverage, response time).
* Confirm target platforms: S3, Bedrock, Jira API, internal Confluence.

---

### **🔹 Week 2 – Ingest & Normalize Inputs**

* Build ingestion module:

  * PDFs + DOCX → text chunks
  * Jira API → ticket content + metadata
* Normalize to common schema: `{"source_type": ..., "text": ..., "meta": {...}}`

---

### **🔹 Week 3 – MVP Agent Templates**

* Draft shared `AgentBase()` class or wrapper (DSPy or LangChain):

  * Handles chunking, embedding, retrieval, prompting, output formatting.
* Create separate subclasses for:

  * `DocPreviewAgent()`
  * `JiraTriageAgent()`

---

### **🔹 Week 4 – Embedding + Index**

* Use **Bedrock Titan v2** or Claude v2 embeddings for both agents.
* Create modular FAISS/pgVector indexer.
* Enable per-agent reindexing (doc vs ticket context buckets).

---

### **🔹 Week 5 – Retrieval + Prompting**

* Create reusable retrieval block (by source type).
* Write DSPy chains or prompt templates:

  * For docs: highlight compliance risk, summarize preview
  * For Jira: classify issue, assign owner, suggest comment

---

### **🔹 Week 6 – Agent Tuning & Sample Runs**

* Run both agents on test set:

  * 10+ documents (doc preview)
  * 30+ Jira tickets (triage)
* Log: retrieved context, output, next action
* Adjust few-shot examples + chunk sizes

---

### **🔹 Week 7 – MVP UI + API Integration**

* Build simple UI (Streamlit or CLI):

  * Upload or select doc → preview output
  * Enter Jira ID → triage result
* Add Slack/Jira API integration for testing updates

---

### **🔹 Week 8 – Logging, Feedback, Audit Trail**

* Add feedback flagging for:

  * Incorrect preview
  * Misrouted ticket
* Log full run context: input, retrieved, output, user correction

---

### **🔹 Week 9 – Internal Pilot**

* Deploy both agents internally (passworded or local link).
* Invite 3–5 testers from risk + support teams.
* Gather evaluation:

  * 📄 Document Agent: Preview relevance, usability
  * 🛠️ Jira Agent: Routing accuracy, comment usefulness

---

### **🔹 Week 10 – Production Launch of MVP1**

* Harden both agents:

  * Retry logic, missing data fallback, batch mode
* Deploy final containerized version
* Deliver internal dashboard or update report
* MVP1 ✅ complete — ready for next-phase proposal

---

## 🔗 MVP1 System Diagram

```
       ┌───────────────────────────────┐
       │         MVP1 Core Agent       │
       │    (shared retrieval + LLM)   │
       └────────────┬──────────────────┘
                    │
      ┌─────────────┴─────────────┐
      ▼                           ▼
┌───────────-───---┐       ┌─────────────--─────┐
│ DocPreviewAgent  │       │ JiraTriageAgent    │
│ - PDF → Chunks   │       │ - Ticket Text →    │
│ - Risk Flagging  │       │   Class/Assign     │
│ - Preview Output │       │ - Comment Drafting │
└────────────----──┘       └──────────==────────┘
```

