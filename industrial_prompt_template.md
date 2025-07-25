# Industrial-Grade Prompt Template
## 20 Element Framework for Professional AI Engineering

*Version 2.0 | Created for token efficiency and cross-model compatibility*

---

## 🎯 CORE SPECIFICATION (Elements 1-13)
*Essential for every prompt - start here*

### **1. PROMPT ID**
**Purpose**: Version tracking like software development  
**Format**: Domain-Function-Version (e.g., HR-RECRUIT-003)  
**Examples**:
- `FIN-ANALYSIS-012` - Financial analysis, 12th iteration
- `COMMS-CRISIS-001` - Crisis communication, first version
- `DATA-ANOMALY-005` - Anomaly detection, version 5

**Replace with your ID**: `[YOUR-DOMAIN-FUNCTION-VERSION]`

---

### **2. PURPOSE** 
**Purpose**: Strategic "why" - clear objective beyond "do something"  
**Missing from typical frameworks**: Most never ask WHY you're doing this  

**Template**: 
```
To [SPECIFIC GOAL] in order to [BUSINESS OUTCOME] by [METHOD/APPROACH]
```

**Examples**:
- To identify fraud risks in transaction data in order to prevent financial losses by statistical anomaly detection
- To explain complex technical concepts in order to enable non-expert decision-making by structured simplification
- To optimize resource allocation in order to reduce costs by 15% by data-driven recommendations

**Replace with your purpose**: `[YOUR SPECIFIC GOAL AND BUSINESS OUTCOME]`

---

### **3. CONTEXT**
**Purpose**: Environmental awareness - where the AI operates  
**Not just**: Background information  

**Template**:
```
Organization: [TYPE, SIZE, INDUSTRY]
Environment: [REGULATORY/CULTURAL/TECHNICAL CONSTRAINTS]  
Stakeholders: [WHO WILL USE/BE AFFECTED BY RESULTS]
Timeline: [URGENCY/DECISION DEADLINES]
```

**Example**:
```
Organization: Mid-size aviation company, 200 employees, GDPR compliance required
Environment: Regulated industry, risk-averse culture, first AI implementation
Stakeholders: Risk managers, compliance officers, executive leadership
Timeline: Monthly reporting cycle, decisions needed within 48 hours
```

**Replace with your context**: `[YOUR ORGANIZATIONAL AND ENVIRONMENTAL CONTEXT]`

---

### **4. SYSTEM INSTRUCTION**
**Purpose**: Intelligent persona activation - not generic "expert for everything"  
**Avoid**: Fantasy roles like "successful billionaire entrepreneur"  
**Focus**: Relevant, specific expertise

**Template**:
```
Adopt the perspective of [SPECIFIC ROLE] with [YEARS] years experience in [DOMAIN].
Prioritize [KEY SKILLS/APPROACHES] when analyzing problems.
Consider [SPECIFIC CONSTRAINTS/STANDARDS] in all recommendations.
```

**Examples**:
- Adopt the perspective of a senior fraud analyst with 10+ years experience in aviation finance. Prioritize statistical rigor and regulatory compliance when analyzing transaction patterns.
- Act as a change management consultant with 15+ years experience in digital transformations. Consider stakeholder psychology and organizational culture in all recommendations.

**Replace with your role**: `[YOUR SPECIFIC EXPERT PERSPECTIVE]`

---

### **5. INSTRUCTION**
**Purpose**: Concrete, executable action commands  
**Structure**: Verb + Object + Method + Success Criteria  

**Template**:
```
[ACTION VERB] the [INPUT OBJECT] by [METHOD/APPROACH].
Prioritize results by [CRITERIA].
Ensure outputs meet [QUALITY STANDARDS].
If [CONDITION], then [ALTERNATIVE ACTION].
```

**Examples**:
- Analyze the transaction dataset using statistical outlier detection. Prioritize results by potential financial impact. Ensure all flagged items include confidence scores above 80%.
- Create a 3-phase implementation plan using change management best practices. Prioritize quick wins in phase 1. Ensure each phase has measurable success metrics.

**Replace with your instructions**: `[YOUR SPECIFIC ACTION COMMANDS]`

---

### **6. USER INPUT EXPECTATION**
**Purpose**: Clear expectations about what you'll provide  
**Prevents**: "I don't know what to input" frustration  

**Template**:
```
Required inputs:
- [INPUT TYPE 1]: [FORMAT, SIZE LIMITS, REQUIRED FIELDS]
- [INPUT TYPE 2]: [FORMAT, SIZE LIMITS, REQUIRED FIELDS]

Optional inputs:
- [OPTIONAL INPUT]: [WHEN USEFUL, FORMAT]
```

**Example**:
```
Required inputs:
- Transaction data: CSV format, max 10,000 rows, fields: TransactionID, Amount, Timestamp, UserID
- Analysis timeframe: Date range in YYYY-MM-DD format

Optional inputs:
- Historical baseline: Previous month's data for comparison
- Risk tolerance: High/Medium/Low preference for sensitivity
```

**Replace with your input requirements**: `[YOUR INPUT SPECIFICATIONS]`

---

### **7. OUTPUT FORMAT**
**Purpose**: Structure requirements for usable results  
**Consider**: Who reads it? How will it be used?  

**Template**:
```
Primary format: [STRUCTURE TYPE]
Length: [WORD/CHARACTER LIMITS]
Sections: [REQUIRED COMPONENTS]
Tone: [PROFESSIONAL LEVEL]
Special requirements: [CHARTS, LINKS, CITATIONS, ETC.]
```

**Examples**:
- Primary format: Executive summary (max 200 words) + detailed analysis + 3 prioritized recommendations
- Length: Email-appropriate, under 300 words total
- Sections: Problem statement, key findings, immediate actions required
- Tone: Professional but accessible to non-technical stakeholders

**Replace with your format needs**: `[YOUR OUTPUT STRUCTURE REQUIREMENTS]`

---

### **8. EXECUTION PARAMETERS**
**Purpose**: Controls AI engine behavior  
**Key parameter**: Temperature (creativity vs. consistency)  

**Temperature Guidelines**:
- `0.1` - Facts, compliance, numbers (minimal creativity)
- `0.3` - Technical analysis, balanced recommendations  
- `0.7` - Strategic planning, creative problem-solving
- `0.9` - Innovation, brainstorming, maximum creativity

**Template**:
```
Temperature: [0.1-0.9]
Response style: [ANALYTICAL/CREATIVE/BALANCED]
Risk tolerance: [CONSERVATIVE/MODERATE/AGGRESSIVE]
```

**Replace with your parameters**: `Temperature: [YOUR TEMPERATURE SETTING]`

---

### **9. FEW-SHOT EXAMPLES**
**Purpose**: Shows AI exactly what you want  
**Format**: Input → Desired Output  
**Optimal number**: 2-3 examples  

**Template**:
```
Example 1:
Input: [SAMPLE INPUT 1]
Expected Output: [IDEAL RESPONSE 1]

Example 2:
Input: [SAMPLE INPUT 2]  
Expected Output: [IDEAL RESPONSE 2]
```

**Example**:
```
Example 1:
Input: "Transaction: €5,000, 23:47, Gas Station"
Expected Output: "RISK ANALYSIS: Medium risk - unusual time for high amount, gas station context plausible, recommend manual review"

Example 2:
Input: "Transaction: €50, 14:30, Supermarket"
Expected Output: "RISK ANALYSIS: Low risk - normal amount, normal time, typical context"
```

**Replace with your examples**: `[YOUR INPUT/OUTPUT EXAMPLES]`

---

### **10. NOTES**
**Purpose**: Learning diary for continuous improvement  
**Content**: What works, what doesn't, why  

**Template**:
```
Version history:
- v[X.X]: [CHANGE MADE] - [REASON] - [RESULT]

Known limitations:
- [LIMITATION 1]: [WORKAROUND]
- [LIMITATION 2]: [MITIGATION]

Optimization ideas:
- [FUTURE IMPROVEMENT]: [EXPECTED BENEFIT]
```

**Replace with your notes**: `[YOUR LEARNING OBSERVATIONS]`

---

### **11. MODEL**
**Purpose**: Target AI systems (different models have different strengths)  
**Important**: What works on ChatGPT may not work on Claude  

**Template**:
```
Primary model: [MODEL NAME AND VERSION]
Tested on: [ADDITIONAL MODELS]
Model-specific notes: [PERFORMANCE DIFFERENCES]
```

**Examples**:
- Primary model: Claude Sonnet 4 (best for complex analysis)
- Tested on: ChatGPT-4o (good for communication), Gemini Pro (multimodal)
- Model-specific notes: Claude better for logical reasoning, ChatGPT better for creative communication

**Replace with your model preferences**: `[YOUR TARGET AI MODELS]`

---

### **12. VERSION/CREATION/MODIFIED**
**Purpose**: Lifecycle tracking and accountability  
**Format**: Semantic versioning (1.0, 1.1, 2.0)  

**Template**:
```
Version: [X.X]
Created: [DATE] by [PERSON]
Last modified: [DATE] by [PERSON]
Change log: [SUMMARY OF CHANGES]
```

**Replace with your version info**: `[YOUR VERSION DETAILS]`

---

### **13. METADATA**
**Purpose**: Taxonomic organization for team findability  

**Template**:
```
Tags: [KEYWORD1, KEYWORD2, KEYWORD3]
Category: [BUSINESS-FUNCTION/SUB-FUNCTION]
Target audience: [USER ROLES]
Language: [LANGUAGE CODE]
Compliance level: [REGULATORY REQUIREMENTS]
```

**Replace with your metadata**: `[YOUR CLASSIFICATION TAGS]`

---

## 🔧 PROFESSIONAL EXTENSIONS (Elements 14-20)
*Advanced elements for enterprise deployment*

### **14. VALIDATION CRITERIA**
**Purpose**: Objective success measurement  
**Measurable**: Not "good" but "90% accuracy"  

**Template**:
```
Success metrics:
- [METRIC 1]: [TARGET VALUE] (e.g., 85% accuracy)
- [METRIC 2]: [TARGET VALUE] (e.g., <30 second response time)

Quality checks:
- [CHECK 1]: [VERIFICATION METHOD]
- [CHECK 2]: [VERIFICATION METHOD]
```

**Replace with your success criteria**: `[YOUR MEASURABLE OUTCOMES]`

---

### **15. ERROR HANDLING**
**Purpose**: Failure recovery strategies  
**Common issues**: Hallucination, misunderstanding, technical errors  

**Template**:
```
If [ERROR CONDITION 1], then [RECOVERY ACTION 1]
If [ERROR CONDITION 2], then [RECOVERY ACTION 2]
Escalation: When to involve humans vs. automated retry
```

**Replace with your error strategies**: `[YOUR FAILURE RECOVERY PLANS]`

---

### **16. DEPENDENCIES**
**Purpose**: Prerequisites and assumptions  
**Categories**: Data, knowledge, tools, access rights  

**Template**:
```
Required:
- [DEPENDENCY 1]: [DESCRIPTION]
- [DEPENDENCY 2]: [DESCRIPTION]

Assumptions:
- [ASSUMPTION 1]: [RISK IF INVALID]
- [ASSUMPTION 2]: [RISK IF INVALID]
```

**Replace with your dependencies**: `[YOUR PREREQUISITES]`

---

### **17. ITERATION STRATEGY**
**Purpose**: Systematic improvement path  
**Not**: Trial-and-error  

**Template**:
```
Improvement cycle: [FREQUENCY] (e.g., monthly)
Feedback sources: [WHO PROVIDES INPUT]
A/B testing plan: [WHAT TO TEST]
Success measurement: [HOW TO MEASURE IMPROVEMENT]
```

**Replace with your improvement plan**: `[YOUR ITERATION APPROACH]`

---

### **18. RISK ASSESSMENT**
**Purpose**: Failure modes and damage mitigation  
**Categories**: Technical, business, legal, reputational risks  

**Template**:
```
High risk: [RISK 1] → Mitigation: [STRATEGY 1]
Medium risk: [RISK 2] → Mitigation: [STRATEGY 2]
Low risk: [RISK 3] → Mitigation: [STRATEGY 3]
```

**Replace with your risk analysis**: `[YOUR RISK MITIGATION STRATEGIES]`

---

### **19. PERFORMANCE METRICS**
**Purpose**: Continuous performance monitoring  
**Types**: Quality, speed, user satisfaction, cost efficiency  

**Template**:
```
Quality: [ACCURACY METRIC] (target: [VALUE])
Speed: [RESPONSE TIME METRIC] (target: [VALUE])  
Satisfaction: [USER FEEDBACK METRIC] (target: [VALUE])
Efficiency: [COST/TIME SAVINGS] (target: [VALUE])
```

**Replace with your metrics**: `[YOUR PERFORMANCE INDICATORS]`

---

### **20. INTEGRATION POINTS**
**Purpose**: System connections and workflows  
**Aspects**: APIs, data flows, user workflows, other prompts  

**Template**:
```
Input sources: [WHERE DATA COMES FROM]
Output destinations: [WHERE RESULTS GO]
Workflow position: [STEP X OF Y IN PROCESS]
Dependencies: [OTHER PROMPTS/SYSTEMS NEEDED]
```

**Replace with your integration needs**: `[YOUR SYSTEM CONNECTIONS]`

---

## 🚀 IMPLEMENTATION GUIDELINES

### **Start Simple (Elements 1-9)**
For individual/pilot use, focus on the core elements first.

### **Scale Systematically (Elements 10-13)**  
Add documentation and versioning when sharing with team.

### **Enterprise Ready (Elements 14-20)**
Include all elements for production deployment and compliance requirements.

### **Token Efficiency Notes**
- Write in **English** for optimal token utilization
- Use **Markdown** formatting for structure recognition  
- Keep **Few-Shot Examples** concise but specific
- Test **Temperature** settings empirically for your use case

---

*This template transforms prompt engineering from art to engineering discipline.*

**Framework Status**: Anti-fragile | Gets stronger with real-world stress testing  
**Last Updated**: Version 2.0 | Optimized for professional AI deployment