---
title: Deliveries
layout: default
parent: SPEC Acquisitions
grand_parent: SPEC
nav_order: 7
---

## Deliveries
The Delivery List section of the **Acquisition Summary** displays details for all deliveries scheduled or completed from pre-acquisition sites. Click on the *location* name in the Location List to navigate to the **Location Record** interface to view, edit, or add additional delivery information. 

The Delivery Log section in the **Location Record** interface contains details of all scheduled deliveries from *that* location. Note that an acquisition can be associated with multiple pre-acquisition locations, and each pre-acquisition location can be associated with multiple deliveries. 


To schedule a delivery from the pre-acquisition location, click on the **+ Add** button at the top of the Delivery Log. This will add a new entry into the log. 

The following fields constitute a delivery:

### Delivery ID
*automatically generated, single numeric value, unique*  
This number appears next to Request details and can be used to associate SPEC objects with the delivery and acquisition.  

### Arranged By
*required, single controlled value*  
Specify whether NYPL or the donor or dealer will coordinate the shipment, select NYPL or Source.

### Number of Objects to Deliver
*automatically generated, single numeric value*  
Provides an automatic count of objects associated with the delivery. Click the blue **>** to navigate to the **Object Search** interface where object delivery references can be updated using the delivery id. See [SPEC Objects / References](https://nypl.github.io/pres-docs/spec/specObjectsReferences.html) and [Bulk Action Menu](https://nypl.github.io/pres-docs/spec/specObjectsBulkActionMenu.html) for more information.  

### Delivery To
*required, single controlled value*  
Select either Library Services Center or My curatorial division.

### Scheduled For
*required, single date value, month/day/year*  
Date for which the delivery has been scheduled. When this date is entered, the status of the acquisition is updated to Delivery Pending and the action is recorded in the [Activity Log](https://nypl.github.io/pres-docs/spec/specAcquisitionsActivityMessage.html#activity-log). See [Action / Status](https://nypl.github.io/pres-docs/spec/specAcquisitionsActions.html) for more information.

### Shipment Type
*optional, single controlled value*  
Select shipment type from drop-down list. 

### Requires Packing
*optional, single controlled value*  
Select Y if the shipment requires packing. 

### Boxes Needed
*optional, single free text value*  
Quantity of boxes required to house acquisition materials requiring packing.

### Packing Completed
*optional, single free text value*  
Date when packing was completed.

### Mover Name / First Name / Last Name
*optional, single free text values*  
Name of the moving company and the first and last name of moving company contact.

### Mover Email / Phone
*optional, single free text values*  
Mover's phone and email.

### Cost
*optional, single free text value*  
Total cost of mover in USD.

### Tracking Number
*optional, single free text value*  
Mover tracking number

### Notes
*optional, single free text value*  
Any notes or additional information pertaining to the delivery.

### Receipt Info
*required for received deliveries, various field types*  
Displays the year, month, day, when the delivery was received, the location where it was received, the number objects received and the automatically assigned accession id for the delivery. These fields are auto-populated when an acquisition is marked as received, all except the accession id can be modified manually if necessary. See [Action / Status](https://nypl.github.io/pres-docs/spec/specAcquisitionsActions.html) for more information. 

A delivery received date can also be added in the Deliveries Received section of the **Edit Proposal / Acquisition Record** form. However, doing so overrides the acquisition approvals process and updates the acquisition status to Received. The **Edit Proposal / Acquisition Record** form also includes an optional local accession id field. 