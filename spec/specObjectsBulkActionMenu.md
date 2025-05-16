---
title: Bulk Action Menu
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 20
---

## Bulk Action Menu
The **Bulk Action Menu** provides a way to edit certain object record elements across a group of objects. Find a set of objects in the **Object Search** interface. Select a subset of objects records in the object search result list by clicking the check box to the left of each object, or click on the **Action** menu button above the object check boxes and click **Select All** from the menu. Objects can be deselected individually or using the **Select None** option from the **Action** menu. 

{: .tip }
> When using the Bulk Action Menu the object element specified in the action will be updated to the same value across all selected objects, i.e. each selected object will be assigned the same collection and/or acquisition/delivery reference, the same active location, the same reason for deactivation, etc.

Click on the **Action** menu button to select an action to be performed across all selected objects.

| **Action** | **Use to** |
| **Add issue** | add issue to selected objects |
| **Add to acquisition (delivery / location)** | search for and assign an acquisition delivery id and associated acquisition id references; this action will replace existing acquisition delivery and acquisition references |
| **Add to collection** | search for and assign a collection id reference; if the collection is associated with an acquisition, this action also adds the acquisition delivery and acquisition references, if not already present; this action will replace existing an existing collection reference. See SPEC Object [References](https://nypl.github.io/pres-docs/spec/specObjectsReferences.html) for more information on SPEC acquisition, acquisition delivery and collection reference logic  |
| **Add to container** | search for a container and create a contains/containedIn relationship between the container and selected objects; adding selected objects to a container will deactivate any existing relationships to another container |
| **Add to exhibition** | FORTHCOMING |
| **Add to loan checklist** | add selected objects to an outgoing loan by navigating from loan record (registrar only) |
| **Add to project** | add selected objects to a project by searching for or navigating from a project record |
| **Create container label pdf** | generate labels for selected containers, any selected items will be omitted; a .pdf file downloaded to the user's Desktop will open automatically |
| **Deactivate selected objects** | make selected objects inactive. See [Deactivating Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#deactivating-object-records) for more information |
| **Edit content estimates** | replace existing content estimate(s) or add an additional content estimate to selected containers |
| **Edit labels and sequence numbers** | assign a label, label number prefix, and/or sequence number to selected objects |
| **Edit migration status** | assign a new migration status to selected objects, previously active migration status will be made inactive by receiving an end date |
| **Mark selected objects as received** | assign a received date based on the associated acquisition delivery date to selected objects |
| **Reactivate selected objects** | make selected inactive objects active again. See [Reactivating Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#reactivating-object-records) for more information |
| **Remove from collection** | remove any collection references|
| **Remove from container** | deactivate relationships between selected objects and their current containers; object locations inherited from the disassociated container will update to "not indicated" |
| **Remove from project** | remove selected objects from a project |
| **Select all** | select all of the objects in the found set for subsequent actions |
| **Select none** | deselect all previously selected objects in the found set |
| **Update object locations** | add or update the location of selected objects, any previously active location will receive an end date and become inactive; locations for contained objects or objects that are part of deliveries that have not been received will not be updated |