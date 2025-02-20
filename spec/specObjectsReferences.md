---
title: References
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 6
---

{: .note }
> This page is under construction! 
> Content update in progress ...

## References
*as needed, multiple controlled values*

Object references are alternate identifiers assigned to an object, such as an AMI id or other legacy id. In many cases, references point to related records within SPEC or other databases such as ArchivesSpace, Archives Portal, or Sierra; SPEC provides links to those records whenever possible. Often, multiple objects share a particular reference, such as an acquisition id or a collection id, grouping sets of objects together in specific contexts. References are created and revised in the course of actions taken in SPEC, processes being tracked within SPEC, and data imports from other systems.

References that refer to other record types in SPEC include CMS acq delivery id, CMS acquisition id, and CMS collection id. Each acquisition can be associated with one or more deliveries, however each delivery is only associated with one acquisition; adding a delivery reference to an object automatically adds the associated acquisition id. Collections can be associated with one or more acquisitions, and an acquisition can be associated with one or more collections. Linking a collection to an acquisition does not automatically cause the objects associated with the acquisition to inherit the collection reference. ... [MORE DETAILS FORTHCOMING] ... All newly acquired objects entered into SPEC should be associated with acquisition and acq delivery ids; only objects that are part of archival collections need to be associated with a collection id. 

SPEC Project IDs [SPEC PROJECTS DOCUMENTATION FORTHCOMING]

Other editable object references are accession number, CMS digital media log legacy id, conservation id, other legacy id, separation id, TL number.

CMS AMI id, also referred to as simply AMI id, is the SPEC generated id assigned to all AMI items. This reference is not editable. See [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjectsBasicFields.html#ami-id) for more information.  

The cat bnumber refers to the corresponding bibliographic record in Sierra (the library catalog), and the cat item record refers to the Sierra item record. These references along with classmark may be imported from Sierra, see [Sierra Data Updates](https://nypl.github.io/pres-docs/spec/specObjectsSierra.html) for more information. Cat bnumber and classmark can also be added or edited individually, cat item number is not editable.   

References imported from ArchivesSpace are the ASpace archival object id, ASpace top container id, ASpace multiple identifier record id, other id (ASpace); references imported from the Archives Portal are Archives Portal component id and Archives Portal collection id. Additional ids imported from other databases are the MMS capture UUID and Preservica UUIDs. These references are not editable. 

Legacy reference types include the CMS AMI dig batch id (superseded by SPEC Project IDs), CMS item id, CMS ingest report import record id, CMS project id (superseded by SPEC Project IDs), and Rose Building temporary id.

&nbsp; 
&nbsp; 

All references can viewed and editable references can be updated by navigating to the **References** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and via the References section of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. To delete an incorrect reference click the **x** button next to the reference, only editable references can be deleted. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information.

When adding references to other SPEC record types, such as CMS collection id and CMS acq delivery id, click the **Search** button to the right of the new reference to open an intermediate window and search for the related record. Select the related record from the results to create the reference. When adding an acquisition delivery and its associated acquisition reference there is an option to create a new acquisition record using the green **+ NEW ACQUISITION** button. See SPEC Acquisitions [ADD LINK] for more information.

Use the **Add to collection**, **Add to acquisition (delivery / location)**, or **Add to project** options in in the [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) to add the same collection, acquisition and delivery, or SPEC project reference to multiple objects. Search for the related collection, acquisition delivery or SPEC project in the pop-up search window; there is also an option to create a new acquisition or a new SPEC project when creating references using the Bulk Action Menu.