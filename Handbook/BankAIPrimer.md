

## 📘 **Title:**

**AI Testing in Banking: A Hands-On Guide to Model Governance and SR 11-7 Compliance**

**Subtitle:**
From credit risk to generative AI, this guide teaches how to test, validate, and document models with banking regulators in mind.

---

## 🧠 **Book Structure (Teaching Guide Format)**

Each chapter has:

* **IconBook** visual reference
* **Real-world banking scenario**
* **Test method**
* **SR 11-7 compliance takeaway**
* **AI Assistant Tip** (optional: prompt, script, or checklist)

---

### 📘 Chapter 1: Credit Risk Models — Cross-Validation in Action

**Scenario:** Auto loan underwriting
**Test:** k-fold cross-validation across FICO bands
**Goal:** Avoid overfitting; ensure segment generalization
**SR 11-7 Tag:** Model Development | Documentation
**AI Assistant Tip:** Prompt GPT to explain "train/test split vs. CV using borrower segments"

---

### 📘 Chapter 2: AML Surveillance — Classification Accuracy Testing

**Scenario:** Flagging suspicious wire transfers
**Test:** Confusion matrix, ROC, precision/recall
**Goal:** Minimize false negatives (undetected laundering)
**SR 11-7 Tag:** Threshold Calibration | Monitoring
**AI Assistant Tip:** Use GPT to auto-summarize alert types and misclassification causes

---

### 📘 Chapter 3: Model Explainability — Feature Importance Analysis

**Scenario:** Mortgage loan approvals
**Test:** SHAP values to evaluate input weight (LTV, DTI)
**Goal:** Support regulatory explainability
**SR 11-7 Tag:** Governance | Documentation
**AI Assistant Tip:** Generate a SHAP summary chart with auto-annotated drivers

---

### 📘 Chapter 4: Fraud Risk — Robustness Under Attack

**Scenario:** Credit card fraud detection
**Test:** Input perturbation, adversarial stress test
**Goal:** Validate model performance under degraded inputs
**SR 11-7 Tag:** Limitations Testing
**AI Assistant Tip:** Prompt model to simulate edge cases like duplicate transactions or out-of-sequence data

---

### 📘 Chapter 5: Monitoring Credit Trends — Temporal Stability Testing

**Scenario:** Small business loan default forecasting
**Test:** PSI (Population Stability Index), KS drift
**Goal:** Detect input/output drift over time
**SR 11-7 Tag:** Ongoing Monitoring
**AI Assistant Tip:** Use GPT to write drift monitoring SQL scripts and trend graphs

---

### 📘 Chapter 6: Light-touch AI — De Minimis Testing Protocols

**Scenario:** Internal NLP for tagging 10-K documents
**Test:** Basic accuracy and minimal validation logs
**Goal:** Document that model is low-risk Tier 3
**SR 11-7 Tag:** Risk Tiering | Minimal Oversight
**AI Assistant Tip:** Auto-generate a de minimis declaration memo for model registry

---

### 📘 Chapter 7: Fairness Testing — Preventing Discrimination

**Scenario:** Personal loan approvals
**Test:** Adverse impact ratio, disparate impact tests
**Goal:** Ensure fairness across race/gender segments
**SR 11-7 Tag:** Regulatory Compliance | Fair Lending
**AI Assistant Tip:** Prompt LLM to review output by protected class and flag disparities

---

### 📘 Chapter 8: Generative AI — LLM Accuracy Validation

**Scenario:** Banking chatbot for customer balance inquiries
**Test:** Answer correctness across benchmark set
**Goal:** Avoid hallucinations and compliance misstatements
**SR 11-7 Tag:** Output Validation | QA Logs
**AI Assistant Tip:** Fine-tune GPT to respond only with structured account info or deferral to human

---

### 📘 Chapter 9: Red Teaming AI — LLM Safety, Harm, and Privacy

**Scenario:** Mortgage pre-qualification assistant
**Test:** Prompt injection, restricted word handling, private data leakage test
**Goal:** Ensure no harmful or unauthorized advice is generated
**SR 11-7 Tag:** Control Environment | Risk Mitigation
**AI Assistant Tip:** Generate a “forbidden topics” prompt filter and testing suite

---

## 🔖 Bonus Chapter:

**Build Your Own Testing Suite**

* GPT prompts for documentation
* SQL templates for monitoring
* Checklists for MRM audit prep

---




