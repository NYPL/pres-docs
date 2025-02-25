---
title: Assessments
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 10
---

## Assessments
*as needed, multiple values*

Objects are assessed by staff in various contexts: during the evaluation of an acquisition; in response to inclusion in a potential loan, exhibition, or digitization project; and during an assessment/survey project. An object can be assessed multiple times. Each assessment consists of multiple elements.


### Date
*required, single date value*  
The date an object was assessed. SPEC auto-populates the field with today's date; the field can be modified manually if necessary.

### Assessed By
*required, single controlled value*  
Records the staff member who conducted the assessment. SPEC auto-populates the field with the name of the user logging the assessment; the field can be modified manually, if necessary.

### Assessment Name
*optional, single controlled value*  
This field associates the assessment with a specific project or specifies the type of assessment. In many instances SPEC auto-populates the field to special collections survey; the field can be modified manually, if necessary. The following assessment names are available in SPEC: accessioning, exhibition loan / review, site visit, or the special collections survey. 

### Documentation
*required as needed, single controlled value*  
Enter "Y" when the object has acquisition or other documentation, leave blank otherwise.

### Issues (Count)
*automatically generated*  
Displays the number of issues recorded during the assessment.

&nbsp; 
&nbsp; 

The left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface displays the date of the latest assessment associated with an object. Click on the assessment date or the placeholder text under the Last Assessed heading to view details about all previous assessments or to add a new assessment in the **Assessments**  pop-up window.  

Click the **Today** button shortcut (CLMGT only) next to the Last Assessed heading in the **Object Record** or use the **eye** icon on the [List Edit - Survey](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.html#survey-clmgt-only) interface (CLMGT only) to add an assessment with today's date, special collections survey assessment name, and your username.

An assessment is automatically created when an issue is added to an object, with the date the issue is noted and the name of the user who added the issue. If multiple issues are added with the same date, no new assessment is created, rather the number of issues is added up in the issues count field. See [Issues](https://nypl.github.io/pres-docs/spec/specObjectsIssuess.html) for more information.

An assessment is automatically created when an AMI film item is marked as inspected with today's date, a film inspection assessment name, and the name of the user who marked the film as inspected. See [AMI Specific Fields](https://nypl.github.io/pres-docs/spec/specObjectsAMI.html) for more information.

An assessment added by mistake can be deleted using the **x** button in the **Assessments**  pop-up window. However, deleting an assessment does not delete an issue or film inspection that may have automatically created the assessment. 