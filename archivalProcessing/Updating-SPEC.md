---
title: Updating SPEC
layout: default
parent: Archival Processing
nav_order: 19
has_children: false
---
# Updating SPEC
{: .no_toc }

There are a number of tasks that need to be completed in SPEC both during and after processing a collection. This section details some of those workflows.

## Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

# Updating Processed Object Records in SPEC
It is recommended that you deactivate a collection’s original container as you are processing. Once you have finished processing a collection, you should verify that you have made all original containers inactive in SPEC, and double check that you did not miss any of the unprocessed materials. In most cases objects should be deactivated from the _acquisition record_. However, if you are processing a backlog collection without an acquisition record, or an artificial collection without acquisition information, then you will need to deactivate the boxes from the _collection record_. 

Below are the steps and some accompanying images that illustrate how to deactivate boxes in a SPEC acquisition record. If you are working on backlog, legacy, or an artificial collection, skip to [Deactivating Objects in a Collection Record]().

## Deactivating Objects in an Acquisition Record
Login to SPEC and select find/propose an acquisition in the Acquisitions menu.
![SPEC acquisition search](/Images/96-Spec-acquisition-search.png)

The acquisitions search screen will open. Enter the acquisition identifier or acquisition title and select search.

![SPEC acquisition search screen](/Images/97-acquisition-search-screen.png)

The search results will appear below the search menu. Select the acquisition record you need to update by clicking on the acquisition name.

A screen will open with detailed information about the acquisition. Select the _inventory_ icon in the _extent summary_ box to view the objects associated with the acquisition.

![SPEC extent summary](Images/98-extent-summary.png)

 A new screen will open listing all the objects associated with the collection. This will often include audio and moving image items, digital media carriers, received boxes that were rehoused, and unprocessed containers with their original stacks locations. 

To deactivate a box, click on the ^ icon and select deactivate from the pop-up menu as illustrated below. 

![SPEC deactivate object](/Images/100-SPEC-deactivate.png)

A new dialog box will open that is populated with the current date in the _When_ field and your SPEC username in the _Deactivated By_ field. The _Reason For Deactivating_ field has a dropdown menu. Click on the dropdown menu icon on the right to open the menu.

Select the reason you are deactivating the object record from the menu. When deactivating boxes from processed collections, you should always select Contents rehoused.

![SPEC deactivation reason](/Images/101-SPEC-deactivation-reason.png)

Once you have made your selection, click on the _confirm_ button.

![Confirm Button](/Images/108-confirm-button.png)

If you wish to deactivate multiple boxes at once, use the SPEC bulk deactivation feature, which allows you to select all the objects you need to deactivate. See the section of this documentation on [Bulk Object Deactivation]() for more information about how to do this. 

## Deactivating Objects in a Colletion Record
Login to SPEC and select _search all collections_ in the _Collections menu._

The collections search screen will open.

![SPEC Collections Search](/Images/102-SPEC-Collections-search.png)

Enter the collection identifier or title, and select _search_.

![SPEC search](/Images/103-SPEC-Search.png)

The search results will appear below the search menu. Select the collection you need to update by clicking on the collection name.

A new screen will open with the collection’s summary information, including the call number, format counts, and linked records. Click on the number to the right of the word _objects_ under the SPEC Records menu. This number indicates the total number of objects associated with the collection record.

![Collection Objects](/Images/104-Objects.png)

A new screen will open listing all the objects associated with the collection. After a collection has been processed, all the old boxes need to be deactivated. 

To deactivate a box, click on the ^ icon and select deactivate from the pop-up menu as illustrated below.

![Deactivate Button](/Images/106-Deactivate.png)

A new dialog box will open that is populated with the current date in the _When_ field and your SPEC username in the _Deactivated By_ field. The _Reason For Deactivating_ field has a dropdown menu. Click on the dropdown menu icon on the right to open the menu. 

Select the reason you are deactivating the object record from the menu. When deactivating boxes from processed collections, you should always select _Contents rehoused_.

![Dactivate Object](/Images/107-Object-Deactivate.png)

Once you have made your selection, click on the confirm button.

![Confirm Button](/Images/108-confirm-button.png)

If you wish to deactivate multiple boxes at once, use the SPEC bulk deactivation feature, which allows you to select all the objects you need to deactivate. See the section of this documentation on [Bulk Object Deactivation](https://nypl.github.io/pres-docs/archivalProcessing/updating_processed_object_records_in_SPEC.html#bulk-object-deactivation-in-spec) for more information about how to do this. 

## Bulk Object Deactivation in SPEC
Navigate to the collection’s objects list.

The objects will display in list format with check boxes to the left, as illustrated in the image below. 

![objects List](/Images/109-Objects-List.jpg)

Make sure you are in the _object search_ screen, and not the _batch editor view_. Bulk edit functionality is not available in the _Batch edit_ screen.

Select all the objects you wish to deactivate by clicking in the boxes to the left of the object name. You may also select all objects by navigating to the _Action_ menu and choosing _Select All_.    

![SPEC checkboxes](Images/109-SPEC-checkboxes.jpg) ![Select All](/Images/110-SPEC-Select-all.png)

Click on the _Action_ menu at the top and select _Deactivate Selected Objects._

![Deactivate Selected Objects](/Images/111-Deactivate-Selected-Objects.png)

A dialog box will open asking for the reason you are deactivating the objects. You should always select _Contents Rehoused_.

![Content Rehoused](/Images/112-Content-Rehoused.png)

Press the _Confirm_ button after you have selected _Contents rehoused_ from the menu.

![Confirm Button](/Images/108-confirm-button.png)

A box will pop up asking if you would like to deactivate all the selected objects. Press _OK_.

![Dialog Box](/Images/113-Dialog-Box.jpg)

The objects you selected will be deactivated and appear crossed out in the objects list.

![Deactived Objects](/Images/114-Deactivated-Objects.jpg)

# Importing Object Records Into SPEC
After your finding aid has been approved by your supervisor and curatorial staff, you have barcoded each box, scanned the barcodes into ArchivesSpace, and deactivated the processed containers in SPEC, you will need to import the collection’s containers from ArchivesSpace into SPEC.

First open up the collection in ASpace and select _Export Item CSV_ from the _Export_ dropdown menu.

![ASpace Export Menu](/Images/115-ASpace-Export.png)

ASpace will then generate a csv file of all the containers, each container’s extent (for container types that include dimensions in ASpace), and each container’s barcode. Make sure to save the file in a place where you can easily locate it later. 

If you have to open up the csv file in Excel for editing purposes, be sure to format the cells in the barcode column before you save the file. To do this, highlight the column of barcodes, then right click _Format Cells_. While working in the number tab, click on _Number_ under Category and change Decimal places to 0. This will allow the format of the cells to display the entire barcode numbers correctly. This is very important in order for the barcodes to be correctly imported into SPEC.

Next navigate to  the _collection record_ in SPEC, and locate the _SPEC RECORDS_ portion of the screen.

![SPEC Import Button](/Images/116-SPEC-Import.png)

Select the _ASpace Object Import_ button

A navigation window will pop up. Select the csv file you created, and click _open._

The containers will be imported as objects in the collection record. If your collection includes any containers without dimensions in ASpace, be sure to manually enter them into SPEC so that the collection extent is correct. See the section of this documentation on [Updating Container Dimensions in SPEC]() for instructions on how to do this.

Once the new containers have been imported, make sure to update their locations in SPEC. For instructions on how to update locations, see the [Location Management](https://nypl.github.io/pres-docs/archivalProcessing/Location_Management.html)section of this documentation.



