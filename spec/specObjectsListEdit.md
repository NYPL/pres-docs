---
title: List Edit Interfaces
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 21
---

## List Edit Interfaces
The **List Edit** interfaces provide a way to view and edit data across a set of object records. Generate a found set of object records in the [Object Search](https://nypl.github.io/pres-docs/spec/specObjects.html#object-search) interface. Click on **All**, **AMI**, or **Survey** (CLMGT only) next to the List edit label between the basic search fields and the object search results list. 

Each interface shows a different selection of object elements, see details below. The found set of object records can be sorted by any field where the column name appears in blue. Click on the **Object name** to navigate to the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. Use the **Export (CSV)** button in the lower left corner of each interface to export object record data for all objects visible in the list.

Navigate back to the Object Search using the **< Object search results** button in the upper left, below the **SPEC Logo**, found on each of the **List Edit** interfaces. 


&nbsp; 
&nbsp; 

## List Edit - All 
The **List Object Editor** interface will show a list of all objects in the found set. This interface is also accessible form the Object Counts by Format Category section of the **Collection Summary**.

The object barcode, contained in relationship, current location (for uncontained objects) can be updated by clicking on the **barcode** icon to the left of the column to open a pop-up into which the appropriate barcode can be scanned. 

Type, the format hierarchy, and division can be updated using a drop-down list within the column. Extents, id number prefix, id or sequence number, and title or label text can be updated by typing directly into the field. 

The list displays the first content estimate for container type objects, if one exists, and the object's format with a content count of 1 for item type objects. Click on **View All / Edit / Add estimates** at right end of the list to view and add additional content estimates.

The down caret button to the left of each object provides access to the **Editing Shortcuts** pop-up menu. 

Box labels can be generated from this interface using the **Create box labels** button above the Object name column. Specify the box range in the pop-up window, the found set of objects will be narrowed down to all containers that fall into the specfied range. Click OK to generata a .pdf file; the file, downloaded to user's Documents folder, will open automatically.

&nbsp; 
&nbsp; 

## List Edit - AMI
The **List Edit - AMI** interface will limit the found set of object records to AMI only. 

The object barcode, contained in relationship, current location (for uncontained objects) can be updated by clicking on the **barcode** icon to the left of the column to open a pop-up into which the appropriate barcode can be scanned. 

The **down caret** button to the left of each object provides access to the **Editing Shortcuts** pop-up menu and the **Action** button above the object check boxes provides access to the **Bulk Action Menu** options.

The **All Items in Containers** and **Go to Containers** buttons navigate to the specified set of related records in the  **Object Search** interface. The **Film Stats** button generates film inspection statistics for a specified date range. 

&nbsp; 
&nbsp; 

## List Edit - Survey (CLMGT only)
The **Object list survey** interface is similar to the **List Edit - ALL** interface, but displays fields and shortcuts most relevant to performing special collection survey assessments. The interface includes an **eye** icon that automatically creates an assessment record attributed to the signed in user with today's date. This interface also includes a button to **Create object record** 