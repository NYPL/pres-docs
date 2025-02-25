---
title: Format and related fields
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 2
---

## Format
*highly recommended, controlled single value with up to three levels of specificity*

Format represents the generic name for a single object. For items, the format values are primarily drawn from or inspired by the terms and hierarchical structure of the Getty’s Art and Architecture Thesaurus, though may also follow more local format conventions. For containers, the format values are based on the most common containers used throughout the Research Libraries.

The values in each of the three format fields are conditional to, first, the type of object (item or container) and further, the values entered into each of the three levels of format. Not every format or container type has options for all three format fields. It is not required to select a value in the second or third format field, even when options are available for those fields.

{: .tip }
> Select the format manuscript for a single sheet (leaf) or bound volume of paper that is primarily textual but not printed (e.g., handwritten or typed). Create a single object record for a bound manuscript and designate the class as volume. A multi-leaf unbound manuscript should not be represented by one object record: either make a separate object record for each sheet of paper or make an object record for the container the sheets are in and then enter the number of manuscripts (i.e. sheets) as a content estimate for that container. Though archives (paper) is available as a format selection for container content estimates to represent a mix of paper-based formats, archive is not a format. Therefore, it is not available as a choice for a single item.


## Class
*highly recommended, single controlled value*

Class represents the form factor or approximate "shape" of the object. Most formats have default classes, although the class can be entered or overwritten manually. The available classes are:

- **3D object**: three-dimensional objects for which there are no more specific terms in this list
- **Cassette**
- **Container**: containers that store collection items; use "3D object" for items like a wooden box or other artifacts that are part of the collection
- **Digital file**: digital material, but not the physical carriers on which they are stored, such as compact discs, hard disks, and floppy disks
- **Disc**: flat, round objects, such as audio records and compact discs
- **Disk**: rectangular digital storage devices such as hard disks and floppy disks
- **Reel**
- **Sheet**: non-bound items for which the depth of individual items is negligible, such as paper, vellum, photographs, and photographic negatives, including glass or metal plates
- **Volume**


## Content Form
*highly recommended, single controlled value*

Content form identifies the form of the primary content carried by an object. For example, the fontent form of a book is text, a score is musical notation, and a map is cartographic. The available terms are: audio, cartographic, graphic, moving image, musical notation, and text. 


## Extents
*highly recommended, multiple values*

Extent captures the dimensions of an object. Relevant dimensions depend on the object’s type, class, and content. Each extent measurement comprises several elements:

### Measure Type
*required, single controlled value*  
The specific dimension being measured. The available measure types are: height, width, depth, diameter, weight, runtime, and bytesize.

### Unit
*required, single controlled value*  
The unit of measurement for the selected measure type. The available units are: inches, centimeters, kilograms, pounds, milliseconds, GB.

### Measurement
*required, single numeric value*  
The numeric value representing the number of units.

### Context
*optional, single controlled value*  
Specifies the context in which the measurement was taken. The available contexts are: storage (default value), use, display (used for exhibitions and loans).

### Linear Feet Dimension
*required, single controlled value*  
The linear feet dimension determines which measure type (if any) should be used when calculating linear feet. For most formats and container types, there is a default value, though it can be adjusted as necessary. For example, for most containers and books, linear feet calculations are determined by their widths.

&nbsp; 
&nbsp; 

The fields described above can all be viewed or updated in the [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) pop-up window accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and by clicking on the corresponding fields in the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information.

When adding format information in the **Basic Fields** interface use the format search widget to populate the full format hierarchy automatically. An object format cannot be added until the object type is designated. Class, content form, and extents will auto-populate for some formats. 

Width, depth, and height extents can be viewed or added in the **Basic Fields** interface. Click on the extent or placeholder text under the Extent heading in the left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) to view or edit additional extent types, measurements, the extent context, and linear feet dimension.

Formats and some extents can also be viewed or updated in the [List Edit](https://nypl.github.io/pres-docs/spec/specObjectsListEdit.html) interfaces. 

&nbsp; 
&nbsp; 

## Media
*optional, multiple controlled values*

Media identifies the material that an object is made of. The level of detail for this value can vary depending on the level of analysis performed on the object.

Media can viewed or updated by navigating to the **Media** tab of the pop-up window editing interfaces accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, in the media column of the the **Object list survey** interface, and under the media heading in the left panel of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface. See [Populating and Editing Object Records](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) for more information.