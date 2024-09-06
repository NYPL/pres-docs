---
title: Creating SPEC Objects
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 2
---

# Creating SPEC Objects

## Basic Methods

There are several contexts where object records can be created.

### SPEC Landing Page
The most basic method to create an object record is from the **SPEC Landing page**. Here, click **Create object record**.

### Object Search
In the **Object Search** screen, click **+ Create new object**.

### Acquisition Proposal Inventory
Click **+ Add / Edit** in the **INVENTORY** section of an acquisition proposal, and then click **+ Add** to create a new object record. In this context, SPEC will automatically associate the object with the acquisition.

### Collection Summary
From the context of a **Collection Summary**, in the **SPEC RECORDS** section, click **+New** to the right of the Object Count. In this context, SPEC will automatically associate the object with the collection record.

> **Note:** If you generate a list of objects from the context of a Collection or Acquisition record, this button will read **+ Create new object in [Collection/Acquisition title]**. Any object records created using this button will be assigned to that collection/acquisition. Click the **Clear** button to remove this default assignment.

## Duplicate

From the **Object Search** screen or the **List Object Editor**, click the action button to the left of an existing object record and select **Duplicate** from the action menu.  
   
> **Note:** Object records created via duplication can be edited.

Either method will open the **Object Duplicate Options** window. This window will provide a list of object elements whose values may be carried over to the new duplicate object record. Some object elements will be pre-selected depending on:

- The selection(s) made during the last time you duplicated a record (i.e., your selections will appear automatically).
- The context in which you started the duplication process (e.g., acquisition/collection will be selected if all new records are being assigned to a particular acquisition/collection, and the format will be selected when duplicating an AMI record).
- The record you are duplicating.

### To duplicate a record:

1. Enter the number of duplicate records you want to make.
2. Select elements to duplicate and/or deselect elements.
   - The values that will be assigned to each element are displayed in light gray to the right of each element you can duplicate.
   
> **Note:** Dependencies between fields will restrict or determine your selections. For instance, you cannot select an element with no blue value or an acquisition location or delivery if you are not duplicating the acquisition reference. Selecting **Format** will automatically check **Type**.

> **Additional Note:** You can only select one of the four label number options and cannot select a label number for AMI, since their number is automatically assigned by SPEC.

Click **Duplicate** to complete the process.

## Acquisition Proposal Inventory (Items)

- Click the **duplicate record** button to the right of the row/record to duplicate.
- Indicate the number of duplicate records to create.
- New records duplicate the following fields:
  - Format fields
  - Class
  - Title/label
  - Acquisition reference

> **Note:** Number fields are given sequential numbers based on the highest number value of objects of the same type, except for AMI items, which are given the next available AMI IDs assigned to staff entering the records.

## Acquisition Proposal Inventory (Containers / Loose Items)

- Click the **duplicate record** icon next to the container that you want duplicated.
- In the pop-up window, indicate:
  - The number of duplicate containers to create.
  - The count of items of the specified format in those containers.
  - Whether the count should be applied to each container or distributed across the new containers.
- Click **OK**.
- New records duplicate the following fields:
  - Content format
  - Container type
  - Class
  - Title/label
  - Acquisition reference

> **Note:** Number fields are given sequential numbers based on the highest number value of objects of the same type.