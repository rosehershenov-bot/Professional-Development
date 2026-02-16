Install Cellfie as a plug-in on Protege. (see directions in dimension).    
Download the spreadsheet in the PD document next to the link to this repository.   

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
