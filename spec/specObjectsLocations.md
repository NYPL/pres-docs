---
title: Locations
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 3
---

## Locations
*required, multiple controlled values, one active*

SPEC tracks the present and past locations of objects in several contexts: before they are acquired (i.e. pre-acquisition location), in NYPL storage and processing locations, and internal and external exhibition/loan locations. SPEC does not track: public service circulation when collections are removed from storage to reading rooms, or specific locations within RECAP. 

Except for pre-acquistion locations and external exhibition locations, every location in SPEC is part of a comprehensive location hierarchy maintained by Collection Management. Each location designation consists of the building, room, row, unit, and shelf or drawer. Each location is also assigned a barcode.

Object locations are never deleted, rather when a new location is entered for an object its prior location is made inactive. Entering locations for objects yet to be marked as received will mark those objects as received on the date the corresponding acquisition delivery was received.

Contained objects inherit their container's location. To change a contained object's location, deactivate the container relationship. See [Relationships](https://nypl.github.io/pres-docs/spec/specObjectsRelationships.html) for more information. 

&nbsp; 
&nbsp; 

Locations can viewed or updated by navigating to the **Locations** tab of the pop-up window editing interfaces accessible by clicking on the **Current location** directly in the **Object Search** result list. The locations editing interface can also be accessed via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the Location in the header of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. Although a location can be added by using the drop-down lists for each level of the hierarchy, scanning the location barcode is recommended. Additionally, there is a shortcut to add a location barcode in the **Basic Fields** editing interface. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information. 

Locations can also be updated in the [List Edit](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.htm) interfaces. Use the **Update object locations** option in in the [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) to add a new location to a group of objects. Finally, locations can be updated in the [Object Barcode App](https://nypl.github.io/pres-docs/spec/specObjectsOBA.html). 

The **Object Search** interface will dispaly the object's location in red or as "Missing" if the object is associated with an active (i.e. unresolved) location type issue, see [Issues](https://nypl.github.io/pres-docs/spec/specObjectsIssues.html) for more information.