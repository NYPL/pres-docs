---
title: Restrictions
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 7
---

## Restrictions  
*optional, multiple values*

An object can have multiple active or inactive restrictions. Expired restrictions are not deleted from object records, rather they are made inactive by entering an end date to maintain historical data. Each restriction consists of multiple elements.


### Type  
*required, single controlled value*  
The restriction type classifies the conditions that govern the accessibility of an object. These types help identify the nature of the restrictions applied, such as those related to preservation needs, content sensitivity, or other factors. 

### Restriction Description  
*optional, single free text value*  
Description further clarifies the nature of restriction. 

### From  
*required, single date value*  
Specifies the date the restriction became active, the date defaults to the date the restriction was added to the object record. 

### Until  
*as needed, single date value*  
Specifies the date the restriction expired or will expire (if known). 

&nbsp; 
&nbsp; 

Restrictions can viewed or updated by navigating to the **Restrictions** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the Restictions section of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information. 

