---
title: Restrictions
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 6
---

## Restrictions
*optional, multiple values*
An object can have mulitple active or inactive restrictions. Restrictions are not deleted from object records, rather they are made inactive by entereing an end date to maintain historical data. Each restriction consists of multiple elements.

### Type
*required, controlled single value*, 

The restiction type classifies the conditions that govern the accessibility of an object. These types help identify the nature of the restrictions applied, such as those related to preservation needs, content sensitivity, or other factors. 

### Restiction Description
*optional, single free text value*
The descriptionis used to further clarify the nature of restriction. 

### From
*required, single date value*

Specifies the date the restriction became active, the date defaults to the date the restiction was added to the object record. 

### Until
*as needed, single date value*

Specifies the date the restiction expired or will expire (if known). 

&nbsp; 
&nbsp; 

Restictions can viewed or updated by navigating to the Restiction tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the Restictions section of the **Object Record** interface. See Populating and Editing Object Records [ADD LINK] for more information. 

