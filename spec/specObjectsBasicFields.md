---
title: Basic Fields
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 1
---

## Type
*required, single controlled value*

There are two types of objects in SPEC: items and containers. 

An item in SPEC is always a single thing that is not a container. It is an object that is part of the Research Libraries' collections, such as a book, a photograph, a VHS cassette, or a digital file. 

{: .tip }
> Items in SPEC are not intellectual or bibliographic entities. Item has a more literal meaning in SPEC. It is NOT synonymous with an "item record" in the catalog. In SPEC, a bound volume, such as a book or manuscript diary, is considered a single item. On the other hand, an unbound 40-page manuscript is not a single (manuscript) item, but 40 items.

Containers are objects containing items and/or other containers. Containers are not considered part of the Research Libraries' collections and are also distinct from storage locations since they are not fixed to a physical place. The contents of containers can be represented in SPEC in two ways: with related object records or content estimates.

See [Related Objects](https://nypl.github.io/pres-docs/spec/specObjectsRelationships.html) and [Content Estimates](https://nypl.github.io/pres-docs/spec/specObjectsContentEstimates.html) for more information.


## Barcode
*highly recommended, single numeric value, unique*

The barcode that is affixed to the object. Object barcodes must be unique. 


## Division
*required, single controlled value*

The division indicates the curatorial unit that acquired or currently serves the object. 

The terms "division" and "curatorial unit" are used interchangeably in SPEC. When an object is associated with a collection and there is a mismatch between the division assigned to the object and the division assigned to the collection, SPEC will automatically update the object's division to match the associated collection's division. This update is triggered when any field in the object is updated.


## Title or Label Text
*optional, single free text value*

The title or label field can be used to:

- Give the item a title, whether it be its official title, a shorter informal title, or spine title
- Transcribe what is written on an item or container or on a label affixed (or that will be affixed) to an object
- Briefly describe what an item is (e.g., umbrella)
- Briefly describe a container’s contents, which may be useful when browsing lists and/or shelves of containers and for differentiating two containers with the same sequence number (e.g., Box 1 AMI vs. Box 1 Artifacts vs. Box 1 Files)


## ID Number Prefix
*optional, single free text value*

In conjunction with the id or sequence number to group, the number prefix may be used to sort or differentiate multiple related objects. For example, for an acquisition that contains two sequential volumes, the number prefix may be set to "Volume" or "Vol." and the corresponding id or sequence number set to "1" for one object record, and "2" for the other record.


## ID or Sequence Number
*optional, single numeric value*

The id or sequence number may be used to group, sort, or differentiate multiple related objects.

&nbsp; 
&nbsp; 

The fields described above can all be viewed or updated in the [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjects.html#populating-and-editing-object-records) pop-up window accessible via the **Edit object record** shortcut on the **Object Search** and the **List Edit** interfaces, and by clicking on the corresponding fields in the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface.

&nbsp;

---
 
&nbsp; 


## SPEC Generated Fields

## Object ID
*automatically generated, single numeric value, unique* 

Every object has a unique numerical value assigned by SPEC at the time of its creation. Generally, this number does not appear on the physical collection material. This value is not editable and can be viewed in the header of the [Object Record](https://nypl.github.io/pres-docs/spec/specObjectsObjectRecord.html) interface.


## AMI ID
*automatically generated, single numeric value, unique* 

Every AMI object has a six digit unique numerical value assigned by SPEC when an AMI format is added to the object record; this value is distinct from the object id. AMI ids are not editable and are assigned based on a range of values assigned to a user's account. see [AMI Specific Fields](https://nypl.github.io/pres-docs/spec/specObjectsAMI.html) for more information.


## Object Name
*automatically generated display value*

SPEC creates an object name, displayed on the **Object Search**, **Object Record**, and **List Edit** interfaces, based on the values of the fields listed below in the following order:

- Container type expressed generically (for example, box)
- Item title OR, if there is no title, the item format in brackets (for example, [photograph])
- Sequence number prefix when entered (if the prefix does not repeat the container type)
- Sequence number when entered
- Container label text (in parenthesis if it follows a sequence number)
- Container contents when no sequence number or label is entered
- AMI id for audio and moving image items
- Object id when all other ID fields are empty

&nbsp; 
&nbsp; 

The SPEC generated fields described above cannot be edited.