

## 🏦 Banking-Specific Use Cases of Model Testing under SR 11-7

> Each of the tests below is now paired with **a real-world banking use case** and its link to **regulatory expectations** under SR 11-7, including **validation**, **ongoing monitoring**, and **governance** requirements.

---

### 1. 🔁 **Cross-Validation**

**Use Case:** Credit Risk Scorecard for Auto Loans
**SR 11-7 Focus:** *Development & Independent Validation*

* **Why It Matters:** Prevents overfitting to past borrower profiles.
* **Example:** Use stratified k-fold cross-validation by credit tiers (prime, subprime).
* **Audit Note:** Cross-validation results must be documented in model development files reviewed during MRM validation.

---

### 2. 📈 **Classification Accuracy Testing**

**Use Case:** Anti-Money Laundering (AML) Transaction Monitoring
**SR 11-7 Focus:** *Performance Monitoring & Threshold Calibration*

* **Why It Matters:** False negatives (missed suspicious activity) are regulatory red flags.
* **Example:** Test precision/recall tradeoffs at different alert thresholds.
* **Audit Note:** Must demonstrate alerting system has been tested across customer segments and doesn’t degrade over time.

---

### 3. 📊 **Feature Importance Testing**

**Use Case:** Mortgage Approval Models (FICO, LTV, DTI inputs)
**SR 11-7 Focus:** *Transparency, Documentation, & Explainability*

* **Why It Matters:** Stakeholders (e.g., compliance, model audit, fair lending) must understand what drives approvals/denials.
* **Example:** SHAP values or model cards showing that LTV is the dominant predictor, not zip code.
* **Audit Note:** Models must not use prohibited features or proxies for protected classes (e.g., race, gender).

---

### 4. 🛡️ **Robustness Testing**

**Use Case:** Fraud Detection During System Outage
**SR 11-7 Focus:** *Limitations & Assumptions Testing*

* **Why It Matters:** Inputs may be missing or delayed during system disruptions.
* **Example:** Remove or perturb real-time features (e.g., login time) and measure fraud detection degradation.
* **Audit Note:** Model validation report should explicitly describe how missing data or unusual behavior is handled.

---

### 5. ⏳ **Temporal Stability Testing**

**Use Case:** Small Business Loan Default Forecasting
**SR 11-7 Focus:** *Ongoing Monitoring & Model Drift Detection*

* **Why It Matters:** Economic shocks (e.g., pandemic, interest rate hikes) alter borrower behavior.
* **Example:** Monitor model accuracy quarterly; use PSI (Population Stability Index) to flag input shifts.
* **Audit Note:** Include stability metrics in quarterly monitoring pack; document response if drift is detected.

---

### 6. 🧮 **De Minimis AI/ML Testing**

**Use Case:** Internal NLP model for tagging regulatory filings
**SR 11-7 Focus:** *Tiered Model Governance*

* **Why It Matters:** Even non-customer-facing models must be risk-tiered appropriately.
* **Example:** Classify model as Tier 3 (“low impact”) and perform basic accuracy check with manual QA.
* **Audit Note:** Maintain documentation justifying de minimis designation and minimal validation scope.

---

### 7. 🤖 **LLM Accuracy Testing**

**Use Case:** Customer Support Chatbot for Account Balance Inquiries
**SR 11-7 Focus:** *Fit-for-Purpose Testing, Ongoing Monitoring*

* **Why It Matters:** Incorrect answers on balances or interest rates can trigger compliance issues.
* **Example:** Run a benchmark test set of queries; check answer correctness and hallucination rate.
* **Audit Note:** LLM outputs must be version-controlled and evaluated routinely for drift or hallucination patterns.

---

### 8. 🔐 **LLM Harm/Safety Testing**

**Use Case:** Generative AI assistant helping with mortgage pre-approval questions
**SR 11-7 Focus:** *Control Environment & Risk Mitigation*

* **Why It Matters:** Model may generate misleading guidance on regulatory disclosures (e.g., APR, Fair Lending).
* **Example:** Prompt injection and red-teaming tests to simulate adversarial misuse.
* **Audit Note:** Results must feed into the control framework; testing logs should show harmful prompts blocked or flagged.

---

### 9. ⚖️ **Fairness and Discrimination Testing**

**Use Case:** Personal Loan Underwriting Model
**SR 11-7 Focus:** *Legal & Regulatory Compliance, Fair Lending*

* **Why It Matters:** Models must not exhibit disparate impact against protected groups.
* **Example:** Use disparity metrics (e.g., equal opportunity difference, adverse impact ratio).
* **Audit Note:** Validation team must assess whether model exhibits statistical bias, even if inputs are facially neutral.

---

### ✅ Bonus: Suggested MRM Documentation Table

| **Test**           | **Banking Use Case**          | **SR 11-7 Focus Area**          | **Artifact for Audit**                  |
| ------------------ | ----------------------------- | ------------------------------- | --------------------------------------- |
| Cross-Validation   | Auto Loan Credit Risk         | Development, Validation         | CV methodology & score distribution     |
| Accuracy Testing   | AML Monitoring                | Alert Calibration, Monitoring   | Confusion matrix, threshold curves      |
| Feature Importance | Mortgage Underwriting         | Explainability, Governance      | SHAP summary, feature control log       |
| Robustness Testing | Fraud Detection               | Limitations Testing             | Perturbation test log                   |
| Temporal Stability | SMB Lending                   | Drift & Monitoring              | PSI trends, drift response record       |
| De Minimis Testing | Internal NLP                  | Tiering, Lightweight Validation | Tier 3 classification memo              |
| LLM Accuracy       | Chatbot for Balance Inquiry   | Fit-for-Purpose, QA             | Accuracy logs, benchmark tests          |
| LLM Harm/Safety    | Generative Mortgage Assistant | Red Teaming, Control Framework  | Prompt test logs, filtered response set |
| Fairness Testing   | Personal Loan Decisions       | Fair Lending Compliance         | Disparity metrics, compliance signoff   |

---

## 🛠 Next Steps?

Options:

* ✅ SR 11-7 compliant **model testing checklists**
* ✅ Sample **validation report templates**
* ✅ Risk-tiering matrix (for Tier 1–3 models)
* ✅ Internal audit log examples for LLM output QA

