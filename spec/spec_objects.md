---
title: SPEC Objects
layout: default
parent: SPEC
nav_order: 1
has_children: true
---

# SPEC Objects

## Introduction
Objects are the physical and digital entities held in the Research Libraries collection storage locations. The details provided in the SPEC Objects section describes the elements of a SPEC object record, focusing on their general purpose and use. It does not specify the best practices for using these elements in particular contexts and processes, such as accessioning or deaccessioning. These processes, and the use of SPEC within them, will be outlined in separate sections of the pres-docs repository (and linked out to from this document, where necessary).

SPEC object records support a level of collection management that is not available through the catalog or other existing systems. SPEC complements, references, and interacts with data about objects in other systems, such as the catalog, ArchivesSpace, the Archives Portal, the MMS, Preservica (planned), and Aeon (planned). Broadly speaking, SPEC object records allow Library staff to:
- track the status and locations of objects
- document their needs
- plan, scope, and track projects
- automate and facilitate certain processes (such as special collections moves)
- document actions undertaken by staff to acquire, describe, and preserve those objects

The goal is to populate SPEC with object records for every special collection item and container on the shelf in the Research Libraries through the Special Collection Survey, data imports from the catalog and other sources, and routine processes (e.g, Acquisitions, AMI inventory). Records for individual items and containers (usually folders) within containers will be created as needed in the course of work demanding a more granular level of object tracking.

## SPEC Object Record Elements

### Type
**Required.** Single controlled value.

There are two types of objects:

#### Items
Items are objects that constitute the Research Libraries collection, such as books, sound recordings, manuscripts, and digital files. In the context of SPEC, the term *item* has a more specific and literal meaning than it does in the context of the catalog, where an “item record” can represent one or more items.

An item in SPEC is always a single thing that is not a container. Bound volumes, such as a book or manuscript diary, are considered a single item, although the pages within them are also considered items.

Items in SPEC are physical or digital objects, not intellectual or bibliographic entities. For example, an unbound 40-page manuscript of a short story is not a single (manuscript) item, but 40 items.

#### Containers
Containers are objects containing items and/or other containers. Containers are not considered part of the Research Library’s collection and are also distinct from storage locations since they are not fixed to a physical place. The contents of containers can be represented in SPEC in two ways: with related object records or content estimates.

### Status
**Required.** Single controlled value.

An object’s status is either *active* or *inactive*. Inactive objects are no longer held by the Library. Examples of inactive objects are:

- An item or container that was part of a proposed acquisition but was not ultimately acquired.
- An item that was deaccessioned.
- A container that was replaced during rehousing.
- A record that was created in error.

The SPEC object record displays the status of an object in its header, along with certain qualifying details:

- **Active From:** The date the object became active. This is often, but not always, the same as the record creation date.
- **Inactive Since:** The date on which the object became inactive.
- **Reason Deactivated:**

### Accessibility
**Required.** Single controlled value.

Accessibility statuses:

- Not available to public [default value for new records].
- Available to public.
- Restricted [i.e., available under certain conditions, such as curatorial approval].
- Unknown.

### Description
**Required.** Single controlled value.

Objects are described by catalog records and finding aids. The existence of a description does not necessarily mean an object is adequately described or that it would not benefit from additional description.

An object’s descriptive status can be:

- Not described [default value for new records].
- Described in catalog.
- Described in finding aid.
- Described in catalog and finding aid.
- More description needed.
- No description needed.
- Unknown.

### Division
**Single controlled value.**

The unit indicates the curatorial division that acquired or currently serves the object.

### Identifiers
The following elements are used to differentiate one object from another, and provide ways to group or sort lists of objects. Though these elements may overlap with information included in bibliographic descriptions of the object, the values in these fields are not intended as authorized descriptions and do not need to be formed in compliance with library and archives standards.

#### Object ID
**Single value. Unique.** Automatically generated by SPEC. Not editable.

#### Object Name
**Display value.** Automatically generated by SPEC.

SPEC creates an object name based on the values of the fields listed below in the following order:

- Container type expressed generically (e.g., box).
- Item title OR, if there is no title, the item format in brackets (e.g., [photograph]).
- Sequence number prefix when entered (if the prefix does not repeat the container type).
- Sequence number when entered.
- Container label text (in parenthesis if it follows a sequence number).
- Container contents when no sequence number or label is entered.
- Audio and moving image (AMI) ID for audio and moving image items.
- Object ID when all other ID fields are empty.

When objects are inactive, their names are displayed crossed out.

#### Barcode
**Single value. Optional. Numeric.**

The barcode that is affixed to the object.

#### Title or Label Text
**Single value. Optional.**

The title or label field can be used to:

- Give the item a title, whether it be its official title, a shorter informal title, or spine title.
- Transcribe what is written on an item or container or on a label affixed (or that will be affixed) to an object.
- Briefly describe what an item is (e.g., umbrella).
- Briefly describe a container’s contents, which may be useful when browsing lists and/or shelves of containers and for differentiating two containers with the same sequence number (e.g., Box 1 AMI vs. Box 1 Artifacts vs. Box 1 Files).

Sequential numeric values (such as serial volume and issue numbers) may be included in the title/label field, though sorting/grouping of object lists will be more navigable if you use the number prefix and number fields.

#### Number Prefix
**Single value. Optional.**

Especially in conjunction with the ID or Sequence Number to group, the Number Prefix may be used to sort or differentiate multiple related objects. For example, for an acquisition that contains two sequential volumes, the Number prefix may be set to "Volume" or "Vol." and the corresponding ID or Sequence Number set to "1" for one object record, and "2" for the other record.

#### ID or Sequence Number
**Single value. Optional. Numeric.**

The ID or Sequence Number may be used, especially in conjunction with the Number Prefix, to group, sort, or differentiate multiple related objects.

#### Other Descriptive Text
**Optional.**

This field is used to provide additional identification details for an object when other fields do not fully capture its unique characteristics.

**Important:** Text entered in this field will not be included in the object name or in any labels printed from SPEC. It serves as supplementary information for internal reference and documentation purposes only.

### Format
**Single value with up to three levels of specificity. Highly recommended. Controlled list of values.**

The *Format* field represents the generic name for a single object. For items, the format values are primarily drawn from or inspired by the terms and hierarchical structure of the Getty’s Art and Architecture Thesaurus, though may also follow more local format conventions. For containers, the format values are based on the most common containers used throughout the Research Libraries.

#### Important Notes:
- **Dependent on Object Type:** The values in each of the three format fields are conditional to, first, the type of object (item or container) and further, the values entered into each of the three levels of format.
- **Optional Levels:** Not every format or container type has options for all three format fields. It is not required to select a value in the second or third format field, even when options are available for those fields.

### Class
**Single value. Highly recommended. Controlled list of values.**

The *Class* field represents the form factor or approximate "shape" of the object. Most formats have default classes, though the class can be entered or manually overwritten. The available classes are:

- **3D object**: Three-dimensional objects for which there are no more specific terms in this list.
- **Cassette**
- **Container**: Containers that store collection items; use "3D object" for items like a wooden box or other artifacts that are part of the collection.
- **Digital file**: Digital material, but not the physical carriers on which they are stored, such as compact discs, hard disks, and floppy disks.
- **Disc**: Flat, round objects, such as audio records and compact discs.
- **Disk**: Rectangular digital storage devices such as hard disks and floppy disks.
- **Reel**
- **Sheet**: Non-bound items for which the depth of individual items is negligible, such as paper, vellum, photographs, and photographic negatives, including glass or metal plates.
- **Volume**

### Content Form
**Single value. Controlled list of values.**

The *Content Form* field identifies the form of the primary content carried by an object. For example, the Content Form of a book is text, a score is musical notation, and a map is cartographic. The available terms are:

- **Audio**
- **Graphic**
- **Moving image**
- **Text**
- **Cartographic**
- **Musical notation**

### Media
**Multiple values. Optional. Controlled list of values.**

The *Media* field identifies the material that an object is made of. The level of detail for this value can vary depending on the level of analysis performed on the object.

### Value
**Multiple values. Optional.**

The *Value* field records the monetary value of an object at any given time.

#### Value Details:
- **Value:**  
  **Single value. Required.**  
  The value in USD.

- **Date Assigned:**  
  **Single value. Required.**  
  The date the value was assigned.

- **Assigned By:**  
  **Single value. Required.**  
  The staff member who assigned the value.

- **Type:**  
  **Single value. Required. Controlled list of values.**  
  Indicates what the value is based on: formal appraisal or curatorial estimate.

### Extent
**Multiple values. Required.**

The *Extent* field captures the dimensions of an object. Relevant dimensions depend on the object’s type, class, and content. Each extent measurement comprises several elements:

#### Measure Type
**Single value. Required. Controlled list of values.**

The specific dimension being measured. The available measure types are:

- **Height**
- **Width**
- **Depth**
- **Diameter**
- **Weight**
- **Runtime**
- **Bytesize**

#### Unit
**Single value. Required.**

The unit of measurement for the selected measure type. The current choices are:

- **Inches**
- **GB**
- **Pounds**
- **Centimeters**
- **Kilograms**
- **Milliseconds**

#### Measurement
**Single value. Required. Number only.**

The numeric value representing the number of units.

#### Context
**Single value. Optional.**

Specifies the context in which the measurement was taken. The current choices are:

- **Storage** *(default value)*.
- **Use**.
- **Display** (used for exhibitions and loans).

#### Linear Feet Dimension
The linear feet dimension determines which *Measure Type* (if any) should be used when calculating linear feet. For most formats and container types, there is a default value, though it can be adjusted as necessary. For example, for most containers and books, linear feet calculations are determined by their widths.

### Received Date
**Single value. Required when known. Year at minimum.**

The *Received Date* field indicates the year, month, and day an object was received by the Library. Only the year is required; SPEC will automatically supply missing months and days as "1" and display them in brackets.

#### Important Notes:
- **Containers:** Containers that were not actually received (but were deployed by Library staff during rehousing) will either not have an acquisition date or will display an acquisition date inherited from the items they contain.

### Assessments
**As needed. Multiple values.**

Objects are assessed by Library staff in various contexts: during the evaluation of an acquisition; in response to inclusion in a potential loan, exhibition, or digitization project; and during an assessment/survey project.

Assessments are logged using the following fields:

#### Date
**Required. Single value.**

The date an object was assessed.

#### Assessed By
**Required. Single value.** Generated by SPEC but modifiable.

The staff member who conducted the assessment. SPEC automatically fills in the username of the staff member entering the record, but this field can be modified as needed.

#### Assessment Name
**Optional. Single value. Controlled list of values.**

Use this field to associate the assessment with a specific project.

#### Documentation
**Required as needed. Single value. “Y” or blank.**

Enter "Y" when the object has acquisition or other documentation with or within it.

#### Issues (Count)
**Generated by SPEC. Not modifiable.**

This field displays the number of issues recorded during the assessment.

### Migration / Digitization Status
**As needed. Multiple values. One active value.**

Objects can have their contents migrated to other media or formats. The most common method of migration is digitization, but in cases involving digital carriers, migration can include disk imaging or file transfers.

### Related Objects
**As needed. Multiple values.**

Some objects have relationships with other objects. Relationships are always bidirectional, and, like objects, they can be active or inactive (see the *Relationships* section for instructions on how to create object relationships).

#### Types of Object Relationships (Predicates)
There are four types of relationships:

- **Contains / Contained by:**  
  Use this relationship to represent the containment of objects that are not physically connected to their containers or contents, meaning one can be moved without the other. An object can contain one or more items or other containers. However, an object can only be contained by one other object, though that object may be contained by yet another object.

- **Has part / Part of:**  
  Use this relationship to represent the connection between an item and a subordinate part when that part merits or requires its own object record. For example, a book may include a tipped-in map. That map is part of the book. If it is removed from the book for conservation, storage, or exhibit, it would no longer be part of the book. The physical relationship between the objects would be documented through the inactive relationship in SPEC. The intellectual relationship would be maintained through the object’s description in the catalog or other descriptive utility, to which their SPEC records will make references.

- **Derives / Derived from:**  
  Use this relationship to represent the connection between an object and another object generated from it. For instance, when an object is photographed, it derives the resulting object (e.g., digital file, negative, or print). The resulting object is derived from the object that was photographed.

### Content Estimates
**Required for containers with no contained object records. Multiple values.**

#### Purpose
Use *Content Estimates* to indicate the number of items and their formats within a container for statistical and planning purposes.

### Location
**Required. Multiple values. Controlled list of values.**

SPEC tracks the present and past locations of objects in several contexts. A more detailed explanation of locations may be found in location-specific documentation (forthcoming).

### References
**Optional. Multiple values.**

*References* are other identifiers created within SPEC, or in systems outside of SPEC (i.e., the Library catalog) with which an object is associated. In many cases, multiple objects share a particular reference (e.g., Acquisition ID), so references serve to group sets of objects together in specific contexts.

References are often created and revised in the course of other actions taken in SPEC (e.g., associating an object with a project), processes being tracked within SPEC, and data updates provided by other systems.

### Restrictions
**Optional. Multiple values.**

#### Restriction Types
**Required. Single value. Controlled list of values.**

Restriction types classify the conditions that govern the accessibility of an object. These types help identify the nature of the restrictions applied, such as those related to preservation needs, content sensitivity, or other factors.

#### Restriction Description
**Optional. Single value. Free text.**

Use this field to further clarify the restriction type.

#### (Active) From
**Required. Single value. Date.**

The date the restriction became active, or, if not known, the date it is recorded in SPEC.

#### Until
**Optional. Single value. Date.**

The date the restriction expired or will expire (if known).

### Issues
**Optional. Multiple values.**

The issues section of an object record is used to record preservation issues discovered during any assessment, as well as their resolution. Whenever an issue is recorded, SPEC automatically creates a corresponding assessment record if there is no record covering the date the issue was discovered.

#### Issue Type

The type of issue entered determines the available choices for the specific *Issues* field.

| **Type**                   | **Issue**                               |
|----------------------------|-----------------------------------------|
| Condition Issues            | Corrosion                               |
| Condition Issues            | Damaging attachments                    |
| Condition Issues            | Flaking media                           |
| Condition Issues            | Iron gall ink                           |
| Condition Issues            | Past insect damage                      |
| Condition Issues            | Red rot                                 |
| Condition Issues            | Staining/accretions                     |
| Condition Issues            | Structural damage                       |
| Condition Issues            | Tape/Tape stains                        |
| Conservation Review         | Needs conservation review               |
| Hazard                      | Acetate                                 |
| Hazard                      | Biohazard                               |
| Hazard                      | Chemical hazard                         |
| Hazard                      | Drugs                                   |
| Hazard                      | Explosives                              |
| Hazard                      | Inactive mold                           |
| Hazard                      | Matches                                 |
| Hazard                      | Nitrate                                 |
| Hazard                      | Other                                   |
| Hazard                      | Radiological material                   |
| Hazard                      | Weapons                                 |
| Housing                     | Inadequate container                    |
| Housing                     | Minimally full box                      |
| Housing                     | Needs container                         |
| Housing                     | Needs custom support                    |
| Housing                     | Needs folder replacement                |
| Inherent Vice               | Color photographic materials            |
| Inherent Vice               | Food                                    |
| Inherent Vice               | Glass disease                           |
| Inherent Vice               | Sticky/Plasticizer migration/Unstable   |
| Other                       | Barcode damage                          |
| Other                       | Shrink wrap                             |
| Other                       | Theft risk                              |
| Storage Method              | Needs different size shelf              |
| Storage Method              | Needs hanging storage                   |
| Storage Method              | Needs museum cabinet                    |
| Storage Method              | Needs painting rack                     |
| Storage Method              | Needs platform/pallet                   |
| Storage Method              | Needs rolled storage                    |
| Storage Method              | Needs shelving                          |

#### Noted Date
**Required. Single value. Date.**

The date the issue was noticed. SPEC automatically fills in the date that the issue is entered by default.

#### Noted By
**Required. Single value. Controlled list of values.**

The staff member who noticed the issue. SPEC fills in the username of the logged-in user who entered the record by default.

#### Rating
**Required for Condition Issues > Structural Damage. Single Value. Number.**

The severity of structural damage. 1: minimal, 2: moderate, 3: severe.

#### Resolved On
**Optional. Single value. Date.**

The date an issue was resolved.

#### Resolved By
**As needed. Single value. Controlled list of values.**

Enter the username of the staff member who resolved the issue.

#### Assessment
**Optional. Single value. Controlled list of values.**

Use this field to indicate a named assessment during which the issue was noticed.

#### (Assessment) Notes
**Optional. Free text.**

Use this field to enter any additional information about the issue and its resolution.

### (Object) Notes
**As needed. Free text.**

Use this field to enter any information about the object that is not accommodated within the other Object Record elements.
