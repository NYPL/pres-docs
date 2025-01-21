---
title: Relationships
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 3
---

{: .note }
> This page is under construction! 
> More content coming soon ...


## Related Objects 
*as needed, multiple controlled values*

Some objects have relationships with other objects. Relationships are always bidirectional, and, like objects, they can be active or inactive. 

There are several types of relationships:

- **contains / containedIn:**  
  Use this relationship to represent the containment of objects that are not physically connected to their containers or contents, meaning one can be moved without the other. An object can contain one or more items or other containers. However, an object can only be contained by one other object, though that object may be contained by yet another object.

- **derives / derivedFrom:**  
  Use this relationship to represent the connection between an object and another object generated from it. For instance, when an object is photographed, it derives the resulting object (e.g., digital file, negative, or print). The resulting object is derived from the object that was photographed.

- **hasPart / partOf:**  
  Use this relationship to represent the connection between an item and a subordinate part when that part merits or requires its own object record. For example, a book may include a tipped-in map. That map is part of the book. If it is removed from the book for conservation, storage, or exhibit, it would no longer be part of the book. The physical relationship between the objects would be documented through the inactive relationship in SPEC. The intellectual relationship would be maintained through the object’s description in the catalog or other descriptive utility, to which their SPEC records will make references.

- **splitInto / splitFrom:**  
  [to be deprecated? ]



Restictions can viewed or updated by navigating to the Restiction tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the on the **Object Search** and the **List Edit** interfaces, and via the Restictions section of the **Object Record** interface. See Populating and Editing Object Records [ADD LINK] for more information. 


View additional details or update the the migration status by clicking on the current status or placeholder text under the migration/digitization status heading in the left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface or in the digitization, description, additional IDs tab of the AMI specific editing interfaces, see [AMI Specific Fields](https://nypl.github.io/pres-docs/spec/specObjectsAMI.html) for more information.

Migration statuses can also be viewed or updated in the [List Edit - AMI](https://nypl.github.io/pres-docs/spec/specObjectsMigration.html) interface. Use the [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) to update the migration status of multiple objects at once. 


To deactivate a relationship, click the close button next to the relationship in the **Object Relationships** list window.



