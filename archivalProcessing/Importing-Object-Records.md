---
title: Importing Object Records Into SPEC
layout: default
parent: Final Steps
grand_parent: Archival Processing
nav_order: 6
has_children: false
---
# Importing Object Records Into SPEC
After your finding aid has been approved by your supervisor and curatorial staff, you have barcoded each box, scanned the barcodes into ArchivesSpace, and deactivated the processed containers in SPEC, you will need to import the collection’s containers from ArchivesSpace into SPEC.

First open up the collection in ASpace and select _Export Item CSV_ from the _Export_ dropdown menu.

![ASpace Export Menu](/Images/115-ASpace-Export.png)

ASpace will then generate a csv file of all the containers, each container’s extent (for container types that include dimensions in ASpace), and each container’s barcode. Make sure to save the file in a place where you can easily locate it later. 

If you have to open up the csv file in Excel for editing purposes, be sure to format the cells in the barcode column before you save the file. To do this, highlight the column of barcodes, then right click _Format Cells_. While working in the number tab, click on _Number_ under Category and change Decimal places to 0. This will allow the format of the cells to display the entire barcode numbers correctly. This is very important in order for the barcodes to be correctly imported into SPEC.

Next navigate to  the _collection record_ in SPEC, and locate the _SPEC RECORDS_  portion of the screen.

![SPEC Import Button](/Images/116-SPEC-Import.png)

Select the _ASpace Object Import_ button

A navigation window will pop up. Select the csv file you created, and click _open._

The containers will be imported as objects in the collection record. If your collection includes any containers without dimensions in ASpace, be sure to manually enter them into SPEC so that the collection extent is correct. See the section of this documentation on [Updating Container Dimensions in SPEC]() for instructions on how to do this.

Once the new containers have been imported, make sure to update their locations in SPEC. For instructions on how to update locations, see the [Location Management](https://nypl.github.io/pres-docs/archivalProcessing/Location_Management.html)section of this documentation.



