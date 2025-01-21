---
title: Bulk Action Menu
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 20
---

{: .note }
> This page is under construction! 
> Content is being edited ...

## Bulk Action Menu

The Bulk Action Menu provides a way to edit certain object record elements across a group of objects. Find a set of objects in the **Object Search** inteface. Select a subset of objects records in the object search result list by clicking the check box to the left of each object, or click on the **Action** menu button above the object check boxes and click **Select All** from the menu. Objects can be deselected individially or using the **Select None** option from the **Action** menu. 

{: .tip }
> When using the Bulk Action Menu the object element specified in the action will be updated to the same value across all selected objects, i.e. each selected object will be assigned the same collection and/or acquisition/delivery reference, the same active location, the same migration status, etc.


Click on the **Action** menu button to select an action to be preformed across all selected objects.

| **Action** | **Use to** |
| **Add to acquisition (delivery/location)** | search for and assign an acquisition delivery id and associated acquisition id references |
| **Add to collection:** | search for and assign a collection id reference; if the colelction is associated with an acquisition, this action also adds the acquisition delivery and acqusition references. See SPEC Object [References](https://nypl.github.io/pres-docs/spec/specObjectsReferences.html) for more information on SPEC acquisition, acquisition delivery and collection reference logic  |
| **Add to container:** | search for a container and create a contains/containedIn relationship between the container and selected objects |
| **Add to loan checklist** | add selected objects to an outgoing loan by navigating from loan record (registrar only) |
| **Add to project:** | add selected objects to a project by searching for or navigating from a project record |
| **Add to SCT move:** | forthcoming |
| **Deactivate selected objects:** | make selected objects inactive |
| **Edit content estimates:** | replace existing content estimate(s) or add an additional content estimate to selected containers |
| **Edit labels and sequence numbers:** | assign a label, label number prefix, and/or sequence number to selected objects |
| **Edit migration status** | assign a new migration status to selected objects, previously active migration status will be made inactive by receiving an end date |
| **Mark selected objects as received:** | assign a received date based on the associated acquisition delivery date to selected objects |
| **Reactivate selected objects** | make selected inactive objects active again ... See [add link] for more information|
| **Remove from checklist** | remove project or loan references |
| **Remove from collection:** | remove any collection references|
| **Remove from container:** | deactivate relationships between selected objects and their current containers |
| **Select all:** | select all of the objects in the found set for subsequent actions |
| **Select none:** | deselect any previously selected objects in the found set |
| **Update object locations:** | add or update the location of selected objects, any previously active location will be made inactive by receiving an end date;locations for contained objects or objects that are part of deliveries that have not been received will not be updated |