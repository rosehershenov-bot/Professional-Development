	1.) Install Cellfie as a plug-in on Protege. (see directions in dimension)
	2.) Download this file: cellfie_exercise_school_terms.xlsx
	3.) In “Tools”, choose “Create Axioms from Excel Workbook” (this will use Cellfie)
	4.) Choose the downloaded file above. 
	5.) Creating Transformation Rules
      To start creating transformation rules, select the Add button at the transformation rule edit panel. An editor dialog will pop up where you can type the      transformation expression.
     Enter:
     Start column: B
     End column: B
     Start row: 1
	End row: +
	In the rule box: 
	Class: @B*
    	    SubClassOf: @C*
	This means that B is a subclass of C. Indentations and spaces are important. There are four spaces before “SubclassOf:”
	Click “Generate Axioms”
	Protege/Cellfie should generate 8 axioms. 









