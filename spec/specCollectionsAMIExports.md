---
title: AMI Exports
layout: default
parent: SPEC Collections
grand_parent: SPEC
nav_order: 1
---

## AMI Export
The AMI items associated with a collection can be exported by using the the **AMI Export** button in the SPEC Records section of the **Collection Summary** interface. This export downloads a .csv file to the user's desktop. 

This export is *not* formatted for import into ArchivesSpace; the export contains additional fields describing AMI items for reference purposes. Attempting to import this export or any other AMI export from SPEC that is not formatted exactly like the **ASpace AMI Export** (see below) will result in an error.


## ArchivesSpace AMI Export
Similarly to the **AMI Export**, the **ASpace AMI Export** found in the SPEC Records section of the **Collection Summary** interface, exports a .csv file to the user's desktop of all AMI items associated with a collection.   

This export is specifically formatted for import into ArchivesSpace. It includes the following fields in the following order, with no column headings: AMI id, division, collection id, id label text, date, classmark, legacy id, content notes, generic format (i.e. format 1), group, and sequence. 

If generating a collection AMI item .csv file by other means, manually editing the file to conform exactly to the formatting of this export is required to import the data into ArchivesSpace.