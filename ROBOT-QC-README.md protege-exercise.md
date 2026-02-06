ROBOT Quality Control (QC) Exercise

This document walks you through running ROBOT to perform quality control checks on an ontology file created in Protégé.

Prerequisites
- Java installed (java -version)
- robot.jar downloaded
- An ontology file (.owl, .rdf, or .owx)
- robot.jar and your ontology file located in the same folder

Part B — Run ROBOT Validation (Report)

Step 1 — Open Terminal
On macOS:
- Press Command + Space
- Type Terminal
- Press Enter

Step 2 — Navigate to the Folder Containing Your Files
Example:
cd ~/Downloads/"Ontology practice"

Step 3 — Run ROBOT Validation (Report)
java -jar robot.jar report -i "FILE NAME.owx" -o report.tsv

This command checks for:
- Missing labels
- Missing definitions
- Missing ontology metadata
- Import or IRI problems

Step 4 — Review ROBOT Output
Example output:
Violations: 11
ERROR: 7
WARN: 4

“Report failed” means the ontology failed checks, not that ROBOT failed.

Step 5 — Open the Report File
open report.tsv

Part C — Interpret Results
Common issues:
- Missing rdfs:label
- Missing IAO:definition
- Invalid IRIs
- Import problems

Part E (Optional) — Fix and Re-run
1. Return to Protégé
2. Fix issues
3. Save file
4. Re-run ROBOT

Deliverables
- Edited ontology file
- robot-qc-report.md summary
<img width="432" height="636" alt="image" src="https://github.com/user-attachments/assets/e85cbd4a-8c74-4441-81a1-52fdc4e95de3" />
