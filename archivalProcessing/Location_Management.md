---
title: Location Management
layout: default
parent: Processing Collections
grand_parent: Archival Processing
nav_order: 3
has_children: false
---
# **Location Management in the Archival Processing Unit**
You must update the physical locations of all containers in your collection during processing. Collection Management monitors and manages all storage locations, but it is the responsibility of the processing archivist to make sure each object’s location is up to date in SPEC. Most shelves and rooms at LSC have location barcodes that can be scanned directly into SPEC. Archivists should keep a copy of their workspace room’s barcode at their desks. When you bring collection containers from the stacks to your desk, you must update the location in SPEC, and you must do the same for processed materials being stored in the stacks or at your workspace prior to shipment. Collection Management also has [documentation](clmgt/Location_Management.md) that outlines procedures for location management at LSC. 

The chart below details all the times you need to update collection location information in SPEC:

| Scenario | Action in SPEC |
| ---------| ---------------|
| Collection moved from stacks to workspace for survey and/or processing. | Update objects’ location in SPEC with your workspace barcode or current location. |
| Collection returned to stacks after survey for storage. | Update objects’ location in SPEC with stacks shelf location. |
| Collection rehoused into new containers. | [Deactivate](/updating_processed_object_records_in_SPEC.md) the old containers in SPEC. |
| New containers imported from ASpace into SPEC. | Update the locations of all newly imported objects in SPEC. |
| Processed containers moved to stacks for temporary storage. | Update all containers in SPEC with their current room, shelf, or mapcase location. |

Below are instructions on how to update locations using the Object Barcode App and from the Object Search screens in SPEC. The [SPEC Objects Manual](spec/specObjects.md) also has detailed instructions on how to perform all these tasks, as well as a section about [location](spec/specObjectsLocations.md) management.

## **Updating Locations Using the SPEC Object Barcode App**
From the SPEC landing page navigate to the Object Barcode App under the Object menu.

![SPEC Objects Barcode Menu](archivalProcessing/Images/08-Objects-barcode-menu.png)

On the _Object Barcode App_ screen, scan in the barcode of the object whose location you need to update.

![SPEC Object Barcode App](Images/09-Object_Barcode_App.png)

The object name, type, and current location will appear. Scan the new location barcode into the _Location Barcode_ field on the right.

![Scan Location](/Images/10-Scan_location.png)

A message will pop up notifying you that a different object barcode than the current active location has been entered. Select _OK_. 

![Location Message](/Images/11-Location_Message.png)

This will make the previous location inactive, and update the location to the new one you scanned. The new location will be reflected under _Active Storage Location_.

Repeat these steps for each location you need to change. If you have to update many locations, it is recommended that you use the _Object Search_ or _Batch Object Editor_ functions in SPEC.

## **Updating Locations in SPEC Using the Object Editor**
First, navigate to your collection’s objects list. There are a few ways to update locations from the _Object Search_ screen. If you are moving containers from the stacks to your desk, and updating each object’s location to a single new location, it is generally best to use the _Bulk Edit_ function. If you are moving containers from your workspace to the stacks, then the _Batch Edit_ function is generally most useful.

### **Location Management with the SPEC Bulk Editor**
Once you have moved collection containers from the stacks to your desk, open your collection’s objects list. Select the _Action_ button at the top left to open the _bulk editor menu_, then choose _select all_ to select all the objects in your collection. 

![SPEC Bulk Edit Menu](/Images/12-SPEC_Bulk_Edit.png)

Once all the objects are selected, choose the _Action_ menu again and select _Update object locations_.

![Update Object Locations](/Images/13-Update_object_locations.png)

A dialog box will appear notifying you that the current object locations will be deactivated. Select _OK._

![Object Bulk Deactivate](/Images/14-object_bulk_deactivate.png)

A new screen will open that displays the current location, as well as all previous locations. Scan the new location barcode into the box on the right.

![Update Bulk Locations](/Images/15-Update_location_bulk.png)

Once you have entered the new barcode, select the green _Apply Location to Selected Objects_ button.

![Apply Locations Button](archivalProcessing/Images/16-Apply_locations_button.png)

SPEC will return to the _Objects Search_ screen and update all the object locations you selected. The new location will be reflected in the _Location_ field. 

### **Location Management with the SPEC Batch Editor**
You can also update collection object locations from the SPEC _Batch Editor_. There are no bulk editing capabilities from this screen, but you are able to make your edits from a list view for individual items. This is a good option for shelving processed collections in the stacks, or other situations when you will be moving many objects to various locations. 

To use the SPEC _Batch Editor_, navigate to your collection’s objects in SPEC and _All_ next to _Batch edit_ at the top of the screen. 

![Batch Edit All](/Images/17-Batch_Edit_All.png)

This will open the SPEC _Batch Edit_ screen, which displays an editable list of all objects associated with your collection. You can sort these objects by container number by scrolling to the right and clicking on the word _Number_, as illustrated below.

![sort objects](/Images/18-Sort_objects.png)

The object’s current location is in the _Current Location_ column. In order to update the location, click on the barcode icon next to the location. This will open a box prompting you to scan in a new location.

![Update Location](/Images/19-Update_Location.png)

Once you scan in the new location, a dialog box will appear.

![Make Current Location Inactive](/Images/20-Make_Current_Location_Inactive.png)

Select _OK_, and the new location will appear in the object’s location field. Repeat these steps for each location you need to update.
