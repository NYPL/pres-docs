---
title: Value
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 10
---

## Value
*required for outgoing loans, otherwise optional, multiple values*

Value records the monetary value of an object at any given time. Access to object value is restricted by account privileges. Users with access to view and/or edit an object may not have access to view and/or edit the object value. An object can have multiple values assigned. Each value consists of multiple elements. 


### Value
*required, single numeric value*  
The value in USD. 

### Date Assigned 
*required, single date value*  
The date the value was assigned.

### Assigned By
*required, single controlled value*  
Records the staff member who assigned the value.

### Type  
*required, single controlled value*  
Indicates whether the value is based on a formal appraisal or curatorial estimate.

### Notes
*optional, free text*  
Use this field to enter any additional information about the assigned value.

### Attachment
*optional, file upload*  
Supporting documentation for the value. The file is uploaded only to the SPEC database. This is distinct from the attachments that can be uploaded to the object's GoogleDrive folder. See [Attachments](https://nypl.github.io/pres-docs/spec/specObjectsAttachments.html) for more information.

&nbsp; 
&nbsp; 

The left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface displays the latest value assigned to an object. Click on the value or the placeholder text under the Value heading to view details about all previously assigned values or to add a new value in the **Value** pop-up window. A value added by mistake can be deleted using the **x** button; right click on the on attachment and select "Cut" to delete it.
