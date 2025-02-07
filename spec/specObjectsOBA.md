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
> The Object Barcode App is the most convenient way to update locations when working with multiple objects that need to move to different locations. If working with multiple objects that all need to move to the same location consider using the Bulk Action Menu.

To begin, scan the object barcode at the top of the page in the **Scan object barcode to begin** field. 

### Update Location
To enter or change an object’s location, scan the location’s barcode under the **Location Barcode** label in the Active Storage Location section. If the object was assigned to another location, that location will be made inactive. If the object’s assigned location matches the location barcode entered, the location will be verified and the verification will be logged in the audit log.

See SPEC Object [Locations](https://nypl.github.io/pres-docs/spec/specObjectsLocations.html) for more information. 

### Update Contains/ContainedIn Relationships
To indicate an object is stored in a container, scan the container’s barcode under the **Container Barcode** label in the Contained In section. 

To indicate an object has been removed from the container without entering a new container, click **Take out of [container name]** in the Contained In section.

To indicate a container contains another object, scan the contained object’s barcode under the **Object Barcode** label in the Contains section. 

To indicate any of the contained objects are no longer in the container, click the blue **x** next to the object's name in the Contains list.

When updating relationships the contained object's previous relationship will be made inactive. If the relationship between objects already exists, the relationship will be verified and the verification will be logged in the audit log. If verifying a contains relationsihp the contained object's name will display in in green in the container’s object list.


&nbsp; 
&nbsp; 

The objects must have a barcode in order to be updated via the Object Barcode App, if an object does not have a barcode use the editing interfaces availble through the **Object Search** and **Object Record** or the **List Edit** interfaces [LINK] to update the object. 

{: .note }
> Click on an object name to naviagate to the **Object Record** interface. However, once in the object record interface, navigate back to the SPEC landing page to return to the Object Barcode App

