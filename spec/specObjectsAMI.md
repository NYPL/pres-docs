---
title: AMI Specific Fields
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 15
---

## AMI Specific Fields
In addition to the object elements that are used to describe all objects in SPEC, there are a number of fields specific to AMI items:

| **Field** | **Description** |
| **AMI id** | see [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjectsBasicFields.html#ami-id) for more information | 
| **Diameter** | measurement, in inches, for audio reels, video reels, and grooved media |
| **Generation** | as interpreted during inventory, whether the recording is an original or a copy made subsequently by NYPL or another party |
| **Group** | used to group items within a collection for rough sorting and to aid future arrangement and description |
| **Sequence** | for titles consisting of multiple objects, the sequence number of the particular objects as interpreted during inventory; use numbers only |
| **Content date** | the date of the contents of the object as interpreted during inventory |
| **Content notes** | notes on the content of the object recorded during inventory, often as transcribed on the object or its container |
| **Preservation notes** | notes entered during inventory to indicate condition issues |
| **Manufacturer** | media brand name |
| **Time** |  stock time of the item in minutes |
| **Deaccession?** | enter y when deaccession is recommended |
| **Deaccession rationale** | note to indicate why deaccession is recommended |
| **Inspected?** | film only, enter y if film has been inspected |
| **Inspected by** | film only, account of user who marked film as inspected |
| **Inspected date** | film only, date film was marked as inspected |

Additional film only fields are: shrinkage, base material, acetate decay level, colorbw, edgecode, volume, film element, FPS, length ft, emulsion position, aspect ratio, fading, scratches, splices, perforation, distortion, and con_average.

&nbsp; 
&nbsp; 

AMI specific fields can viewed or updated by navigating to the pop-up window AMI editing interfaces accessible via the **Edit AMI specific fields** or the **Edit AMI film fields** shortcuts on the **Object Search** and the **List Edit** interfaces. The AMI specific editing interfaces can also be accessed by clicking on the **video camera** or **musical note** icon to the right of the object name in the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface.

The **AMI Additional Fields Basic** interface includes fields common to most AMI items. The **Digitization, description, additional IDs** interface includes the [Migration / Digitization Status](https://nypl.github.io/pres-docs/spec/specObjectsMigration.html) information, the [Description](https://nypl.github.io/pres-docs/spec/specObjectsAccessDesc.html#descriptionstatus) field, and a subset of object [References](https://nypl.github.io/pres-docs/spec/specObjectsReferences.html) (cat bnumber, classmark, and other legacy id type references only). The **AMI Film fields** interface displays fields used during film inspection. 

AMI specific fields, along with general SPEC object fields used to describe AMI, can also be viewed or updated in the [List Edit - AMI](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.html#ami) interface.