Install Cellfie as a plug-in on Protege. (see directions in dimension)
Download this file: cellfie_exercise_school_terms.xlsx
In “Tools”, choose “Create Axioms from Excel Workbook” (this will use Cellfie)
Choose the downloaded file above. 
Creating Transformation Rules
To start creating transformation rules, select the Add button at the transformation rule edit panel. An editor dialog will pop up where you can type the transformation expression.
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
Your log should look like this: 
Date: The date
# Cell range: (Terms!B2:B5) Comment: ""
# Class: @C*
#     SubClassOf: @B*
Class: A human individual.  # Generated from value "A human individual." located at cell 'Terms'!C2 using reference @C*.
   	SubClassOf: Person
Class: A role borne by a person while enrolled in an educational program.  # Generated from value "A role borne by a person while enrolled in an educational program." located at cell 'Terms'!C3 using reference @C*.
   	SubClassOf: Student role
Class: A role borne by a person who teaches students.  # Generated from value "A role borne by a person who teaches students." located at cell 'Terms'!C4 using reference @C*.
  	 SubClassOf: Teacher role
Class: An organized set of educational activities and requirements.  # Generated from value "An organized set of educational activities and requirements." located at cell 'Terms'!C5 using reference @C*.
   	SubClassOf: Educational program
# Cell range: (Terms!A4:A4) Comment: ""
# Class: @B*
#     SubClassOf: @C*
Class: Teacher role  # Generated from value "Teacher role" located at cell 'Terms'!B4 using reference @B*.
   	SubClassOf: A role borne by a person who teaches students.















