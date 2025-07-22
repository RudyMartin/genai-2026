# Chapter 1.5: Global Regulatory Landscape - Beyond SR 11-7

## 🌍 **Making Smart Jurisdictional Choices for Banking AI**

*How to assess regulatory requirements across jurisdictions and make informed compliance decisions*

---

## **Learning Objectives**

By the end of this chapter, you will:
- Understand major international banking AI frameworks beyond SR 11-7
- Develop skills to assess which regulatory requirements apply to your situation
- Learn to make cost-effective compliance decisions across multiple jurisdictions
- Create a decision-making framework for international banking AI projects

---

## **🧭 The Jurisdictional Navigation Framework**

### **Core Decision Questions Every Analyst Must Ask:**

1. **Where does the bank operate?** (Physical presence, customers, data)
2. **What data crosses borders?** (Training data, customer data, model outputs)
3. **Who are the customers?** (Retail, corporate, institutional, cross-border)
4. **What's the business model?** (Traditional bank, digital bank, fintech, marketplace)
5. **What's the risk appetite?** (Conservative compliance vs. innovation-first)

---

## **🗺️ Major International Frameworks Overview**

### **Regulatory Philosophy Spectrum**

```
Prescriptive ←→ Principles-Based ←→ Innovation-Friendly

US (SR 11-7)     UK (FCA)     Singapore (MAS)
│                 │            │
Detailed rules    Outcomes     Regulatory sandbox
Risk tiers        Consumer     FEAT framework
Documentation     protection   Industry collaboration
```

### **Framework Comparison Table**

| **Jurisdiction** | **Key Framework** | **Philosophy** | **AI Focus** | **Enforcement Style** |
|------------------|-------------------|----------------|--------------|----------------------|
| 🇺🇸 **US** | SR 11-7 | Prescriptive | Model risk mgmt | Supervisory actions |
| 🇪🇺 **EU** | AI Act | Rights-based | Consumer protection | Heavy fines (6% revenue) |
| 🇬🇧 **UK** | PRA/FCA principles | Outcomes-focused | Fair treatment | Flexible penalties |
| 🇸🇬 **Singapore** | MAS FEAT | Innovation-friendly | Ethics & governance | Collaborative |
| 🇨🇦 **Canada** | OSFI B-13 | Risk-based | Technology risk | Graduated response |
| 🇦🇺 **Australia** | APRA CPG 234 | Prudential | Operational risk | Supervisory |

---

## **🎯 Jurisdictional Decision-Making Scenarios**

### **Scenario 1: The Global Digital Bank**

**Situation:** UK-headquartered digital bank wants to expand to US and EU markets with AI-powered credit scoring.

**Jurisdictional Analysis:**
- **UK Base:** FCA principles apply - focus on consumer outcomes
- **US Expansion:** SR 11-7 compliance required - detailed model validation
- **EU Market:** AI Act applies - high-risk AI system requiring conformity assessment

**Decision Framework:**
```
Step 1: Identify highest-risk jurisdiction → EU (AI Act penalties)
Step 2: Map overlapping requirements → All require governance + validation
Step 3: Choose compliance strategy → Build to EU standard, adapt for others
Step 4: Implementation approach → EU conformity assessment + US validation + UK outcomes testing
```

**Practical Choice:** Lead with EU AI Act compliance, then layer on SR 11-7 validation requirements and UK consumer testing.

### **Scenario 2: The Regional Bank's AI Chatbot**

**Situation:** Canadian bank wants to deploy customer service AI for account inquiries, considering US market entry.

**Jurisdictional Analysis:**
- **Canada:** OSFI B-13 technology risk framework applies
- **Potential US:** Likely Tier 3 (de minimis) under SR 11-7
- **Customer Data:** Cross-border data considerations

**Decision Framework:**
```
Risk Assessment:
- Canada: Medium risk (customer-facing, technology risk)
- US: Low risk (account inquiry only, likely Tier 3)
- Data: High importance (cross-border privacy laws)

Compliance Strategy:
- Start with Canadian technology risk assessment
- Prepare for US Tier 3 documentation
- Implement data governance for cross-border operations
```

**Practical Choice:** Implement robust Canadian framework that exceeds US Tier 3 requirements, ensuring easy US expansion.

### **Scenario 3: The Fintech's Global Expansion**

**Situation:** Singapore-based lending fintech using AI for SME credit decisions, expanding to Australia and Hong Kong.

**Jurisdictional Analysis:**
- **Singapore:** MAS FEAT framework - ethics and fairness focus
- **Australia:** APRA technology risk - operational risk emphasis
- **Hong Kong:** HKMA principles - consumer protection focus

**Decision Framework:**
```
Business Strategy Assessment:
- Core competency: AI-driven credit decisions
- Value proposition: Fast, fair, automated lending
- Risk tolerance: Moderate (fintech innovation vs. banking stability)

Regulatory Strategy:
- Singapore FEAT as baseline (home jurisdiction)
- Australia APRA overlay for operational risk
- Hong Kong consumer protection addendum
```

**Practical Choice:** Build comprehensive FEAT-compliant system with additional operational risk controls for Australia and enhanced consumer protection for Hong Kong.

---

## **🔍 Framework Deep Dives**

### **🇪🇺 European Union: The AI Act Standard**

**When It Applies:**
- Bank operates in EU
- Serves EU customers
- Uses AI systems affecting EU persons
- Processes EU personal data

**Key Requirements for Banking:**
```
High-Risk AI Systems (Credit, Insurance, etc.):
✓ Conformity assessment before deployment
✓ CE marking and technical documentation
✓ Human oversight requirements
✓ Accuracy, robustness, cybersecurity measures
✓ Transparency and explainability
✓ Record-keeping and logging systems
```

**Practical Implementation:**
- **Documentation:** Technical files, risk management system, quality management
- **Testing:** Pre-market testing, post-market monitoring
- **Governance:** Designated compliance officers, audit procedures

**Decision Trigger:** "Are we making automated decisions about EU persons that significantly affect them?"

### **🇬🇧 United Kingdom: Principles-Based Approach**

**When It Applies:**
- UK banking license
- UK customers
- UK data processing
- Cross-border services to UK

**Key Principles:**
```
Consumer Duty + Technology Risk:
✓ Good outcomes for customers
✓ Fair value and treatment
✓ Explainable decisions
✓ Operational resilience
✓ Senior manager accountability
```

**Practical Implementation:**
- **Testing:** Consumer outcome testing, fair treatment assessment
- **Documentation:** Governance arrangements, accountability mapping
- **Monitoring:** Ongoing outcomes measurement, complaints analysis

**Decision Trigger:** "Can we demonstrate good consumer outcomes and senior manager accountability?"

### **🇸🇬 Singapore: Innovation-Friendly Framework**

**When It Applies:**
- Singapore banking operations
- MAS-regulated activities
- Cross-border services from Singapore
- Regional headquarters function

**FEAT Framework:**
```
Fairness: Bias testing, fair outcomes
Ethics: Responsible AI use, societal benefit
Accountability: Clear governance, human oversight
Transparency: Explainable decisions, clear communication
```

**Practical Implementation:**
- **Self-Assessment:** FEAT questionnaire and scoring
- **Governance:** AI ethics board, responsible AI officer
- **Innovation:** Regulatory sandbox participation option

**Decision Trigger:** "How do we balance innovation with responsible AI use?"

---

## **⚖️ The Jurisdictional Choice Matrix**

### **Risk vs. Complexity Assessment**

```
                    High Regulatory Risk
                            │
Low Complexity ──────────────────────── High Complexity
     │                    │                    │
     │              US + EU + UK           Global Operation
     │              (Pick Highest          (Unified Framework
 Single Market        Standard)            + Local Variants)
     │                    │                    │
     │              Medium-High            Highest Cost
 Low Cost              Cost                Maximum Control
```

### **Decision Tree for Analysts**

```
1. Is this a HIGH-RISK AI system?
   ├─ Yes → Check EU AI Act requirements first
   └─ No → Proceed to jurisdiction analysis

2. Where will the system operate?
   ├─ Single jurisdiction → Follow local framework
   ├─ Multiple similar → Choose highest standard
   └─ Global/diverse → Unified approach + local variants

3. What's the business priority?
   ├─ Speed to market → Start with most permissive jurisdiction
   ├─ Risk minimization → Start with most restrictive
   └─ Cost optimization → Assess compliance overlap

4. What's the data situation?
   ├─ Local data only → Local framework sufficient
   ├─ Cross-border data → Consider data residency requirements
   └─ Global data sets → Unified data governance approach
```

---

## **🛠️ Practical Tools for Jurisdictional Assessment**

### **Compliance Overlap Analysis Template**

```
Requirement Category | US | EU | UK | SG | AU | Common?
Model Governance     | ✓  | ✓  | ✓  | ✓  | ✓  | YES
Independent Validation| ✓  | ~  | ~  | ~  | ~  | Partial
Conformity Assessment | ✗  | ✓  | ✗  | ✗  | ✗  | NO
Consumer Testing     | ~  | ✓  | ✓  | ✓  | ~  | Partial
Documentation       | ✓  | ✓  | ✓  | ✓  | ✓  | YES
```

### **Risk-Adjusted Compliance Strategy**

**Low-Risk Systems (Tier 3/Minimal Risk):**
- Choose most business-friendly jurisdiction as baseline
- Add minimal requirements from other jurisdictions
- Focus on operational efficiency

**Medium-Risk Systems:**
- Identify jurisdiction with most detailed guidance
- Use as foundation, adapt for others
- Balance compliance cost with business value

**High-Risk Systems:**
- Start with most restrictive requirements (often EU)
- Ensure all jurisdictions covered
- Invest in comprehensive governance framework

---

## **📋 Chapter 1.5 Practical Exercise**

### **Case Study: International Credit Scoring Platform**

**Your Assignment:** A US-based fintech is developing an AI credit scoring platform and considering expansion to:
- Canada (similar market, easier expansion)
- UK (English-speaking, large market)
- Singapore (Asia-Pacific gateway)
- Germany (EU's largest economy)

**Task:** Using the frameworks learned, recommend:
1. Which jurisdiction to launch in first and why
2. What compliance approach to take for each market
3. How to structure the development to minimize total compliance cost
4. What documentation strategy to use across jurisdictions

**Deliverable:** 2-page memo with jurisdictional analysis and implementation roadmap

---

## **🎯 Key Decision-Making Takeaways**

### **For Individual Analysts:**
1. **Always start with jurisdiction mapping** - Where does your system operate/impact?
2. **Identify the most restrictive requirement** - This often becomes your baseline
3. **Look for common requirements** - These provide efficiency opportunities
4. **Consider business strategy** - Compliance should enable, not hinder, business goals
5. **Document your reasoning** - Regulatory choice decisions should be auditable

### **For Teams and Organizations:**
1. **Develop standard frameworks** - Don't reinvent for each jurisdiction
2. **Invest in flexible architecture** - Systems should adapt to different requirements
3. **Build regulatory expertise** - Have specialists for major jurisdictions
4. **Plan for change** - Regulatory requirements evolve rapidly
5. **Consider total cost of ownership** - Include ongoing compliance, not just initial setup

---

## **🔮 Looking Ahead**

This chapter provides the foundation for making smart jurisdictional choices. In subsequent chapters, we'll see how these international perspectives play out in specific banking scenarios:

- **Chapter 2:** How credit risk validation differs across jurisdictions
- **Chapter 3:** International approaches to AML surveillance testing
- **Chapter 4:** Documentation standards that satisfy multiple regulators
- **And beyond:** How international frameworks handle fairness, explainability, and GenAI

**🤖 AI Assistant Tip:** Create a prompt template: "Given a banking AI system operating in [jurisdictions], what are the key regulatory requirements I need to consider, and what's the optimal compliance strategy?"
