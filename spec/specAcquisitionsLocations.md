---
title: Locations
layout: default
parent: SPEC Acquisitions
grand_parent: SPEC
nav_order: 6
---

## Pre-Acquisition Locations
Each acquisition is associated with one or more pre-acquisition locations, which specify where collection materials are stored prior to their delivery to NYPL (i.e. a storage space, a donor’s apartment). Each pre-acquisition location is associated with one or more deliveries.

Use the **+ Add** button in the Location List section of the **Edit Proposal / Acquisition Record** form to add a new pre-acquisition location to an acquisition. Click on the location name in the **Edit Proposal / Acquisition Record** form to edit an existing location. By default, every new acquisition has a stub pre-acquisition location, which should be updated with location information. See [Creating and Editing Acquisition Records] (https://nypl.github.io/pres-docs/spec/specAcquisitions.html#creating-and-editing-acquisition-records) for more information.

The following fields constitute a location:

### Location Name
*required, single free text value*  
Enter name for location, for example: Donor’s Storage Space.

### Transport Coordinated By
*required, single controlled value*  
Specify who will coordinate transport of collection items to NYPL, select NYPL or Source.

### Transport To
*required, single controlled value*  
Specify where collection items will be delivered, select Library Services Center or My curatorial division.

### Import Address Details From This Contact
*optional, single controlled value*  
Select from list of contacts entered into the acquisition's Contact List to import location address details entered into the contact's information.

### Street / City / State 
*required, free text values*  
Location street address, city, and state.

### Zip / Country
*optional, free text values*  
Location zip code and country.

### Contact for This Location
*required, single controlled value*  
Select from list of contacts entered into the acquisition's Contact List.

### Phone / Email
*optional, free text values* 
Location contact's phone and email.

### Notes
*optional, free text value*  
Any notes or additional information pertaining to the location.

### Needs Packing
*optional, single controlled value*  
Select Y if the collection items require packing prior to pickup.

### Needs Site Visit
*optional, single controlled value*  
Select Y if acquisition location requires a site visit prior to pickup.

&nbsp; 
&nbsp; 

The Location List section of the **Acquisition Summary** displays the information entered via the **Edit Proposal / Acquisition Record** form. Locations where a site visit has been requested show a Site Visit flag. Click on the location name in the Location List to navigate to the full **Location Record** interface, where existing location details can be edited and additional location information can be added. The General Information section in the **Location Record** interface contains the fields described above. 

The Site Description section contains more detailed narrative information about a pre-acquisition location that may be used in planning or preparing for subsequent site or packing visits. Enter information about the building, site accessibility, health and safety concerns and other general descriptions. This section also includes a checkbox where Preservation and Collections Processing staff may indicate that a site visit is needed. The Location Details section contains a checklist of common location characteristics that may be useful to know for those involved in site visits, packing or pickup.

The **Location Record** interface also contains a Delivery Log section. See [Deliveries](https://nypl.github.io/pres-docs/spec/specAcquisitionsDeliveries.html) for more information.


&nbsp; 
&nbsp; 

## Site Visit Log
Click on the date field in the Site Visit Log section of the **Location Record** to navigate to the **Site Visit Record** interface. The visit date, coordinated by, staff assigned, travel hours, site hours, goal, and notes related to the Site Visit can be recorded in this interface. Click the blue **checkmark** icon to log the site visit; visit date and total hours (calculated based on travel and site hours) are required to log the site visit. A logged site visit is recorded in the [Activity Log](https://nypl.github.io/pres-docs/spec/specAcquisitionsActivityMessage.html#activity-log).

The **Site Visit Record** interface also displays general Acquisition details in the header, the Extent Summary, Resource Projection, Location Details, and Site Visit Log sections that are also visible in either the **Acquisition Summary** or **Location Record** interfaces.