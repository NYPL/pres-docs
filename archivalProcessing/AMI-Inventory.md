---
title: Audio and Moving Image Inventory and Description
layout: default
parent: Processing Audio and Moving Image Material
grand_parent: Archival Processing
nav_order: 2
has_children: false
---
# **AMI Inventory and Description**
AMI in archival collections are accessioned on an item level by collection management when a new acquisition is received, or when a backlog collection is shipped to the Archival Processing unit for processing. Each piece of media is labeled with a barcode and a unique AMI identifier generated in SPEC. Collection management will also update SPEC with the format of each object. 

For acquisitions received in 2023 to the present, the AMI inventory will be attached to the acquisition record. Older collections may have a preliminary inventory with bibliographic data attached to the collection record. 

In the Archival Processing unit, the inventory of AMI in archival collections is performed by exporting a spreadsheet of the initial Collection Management inventory and enhancing it with DACS-compliant descriptive data, including titles, dates, and tracklists. During the inventory, if you encounter incorrect formats, you should correct the record in SPEC. The completed inventory will be imported into ArchivesSpace. See the section on [Importing an Audio and Moving Image Inventory]() into ArchivesSpace for instructions on how to do this.

## **Moving a SPEC AMI Inventory to the SPEC Collection Record**
Before you begin processing any AMI, your first step is to move the inventory into the acquisition’s associated collection record. To do this follow the steps below:

1. Navigate to the acquisition record and select the inventory icon.
![SPEC Objects List](/Images/37-SPEC-objects-list.jpg) 

2. When the inventory opens, filter the SPEC objects list just for AMI.
![SPEC AMI Filter](/Images/38-AMI-objects_filter.jpg)

3. Select the _bulk action_ menu.
![SPEC Bulk Action Menu](/Images/39-SPEC-Bulk-Action.jpg)

4. Choose _select all_ from the _Action_ menu. This will check the boxes for each AMI object.
![SPEC Select All](/Images/40-SPEC-Select-All.jpg)

5. Select the _Action_ menu again, and this time choose _add to collection_.
![SPEC Add to Collection](/Images/41-SPEC-add-to-collection.jpg)

6. A warning dialog box will open, select _OK_.
![SPEC warning box](/Images/42-SPEC-Warning.jpg)

7. Search for the collection in the pop up box, and then choose the blue _select_ button next from the list.
![SPEC reference list](/Images/43-SPEC-reference-list.jpg)

8. SPEC will then perform an operation to associate all the AMI with the collection record. This may take a few minutes. 

9. Once this is complete, navigate to the collection record, and you should see all the new associated objects in the content summary. 

## **Inventory Export**
To create an inventory of the AMI for ArchivesSpace you will need to export an inventory spreadsheet from the SPEC collection record. This step should only occur in the collection record after all objects have been associated with the collection record. Do not export from the Acquisition record.

There are two types of exports, a full csv export from the SPEC _List Object Editor_ or the AMI _ASpace export_, which exports only the fields that can be imported in ASpace.

### **SPEC Export csv**
For larger collections, it is advisable to export the full AMI object list. Follow the steps below to complete this object. 

1. Navigate to the collection record and select the collection objects from the _SPEC Records_ menu on the left.

![SPEC Records menu](/Images/44-SPEC-Records-Menu.jpg)

2. This will open the full collection objects list that includes container objects, born-digital carriers, and AMI. 

3. Navigate to the top of the page and select _AMI_ next to the term _List edit_. This will filter the objects to only display the collection’s AMI.

![List edit](/Images/45-SPEC-list-edit.jpg)

4. Once you have filtered the objects for just AMI, navigate to the bottom of the screen and select _Export (CSV)_.

![Export csv](/Images/46-export-csv.png)

5. A dialog box will pop up when the export is finished indicating that the csv has been downloaded to your desktop.

![SPEC file downloaded](/Images/47-SPEC-file-downloaded.jpg)

6. It is recommended that you upload the csv to google drive and open it in google sheets before starting your inventory work. Excel sometimes adds special characters or formatting that can lead to data loss. 

### **AMI ASpace Export**
If you have a small collection, you may choose to just export the basic AMI inventory using the _AMI ASpace Export_ button. This creates a spreadsheet in the format required for import into ASpace, and includes only the fields that will import. 

The _AMI ASpace Export_ button is also located on the left hand side of a SPEC collection record. 

![SPEC AMI ASpace Export Button](/Images/48-AMI-ASpace_export-button.jpg)

When you select this button, a spreadsheet of all the AMI objects will automatically export to your desktop. This spreadsheet will export without column labels. It is recommended that you add them before resuming inventory work. 

The fields that will import into ASpace are listed in [SPEC CSV Export to AMI ASpace Export Crosswalk](/Documents/SPEC_CSV_Export_to_AMI_ASpace_Export_Crosswalk.pdf).





