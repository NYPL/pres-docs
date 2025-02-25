---
title: Sierra Data Updates
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 27
---

## Sierra Data Updates
SPEC queries Sierra using an object’s barcode in order to update fields in the object record, create references in an object record to its Sierra item and bibliographic records, and update the description status of the object based on those references.

{: .tip }
> SPEC object division, title or label text, id number prefix, id or sequence number, format, class, and other descriptive text fields are updated with data from Sierra if they are empty; collection id, bnumber, item number, and classmark object references are added or updated if they are different.

SPEC queries Sierra in the scenarios described below.

### Barcode Entry
When a user enters a barcode in an object record, SPEC queries Sierra and updates the object record immediately if a match is found. If no match is found, the record is marked so that its barcode is checked against Sierra each night until a match is found or the object is made inactive.

### SPEC Project Updates
When SPEC updates the outputs for an archival processing project, it queries Sierra using the barcode of each of the project’s output objects that has a barcode and has yet to be matched to a Sierra record.

SPEC updates projects that are in progress or have been completed in the last 60 days each night. The latter are updated since there can be a delay between when a project is completed and records are added to Sierra.

### SPEC Nightly Updates
Each night, SPEC queries Sierra using the barcode of each object with a barcode that has yet to be matched to a Sierra record, excluding inactive objects, AMI originals, and digital carriers. This updates objects that are not associated with a SPEC project and that were added to SPEC before they were added to the catalog.