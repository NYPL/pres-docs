---
title: Issues
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 8
---

## Issues
*as needed, multiple values*

The issues section of an object record is used to record preservation issues discovered during any assessment, as well as their resolution. Whenever an issue is recorded, SPEC automatically creates a corresponding assessment record if there is no assessment record covering the date the issue was discovered. See [Assessments](https://nypl.github.io/pres-docs/spec/specObjectsAssessments.html) for more information. 


### Type
*required, single controlled value*  
The type of issue entered determines the available choices for the specific issue field. The following issue types are availabe in SPEC: Condition Issues, Conservation Review, Digital Media, Disposition, Hazard, Housing, Inherent Vice, Location, Media Caputure, Other, Storage Method.

### Issue 
*required, single controlled value* 
Every specific issue is classfied into one of the above types. 

### Noted Date
*required, single date value*  
The date the issue was noticed. SPEC automatically fills in the date that the issue is entered by default.

### Noted By  
*required, single controlled value*  
Records the staff member who noticed the issue. SPEC auto-populates the field with the name of the user adding the issue; the field can be modified manually, if necessary.

### Rating
*required for condition issues: structural damage,  single numeric value*  
Records the severity of structural damage. 1: minimal, 2: moderate, 3: severe.

### Resolved On
*as needed, single date value*  
The date an issue was resolved.

### Resolved By
*as needed, single controlled value*  
The name of the user who resolved the issue.

### Assessment
*optional, single controlled value*
Indicates a named assessment during which the issue was noticed.

### Notes
*optional, free text*  
Use this field to enter any additional information about the issue and its resolution.

&nbsp; 
&nbsp;

Issues can viewed or updated by clicking on the yellow **hazard** icon in the [Object Search](https://nypl.github.io/pres-docs/spec/specObjects.html#object-search) interface, which appears when an object is associated with an unresolved issue. When an object is not already associated with an unresovled issue, add a new issue by navigating to the **Issues** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the Issues section of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information. 

Use the [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) to add an issue to multiple objects at once. The same issue data will be added to each selected object.

Use the **Remove issue** button only to delete an issue added to an object by mistake, otherwise use the resolved on and resolved by fields to maintain an accurate historical record of object issues.