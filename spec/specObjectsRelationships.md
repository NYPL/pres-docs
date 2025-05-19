---
title: Relationships
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 4
---

## Related Objects 
*as needed, multiple controlled values*

Some objects have relationships with other objects. Relationships are always bidirectional, and, like objects, they can be active or inactive. 

There are several types of relationship pairs:

- **contains / containedIn**: Use this relationship to represent the containment of objects that are not physically connected to their containers or contents, meaning one can be moved without the other. An object can contain one or more items or other containers. However, an object can only be contained by one other object, though that object may be contained by yet another object.

- **hasPart / partOf**:  Use this relationship to represent the connection between an item and a subordinate part when that part merits or requires its own object record. For example, a book may include a tipped-in map. That map is part of the book. If it is removed from the book for conservation, storage, or exhibit, it would no longer be part of the book. The physical relationship between the objects would be documented through the inactive relationship in SPEC. The intellectual relationship would be maintained through the object’s description in the catalog or other descriptive utility, to which their SPEC records will make references.

- **derives / derivedFrom**: Use this relationship to represent the connection between an object and another object generated from it. For instance, when an object is photographed, it derives the resulting object (e.g., digital file, negative, or print). The resulting object is derived from the object that was photographed.

- **splitInto / splitFrom**: Deprecated

&nbsp; 
&nbsp; 

Relationships can viewed or updated by navigating to the **Relationships** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the on the **Object Search** and the **List Edit** interfaces, and via the Related Objects section of the **Object Record** interface. When adding a relationship using this interface, an intermediate search window will open. Select the relationship type or predicate, search for the relationship's target object using one or more of the available search fields, and select the target objects from the results to create the relationship. Whenever adding a relationship to the object, the inverse relationship is added to the target object. To deactivate a relationship click the **x** button next to the relationship in the **Relationships** pop-up window; the inverse relationship is automatically deactivated also. Inactive relationships will appear greyed out. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information. 

Additionally, there is a shortcut to add a containedIn relationship in the **Basic Fields** editing interface when the object is an item. A containedIn relationship can also be viewed or updated in the [List Edit](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.htm) interfaces. A containedIn relationship for multiple objects and the same container can be established using the [Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsActionMenu.html). ContainedIn and contains relationships can also be viewed and updated in the [Object Barcode App](https://nypl.github.io/pres-docs/spec/specObjectsOBA.html). 

If an object has an active containedIn relationship, an icon representing the container is visible next to the location designation in the **Object Search** interface. Hover over the icon to see details about the container, click on the icon to open the container's object record. Contained objects inherit their locations from their containers, see [Locations](https://nypl.github.io/pres-docs/spec/specObjectsLocations.html) for more information.

