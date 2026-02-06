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
# Part B — Run ROBOT Validation

This exercise demonstrates how to run ROBOT quality checks on an ontology file using the command line.

---

## Prerequisites

- Java installed (verify with `java -version`)
- `robot.jar` downloaded
- An ontology file created in Protégé (e.g., `.owl`, `.rdf`, or `.owx`)
- All files located in the same folder

---

## Steps

### 1. Open Terminal

On macOS:
- Press `Command + Space`
- Type **Terminal**
- Press Enter

---

### 2. Navigate to the Folder Containing Your Files

For example, if your files are in **Downloads → Ontology practice**:

```bash
cd ~/Downloads/"FILE NAME.owx "

3. Run ROBOT Validation (Report)

Use the following command (quotation marks are required if the file name has spaces):

java -jar robot.jar report -i "FILE NAME.owx" -o report.tsv

This command checks the ontology for common quality control issues such as:
	•	Missing labels
	•	Missing definitions
	•	Missing ontology metadata
	•	Import or IRI problems

4. Review ROBOT Output

ROBOT will report:
	•	Errors (must be fixed)
	•	Warnings (should be fixed)
	•	Info (optional improvements)

If you see output like:
Violations: 11
ERROR: 7
WARN: 4

This means ROBOT ran successfully and identified issues in the ontology.

Note:
“Report failed” means the ontology failed validation checks — not that ROBOT failed to run

5. Open the Report File

To view the detailed results:

Run: 
open report.tsv

This file lists each issue, the affected entity, and what is missing.

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

After completing this step, you should be able to:
	•	Run ROBOT from the command line
	•	Generate a QC report
	•	Identify missing labels, definitions, and metadata
	•	Fix issues in Protégé and rerun ROBOT



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
