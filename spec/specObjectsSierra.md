---
title: Sierra Data Updates
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 27
---

## Sierra Data Updates
SPEC queries Sierra using an object’s barcode in order to update fields in the object record, create references in an object record to its Sierra item and bibliographic records, and update the description status of the object based on those references.

The following object record elements are populated by the Sierra update, if the field is empty in SPEC: division, title or label text, id number prefix, id or sequence number, format, class, and other descriptive text. 

The following object record references are updated when the data in Sierra is different from the data in SPEC: collection id, bnumber, item number, and classmark 

SPEC queries Sierra in the scenarios described below.

### Barcode Entry
When a user enters a barcode in an object record, SPEC queries Sierra and updates the object record immediately if it finds a match. If no match is found, the record is marked so that its barcode is checked against Sierra each night until a match is found or the object is made inactive.

### SPEC Project Updates
When SPEC updates the outputs for an Archival Processing project, it queries Sierra using the barcode of each of the project’s output objects that has a barcode and has yet to be matched to a Sierra record.

SPEC updates Projects that are in progress or have been completed in the last 60 days each night. The latter are updated since there can be a delay between when a project is completed and records are added to Sierra.

### SPEC Nightly Updates
Each night, SPEC queries Sierra using the barcode of each object with a barcode that has yet to be matched to a Sierra record, excluding inactive objects, AMI originals, and digital carriers. This updates objects that are not associated with a SPEC Project and that were added to SPEC before they were added to the catalog.