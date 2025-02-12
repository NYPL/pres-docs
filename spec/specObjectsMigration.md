---
title: Migration / Digitization Status
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 12
---

## Migration / Digitization Statuses
*as needed, multiple controlled values, one active* 

Objects can have their contents migrated to other media or formats. The most common method of migration is digitization, but in cases involving digital carriers, migration can include disk imaging or file transfers. 

An object can have one active migration status, and multiple inactive migration statuses at it goes through the migration process. When a new migration status is added, the previous migration status is made inactive. The date a new status is added is used as the active since date of the new status and the inactive since date for the previous status. If a previous status was entered in error, edit the status field instead of creating a new status record. 

The left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface displays a simplified version of the active migration/digitization status. Click on the status or placeholder text under the Migration / Digitization Status heading to view inactive statuses and their dates or to add a new status. 

The migration / digitization status can also be updated in the **Digitization, description, additional IDs** tab of the AMI specific editing interfaces, see [AMI Specific Fields](https://nypl.github.io/pres-docs/spec/specObjectsAMI.html) for more information. 

When working with a group of objects, migration statuses can be viewed or updated in the [List Edit - AMI](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.html#ami) interface. Use the [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) to update the migration status of multiple objects at once. 

Migration statuses are automatically updated when digitization projects are marked as completed. See SPEC Projects (documentation forthcoming) for more information.

