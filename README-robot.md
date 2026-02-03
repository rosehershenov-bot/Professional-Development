# Associate-Level Exercise: From Protégé to ROBOT

## Purpose

This exercise connects **ontology editing in Protégé** with **quality control using ROBOT**.  
You will:
1. Create or edit ontology content in Protégé (See Protege Readme)
2. Save it as an OWL file
3. Use ROBOT to validate and report on that file


---

## Learning Objectives

By completing this exercise, you will be able to:

- Create or modify ontology content in Protégé
- Save a valid OWL file
- Run ROBOT validation on that file
- Identify missing labels or definitions
- Explain QC results in plain language

---

## Prerequisites

- Protégé installed and working
- ROBOT installed and runnable from Terminal:
  ```bash
  robot --version
  	•	A basic understanding of:
	•	Class
	•	Annotation (e.g., label, definition)
  Part A — Protégé Modeling Task

Step 1: Open Protégé
	•	Open your existing ontology or create a new ontology.
	•	Ensure it is saved locally as an .owl file.

Step 2: Create a Class
	•	Create a new class under owl:Thing
	•	Example (you may choose your own domain term):
	•	MedicalVisit
	•	PatientRole
	•	VaccinationProcess

Step 3: Add Annotations

For your new class, add (See Protege README)
	•	rdfs:label (human-readable name)
	•	A definition annotation
	•	If available: IAO:definition
	•	Otherwise: rdfs:comment

Save the ontology file.

⸻

Part B — Run ROBOT Validation

Open Terminal and navigate to the folder containing your OWL file.

Run:
robot validate --input YOUR_FILE.owl
Example: 
robot validate --input associate-protege.owl

Part C — Review ROBOT Output

Observe whether ROBOT reports:
	•	Errors
	•	Warnings
	•	No issues

Common issues include:
	•	Missing labels
	•	Missing definitions
	•	Invalid IRIs
	•	Import problems

⸻

Part D — Create a QC Report

Create a file called:

robot-qc-report.md

Required Content
	•	The ROBOT command you ran
	•	The ontology file name
	•	The date
	•	ROBOT output (copy/paste or summarized)

Short Answers
	1.	Did ROBOT report any issues?
	2.	If yes, name one issue and explain what it means.
	3.	If no issues, explain why you think the file passed validation.

⸻

Part E (Optional) — Fix and Re-run

If ROBOT reports an issue:
	1.	Return to Protégé
	2.	Fix the issue (e.g., add a missing label or definition)
	3.	Save the OWL file
	4.	Re-run:
  robot validate --input YOUR_FILE.owl

  Deliverables

Submit:
	1.	The OWL file you edited in Protégé
	2.	robot-qc-report.md
