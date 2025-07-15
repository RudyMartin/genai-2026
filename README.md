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
Absolutely — here's a clear **Week-by-Week Breakdown** of **Key Outputs**, **per Agent**, for the unified **MVP1** plan:

---

## ✅ **MVP1 Key Outputs by Week**

*Automated Documentation Preview Agent* + *Automated Jira-Support Triage Agent*

| **Week** | **DocPreviewAgent (📄)**                                                                               | **JiraTriageAgent (🛠️)**                                                                           |
| -------- | ------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| **1**    | • Use cases defined (MRA, model plans, audit docs)<br>• Output spec: preview format, flags, highlights | • Target queues and routing rules confirmed<br>• Output spec: assignment logic, comment suggestions |
| **2**    | • Ingestion script for PDFs/DOCX<br>• Text + metadata JSON structure                                   | • Jira API connector built<br>• Normalized ticket JSONs with comments, status, labels               |
| **3**    | • `DocPreviewAgent` scaffold with DSPy or LangChain<br>• Modular chunking logic                        | • `JiraTriageAgent` scaffold<br>• Ticket data loader + preprocessing                                |
| **4**    | • Titan v2 embedding of document chunks<br>• FAISS/pgVector index saved by doc type                    | • Titan v2 embedding of ticket history + body<br>• FAISS/pgVector index saved by issue type         |
| **5**    | • Retrieval block returns top-k doc chunks<br>• Initial DSPy prompt: summarize + flag risks            | • Retrieval block returns similar past tickets<br>• Initial DSPy prompt: classify + assign + draft  |
| **6**    | • Evaluation run: 10+ sample docs<br>• Logs: preview accuracy, risk flag quality                       | • Evaluation run: 30+ sample tickets<br>• Logs: routing accuracy, label match, comment usefulness   |
| **7**    | • Preview interface (Streamlit/CLI)<br>• Output: HTML/JSON summary for each doc                        | • CLI/Streamlit UI to enter ticket ID<br>• Output: assignment, comment, escalation flag             |
| **8**    | • Feedback buttons for: incorrect preview, missing risk<br>• Full context/output logging               | • Feedback logging: misroute, bad comment<br>• Run trace stored per ticket                          |
| **9**    | • Internal pilot with 3–5 users<br>• Preview quality rated by doc type                                 | • Pilot live on test Jira queue<br>• Feedback: usefulness, error types, timing                      |
| **10**   | • Hardened version deployed<br>• Optional: batch doc audit script + dashboard                          | • Agent live with retry logic<br>• Optional: auto-comment or label suggestions via API              |

---

### 🔁 Final Artifacts (End of Week 10)

* 🧠 **Two modular agents**: `DocPreviewAgent`, `JiraTriageAgent`
* 💾 **Two embedding stores**: documents vs. tickets
* 🛠️ **Retrieval + DSPy pipelines** shared and abstracted
* 📊 **Eval logs**, **feedback dashboard**, **pilot report**
* 🔄 **Deployment-ready**: callable UI/API + reindex jobs



