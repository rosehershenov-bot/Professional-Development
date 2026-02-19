# Associate-Level Protégé Exercise  
## Modeling a Role Using BFO / CCO Concepts

This exercise is designed for **Associate-level ontology engineers** in the SKS Ontology Professional Development Program. It demonstrates basic proficiency with **Protégé**, core **BFO/CCO modeling principles**, and correct handling of **roles vs. material entities**.

---

## Learning Objectives

By completing this exercise, you will demonstrate the ability to:

- Create and edit an OWL ontology in Protégé
- Create classes and object properties
- Distinguish between **material entities** and **roles**
- Apply a simple class restriction
- Add clear textual definitions
- Save, reopen, and verify an ontology file

---

## Scenario

You are modeling a **Student Role** held by a person.

In BFO/CCO-aligned modeling:

- A **Person** is a *material entity*
- A **Student Role** is a *role*
- Roles are **not subclasses of persons**
- Roles are *borne by* persons

---

## Part A — Setup

1. Open **Protégé**
2. Be sure that Protege is open under applications so you can save the ow   l file. 
3. Create a new file and save immediately. Save as "rdf-xml" syntax. 
4. Save the file as:  (your name) associate-protege-role-exercise.owl


## Part B — Create Classes

### 1. Create a `Person` class<img width="57" height="52" alt="Screenshot 2026-02-19 at 8 53 58 AM" src="https://github.com/user-attachments/assets/393533be-e7e2-48a3-886a-52e198713818" />

- Go to the **Classes** tab (under Entities)
- Create a class named `Person`: <img width="64" height="134" alt="image" src="https://github.com/user-attachments/assets/4fed0032-631f-472a-99f1-d29a4f6f0c6f" />
- Make it a subclass of `owl:Thing`

### 2. Create a `StudentRole` class
- Create a class named `StudentRole`
- Make it a subclass of `owl:Thing`

Your class hierarchy should look like:
owl:Thing
├── Person
└── StudentRole
---

## Part C — Create an Object Property

1. Go to the **Object Properties** tab
2. Create an object property named:
 bearer_of
3. Set:
- **Domain:** `Person`
- **Range:** `StudentRole`

---

## Part D — Add a Class Restriction

1. Select the **Person** class
2. Add the restriction:
   bearer_of some StudentRole
   This states that persons may bear a student role.

---

## Part E — Add Definitions

Add a textual definition using `IAO:definition` (preferred) or `rdfs:comment` if IAO is not available.

### StudentRole--add Annotation
> A student role is a role borne by a person while they are enrolled in an educational program.

### Person (optional) ---add Annotation
> A person is a human individual.

---

## Part F — Save and Verify

1. Save the ontology
2. Close Protégé
3. Reopen the file
4. Confirm:
   - Classes are present
   - Object property exists
   - Restriction is visible
   - Definitions are saved

---

## Submission Instructions

### What to Submit

1. **Ontology File**
   associate-protege-role-exercise.owl
   2. **Short Written Reflection (2–3 sentences)**
- What is a *role* in BFO terms?
- Why is `StudentRole` not a subclass of `Person`?

---

## How to Submit (GitHub Workflow)

1. Fork this repository
2. Create a new branch named:
 associate-protege-submission
3. Upload:
- Your `.owl` file
- Your reflection (Markdown or text file)
4. Open a **Pull Request** to the main branch
5. Title the PR:
  Associate Protégé Exercise – [Your Name]
  ---

## Evaluation Criteria

Submissions will be evaluated on:

- Correct class creation
- Proper distinction between material entities and roles
- Appropriate use of object properties
- Clear, accurate definitions
- Ontology opens cleanly in Protégé

---

*SKS Ontology Professional Development Program — Associate Track*
