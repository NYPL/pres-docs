---
title: References
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 6
---

## References
*as needed, multiple controlled values*

Object references are alternate identifiers assigned to an object, such as an AMI id or other legacy id. In many cases, references point to related records within SPEC or other databases such as ArchivesSpace, Archives Portal, or Sierra; SPEC provides links to those records whenever possible. Often, multiple objects share a particular reference, such as an acquisition id or a collection id, grouping sets of objects together in specific contexts. References are created and revised in the course of actions taken in SPEC, processes being tracked within SPEC, and data imports from other systems.

### Acquisition, Acquisition Delivery, and Collection References
References that refer to other record types in SPEC include CMS acq delivery id, CMS acquisition id, and CMS collection id. Each acquisition can be associated with one or more deliveries, however each delivery is only associated with one acquisition; adding a delivery reference to an object automatically adds the associated acquisition id. Collections can be associated with one or more acquisitions, and an acquisition can be associated with one or more collections. Linking a collection to an acquisition does not automatically cause the objects associated with the acquisition to inherit the collection reference. Adding a collection reference to an object adds the first associated acquisition reference and the first associated delivery reference, if the object does not already have those references assigned. All newly acquired objects entered into SPEC should be associated with one acquisition id and one acq delivery id; only objects that are part of archival collections need to also be associated with a collection id. 

### Project References (as of June 2025, in limited use only)
SPEC Project IDs [DOCUMENTATION FORTHCOMING] link objects to projects. An object can have multiple project references. 

### Other Editable References
Other editable object references are accession number, CMS digital media log legacy id, conservation id, other legacy id, separation id, TL number.

### AMI IDs
CMS AMI id, also referred to as simply AMI id, is the SPEC generated id assigned to all AMI items. This reference is not editable. See [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjectsBasicFields.html#ami-id) for more information.  

### Sierra References
The cat bnumber refers to the corresponding bibliographic record in Sierra (the library catalog), and the cat item record refers to the Sierra item record. These references along with classmark may be imported from Sierra, see [Sierra Data Updates](https://nypl.github.io/pres-docs/spec/specObjectsSierra.html) for more information. Cat bnumber and classmark can also be added or edited individually, cat item number is not editable.   

### ArchivesSpace and Archives Portal References
References imported from ArchivesSpace are the ASpace archival object id, ASpace top container id, ASpace multiple identifier record id, other id (ASpace); references imported from the Archives Portal are Archives Portal component id and Archives Portal collection id. Additional ids imported from other databases are the MMS capture UUID and Preservica UUIDs. These references are not editable. 

### Other Database References
A number of references from other databases have been imported into SPEC, including Preservica UUIDs, MMS caputre UUIDs, and TMS ids. As of June 2025, references imported from these databases are not comprehensive.

### Legacy References
Legacy reference types include the CMS AMI dig batch id (superseded by SPEC Project IDs), CMS item id, CMS ingest report import record id, CMS project id (superseded by SPEC Project IDs), and Rose Building temporary id.

&nbsp; 
&nbsp; 

All references can be viewed and editable references can be updated by navigating to the **References** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the References section of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. To delete an incorrect reference click the **x** button to the left of the reference, only editable references can be deleted. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information.

When adding references to other SPEC record types, such as CMS collection id and CMS acq delivery id, click the **Search** button to the right of the new reference to open an intermediate window and search for the related record. Select the related record from the results to create the reference. 

When adding an acquisition delivery and its associated acquisition reference there is an option to create a new acquisition record if one does not yet exist in SPEC using the green **+ NEW ACQUISITION** button. This option is most often used during retrospective accessioning workflows. See SPEC Acquisitions [DOCUMENTATION FORTHCOMING] for more information.

Use the **Add to collection**, **Add to acquisition (delivery / location)**, or **Add to project** options in in the [Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsActionMenu.html) to add the same collection, acquisition and delivery, or SPEC project reference to multiple objects. Search for the related collection, acquisition delivery or SPEC project in the pop-up search window; there is also an option to create a new acquisition or a new SPEC project when creating references using the **Action Menu**.