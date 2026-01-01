# Exercise: Applying a BFO–CCO Design Pattern  
**Associate-Level Ontology Engineering**

## Purpose
This exercise assesses the ability to correctly apply **BFO–CCO standards** and **existing design patterns**, using the approved checklist to guide modeling decisions.

---

## Scenario

You are asked to model information about a **person and their birth date** for an enterprise knowledge graph.

**Requirement:**
> “We need to represent when a person was born so that the information can be reused and queried consistently across systems.”

---

## Task Instructions

### Step 1: Identify the Modeling Problem
In 1–2 sentences, answer:
- What kind of entity is a **birth** in BFO terms?
- Why is birth not best represented as a direct data property of a person?

---

### Step 2: Identify the Appropriate Design Pattern
- Locate an existing **CCO or CUBRC design pattern** relevant to birth or life events.
- Briefly describe:
  - The main entities involved
  - Where temporal (date/time) information is represented

---

### Step 3: Apply the Pattern
Describe your model using text, simple diagrams, or OWL (as assigned):

Your model should include:
- A **Person**
- A **Birth Process**
- The correct relationship between the person and the birth process
- Temporal information associated with the process

Do **not** invent new properties or structures.

---

### Step 4: Checklist Confirmation
Use the **BFO–CCO Design Pattern Application Checklist** and check all applicable items.

---

### Step 5: Reflection
In 3–5 sentences, explain:
- Why reusing an existing design pattern is preferable to creating a custom solution
- How this modeling choice supports interoperability and reuse

---

## Deliverables
Submit:
- Written responses for Steps 1–3
- Completed checklist
- Reflection paragraph

---

## Graded Rubric (Associate Level)

| Criterion | Exemplary (3) | Proficient (2) | Developing (1) | Not Demonstrated (0) |
|---------|----------------|----------------|----------------|---------------------|
| **BFO Classification** | Correctly identifies birth as a process and explains why | Identifies birth as a process with minimal explanation | Partial or unclear identification | Incorrect classification |
| **Pattern Identification** | Correctly identifies an existing CCO/CUBRC pattern | Identifies a relevant pattern with minor gaps | Mentions a pattern but lacks clarity | No pattern identified |
| **Pattern Application** | Applies the pattern correctly with no structural errors | Applies pattern with minor issues | Significant deviations from pattern | Invents custom structure |
| **Temporal Modeling** | Correctly attaches time to the process | Mostly correct with minor confusion | Misplaced or unclear temporal info | Incorrect temporal modeling |
| **Checklist Use** | Checklist fully and thoughtfully applied | Checklist used with minor omissions | Checklist partially used | Checklist not used |
| **Reflection & Justification** | Clearly explains why the pattern is correct | Explanation is mostly clear | Superficial explanation | No justification |

### Scoring Guide
- **15–18 points:** Proficient — Meets associate-level expectations  
- **10–14 points:** Developing — Needs targeted feedback  
- **0–9 points:** Not Yet Ready — Requires remediation

---

## Associate-Level Success Criteria
An associate demonstrates readiness when they:
- Reuse existing BFO–CCO patterns without modification
- Avoid modeling dates as properties of continuants
- Can explain modeling choices in plain language
- Use the checklist as a validation tool

---

*This exercise is part of the SKS Ontology Professional Development Program and aligns with associate-level modeling competencies.*
