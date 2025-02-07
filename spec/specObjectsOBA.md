---
title: Object Barcode App
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 22
---

## Object Barcode App
The Object Barcode App allows users to quickly verify or update an object's location and relationships (container or contained objects). Click on the **Object Barcode App** link in the Objects section on the **SPEC landing page** to access this feature.   

{: .tip }
> The Object Barcode App is the most convenient way to update locations if you are working with multiple objects that need to move to different locations. If you are working with multiple objects that all need to move to the same location consider using the Bulk Action Menu.

Scan the object barcode at the top of the page in the **Scan object barcode to begin** field. 

&nbsp; 
 

To enter or change an object’s location, scan the location’s barcode under the **LOCATION BARCODE** label in the **ACTIVE STORAGE LOCATION** section. If the object was assigned to another location, that location will be made inactive. If the object’s assigned location matches the location barcode entered, the location will be verified. The verification is logged in the audit log.

See SPEC Object [Locations](https://nypl.github.io/pres-docs/spec/specObjectsLocations.html) for more information. 

&nbsp; 
&nbsp; 

To indicate the container in which an object is stored, scan the container’s barcode under the **CONTAINER BARCODE** label in the **CONTAINED IN** section. 

To indicate an object has been removed from the container without entering a new container, click **Take out of [container name]** in the **CONTAINED IN** section.

To indicate that an object is stored in a container, scan the contained object’s barcode under the **OBJECT BARCODE** label in the **CONTAINS** section. 

To indicate any of the contained objects are no longer in the container, click the blue icon to the left of the object's name.

When updating the contains/containedIn relationships the previous relationship will be made inactive. If the relationship between objects already exists, the relationship will be verified and the verification will be logged in the audit log. If verifying a contains relationsihp the contained object's name will display in in green in the container’s object list.


&nbsp; 
&nbsp; 

The objects must have a barcode in order to be updated via the Object Barcode App, if an object does not have a barcode use the editing interfaces availble through the **Object Search** and **Object Record** or the **List Edit** interfaces [LINK] to update the object. 

{: .note }
> Click on an object name to naviagate to the **Object Record** interface. However, once in the object record interface, navigate back to the SPEC landing page to return to the Object Barcode App

