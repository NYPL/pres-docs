---
title: Editing SPEC Objects
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 3
---

# Introduction

[Screenshot pending]

To access and edit the most common object record elements, use the Objects Editor. The Editor can be accessed from a number of different contexts:
- **Object Search or List Object Editor:** click on the action button to the left of an object’s name in the search results and select Edit object record.
- **Object record:** click directly on any blue-underlined field (for example, a barcode) to open the Editor.

You can edit most object elements from the Basic Fields screen. For a list of object elements and their definitions, see [SPEC Object Record Elements](https://nypl.github.io/pres-docs/spec/spec_objects_elements.html#spec-object-record-elements).

The Basic Fields screen includes a navigation bar at the top that can be used to toggle between other common object elements/element groups, including Media, Relationships, References, Restrictions, Issues, Locations and Estimates.

# Editing SPEC Objects

Most object elements can be edited by simply clicking into the field and typing. However, some object elements require additional details to be input.

---

## Assessment

To log an assessment or edit an existing assessment record:

1. For objects that have been previously assessed, click on the assessment date. For objects with no assessments assigned, click “**Click here to enter**.” This will open the **Object Assessments** window.
2. You also have the option to click **Today** to quickly add a new assessment with today’s date (this option is only available to Collection Management staff).
3. Click the `+` button to add a new assessment record to the list.

---

## Accessibility and Description Status

To manually edit the accessibility or description status of an object record:

1. In the **Object Record** header, click on the status to open the **Accessibility and Description Status** window.
2. Enter values for both **Accessibility** and **Description**.

Note: The **description status** will update automatically when you add a reference to a catalog record or finding aid.

---

## Content Estimates

- Update content estimates as necessary. If items are moved from one container to another, deactivate the content estimate in the original container.
- If you make a container inactive, the content estimates will be automatically deactivated, and the counts will no longer be used in statistical calculations.

You can also add and edit multiple content estimates by clicking **View All / Edit / Add** in the **Content Estimates** section in the Object Record.

To add a content estimate for a container:

- Click the `+` button.
- Select from the list of available values or keyword search for the format.

### Notes on Formats

- **Manuscripts**: Use for textual documents that are not printed (e.g., handwritten or typed) or for printed documents with extensive handwritten annotations. Count the number of sheets, not intellectual units like letters.
- **Archives (paper)**: Use for mixed items in various formats (including photographs) that are difficult to count separately. Count the number of sheets of paper.
- Always indicate **Class** and **Media** whenever possible.

---

## Extents

To edit **Extents**, click under the **Extents** section in the left-hand pane of the **Object Record**. To add a new extent measurement, click the `+` button.

When adding extent measurements in the Basic Fields screen, the default unit of measure will be inches. If you change the unit of measure, it will change it for all three dimensions.

---

## Formats / Container Types

In the **List Object Editor** and the **AMI object list**, you can add or edit an object’s format or container type using dropdown menus for each field. The available values depend on the type of object (item or container) and other selected values.

### Keyword Search

To navigate format hierarchies more easily, SPEC provides an option to keyword search available format terms in the **Basic Fields screen**.

---

## Locations

### General Rules

Entering a location for an object will either:

- Make the current location inactive and create a new active location record.
- Create a record in the object record audit log noting that the location was verified.

For contained objects, location inheritance applies. To change a contained object's location, you must first disassociate it from its container.

### Editing Locations

Whenever possible, use a location’s barcode to enter an object’s location. You can edit or add a location by clicking on the object’s current location, including pre-acquisition locations.

To edit the **NYPL location**, click **+ UPDATE LOCATION** and enter all known elements of the location. The location fields will automatically populate when the barcode is entered.

---

## Media

To add or edit an object's medium/media, click under the **MEDIA** section in the left-hand pane of the **Object Record**. Click **+ ADD MEDIA** to add a new media type.

---

## Received Date

### Adding a Received Date

When an object is part of an acquisition delivery that has been marked as received:

1. Assign it an NYPL location.
2. Select **Mark as received** from the action menu in the **Object Search** list or the **Object Record**.

This will automatically assign a **Received Date** based on the delivery date. You can also manually enter the **Received Date** by clicking under **RECEIVED** in the left-hand pane of the **Object Record**.

### Editing a Received Date

Click the **Received Date** to:

- Edit the received date.
- Change its pre-acquisition location.
- Change the delivery it belongs to.

---

## References

Objects are often related to other records within and outside SPEC. For example, an object may be linked to a **SPEC acquisition record**, a **finding aid** in the Archives Portal, or a **bibliographic record** in the NYPL catalog. These relationships are called **references**.

To add or edit a reference:

1. Click **View All / Edit / Add** in the **REFERENCES** section of the **Object Record**.
2. Click the `+` button to add a new reference.
3. Select the reference type from the dropdown menu.
4. Manually enter the reference; some references may be searched for (Collections, Acquisitions, or Acquisition Deliveries).

## Reference Types

The table below describes the current reference types, the record that the type describes, whether they can be manually added or are automatically added by the system, and whether they refer to a legacy identifier.

| **From System**  | **Reference Type**                 | **Record Description**                                            | **Manually or Automatically Added?** | **Legacy?** |
|----------------- |------------------------------------|-------------------------------------------------------------------|--------------------------------------|-------------|
| Archives Portal  | Component ID                       | Component that describes the object.                              | Automatic                            |             |
| Archives Portal  | Collection ID                      | Finding aid in which the object is described.                     | Automatic                            |             |
| ArchivesSpace    | Archival Object ID                 | Component describing the object.                                  | Automatic                            |             |
| Sierra           | Cat bnumber                        | Bibliographic catalog record.                                     | Manual                               |             |
| Sierra           | Cat item record                    | Item catalog record.                                              | Manual                               |             |
| Sierra           | Classmark                          | Curatorial-assigned classmark.                                    | Manual                               |             |
| SPEC             | Acq delivery id                    | Acquisition delivery record of which the object was part.         | Automatic                            |             |
| SPEC             | CMS acquisition id                 | Acquisition of which an object is part.                           | Automatic                            |             |
| SPEC             | CMS AMI dig batch id               | Digitization batch in which an object was included.               | Automatic                            |             |
| SPEC             | CMS AMI id                         | Audio or moving image item assigned during inventory.             | Automatic                            |             |
| SPEC             | CMS collection id                  | Collection of which the object forms a part.                      | Automatic                            |             |
| SPEC             | CMS digital media log legacy id    | Digital carrier assigned during inventory.                        | Automatic                            |             |
| SPEC             | CMS ingest report import record id | Media ingest report.                                              | Automatic                            | Y           |
| SPEC             | CMS item id                        | Object record in the legacy Items table in CMS.                   | N/A                                  | Y           |
| SPEC             | SPEC project id                    | Project where object was addressed                                | Automatic                            |             |
| MMS              | MMS capture UUID                   | Digitization capture record                                       | Automatic                            |             |
| Other            | Other legacy id                    | Any other record identifier                                       | N/A                                  |             |
| SPEC             | Rose Building temporary id         | Object identifier assigned during Rose clearout project (2019-21).| Automatic                            | Y           |

---

## Relationships

### Adding and Deactivating Relationships

To add a relationship:

1. Click the `+` button in the **RELATED OBJECTS** section.
2. Choose a relationship type.
3. Search for the object you want to link.

To deactivate a relationship, click the close button next to the relationship in the **Object Relationships** list window.

---

## Values

To add a value:

1. Open the **Object Value Log** by clicking the value field.
2. Enter the required fields (Value, Date assigned, Type, and Assigned by).
3. Click the `+` button to add the new value.

---

## Migration / Digitization Statuses

To update an object’s migration or digitization status:

1. Click the **Migration / Digitization Status** field in the **Object Record**.
2. Select the new status from the available options.

---

## List Object Editor

The **List Object Editor** provides a way to review and edit lists of objects.

There are two ways to open the List Object Editor:

1. Use the **Object Search** screen to perform a search to generate a list of objects. From there, next to **Batch Edit**, click either **All**, **AMI**, or **Survey**.  
   - **All** will show a list of objects regardless of format.  
   - **AMI** will only show audio and moving image materials.  
   - **Survey** will generate a view specific to performing special collection survey assessments.
2. Click **Batch Edit** in the Actions column within a **Collection Summary’s “Object Counts by Format Category”** section.

---

## Object Barcode App

The **Object Barcode App** is a quick way to specify, edit, or verify an object’s:
- location
- container
- contained objects

To access the app from the SPEC Landing page, click on the **SPEC Barcode App** link.

### To call up an object:
Scan the barcode of the container or the contained object in the top-most field marked **Scan object barcode to begin**.

### Locations
To enter or change an object’s location, scan the location’s barcode under the **LOCATION BARCODE** label in the **ACTIVE STORAGE LOCATION** section.

- If the object was assigned to another location, that location will be made inactive.
- If the object’s assigned location matches the location barcode entered, the location will be verified. The verification is logged in the audit log.

### Container
To indicate the container in which an object is stored, scan the container’s barcode under the **CONTAINER BARCODE** label in the **CONTAINED IN** section.

- If the object was previously associated with another container, that relationship will be made inactive.
- If the object is already associated with the container just scanned, the relationship will be verified. The verification is logged in the audit log.

To indicate an object has been removed from the container (without entering a new container), click **Take out of [container name]** in the **CONTAINED IN** section.

### Contained Objects
To indicate that an object is stored in a container, scan the contained object’s barcode under the **OBJECT BARCODE** label in the **CONTAINS** section.

- If the object was previously associated with another container, that relationship will be made inactive.
- If it already has a relationship to the current container, the relationship will be verified. The verification is logged in the audit log and is indicated by the object’s name displaying in green in the container’s object list.

To indicate any of the contained objects are no longer in the container, click the blue icon to the left of the object's name.

---

## Group Action Tool

Along with making edits to individual object records, SPEC also provides a way to edit certain fields across a group of objects using the **Group Action Tool**.

### To edit a group of object records:
1. Call up a list of objects using the **Object Search** screen.
2. From the found set, either manually check individual records, or select the entire found set by clicking on the **Action Menu** button and then clicking **Select All**. You can deselect all items by clicking **Select None**.

### Available actions for multiple records:
- **Add to acquisition (delivery/location):** Assigns a selected delivery ID and associated acquisition ID as references in the selected object records.
- **Add to a collection:** Assigns a selected collection ID and other associated IDs (e.g., bnumber, classmark) as references in the selected object records.
- **Add to container:** Creates a **containedIn** relationship to a selected object for all of the objects selected.
- **Add to loan checklist**
- **Add to project:** Adds the selected objects to a project. *(In development)*
- **Add to SCT move**:: _Forthcoming_
- **Deactivate selected objects:** Marks the selected objects as inactive.
- **Edit content estimates:** Assigns the same content estimate to each selected container. You can choose to either add the new content estimate to existing ones or replace the existing estimate.
- **Edit labels and sequence numbers:** Assigns the same Label, Label Number Prefix, and/or sequence number to the selected objects.
- **Mark selected objects as received:** Assigns the selected objects a received date based on the date the delivery they were part of was received.
- **Remove from collection:** Dissociates the selected objects from any collection.
- **Remove from container:** Deactivates relationships between the selected objects and their current containers.
- **Select all:** Selects all of the found objects for subsequent actions.
- **Select none:** Deselects any previously selected objects in the found set.
- **Update object locations:** Updates the location for all selected objects. Locations for objects in containers or part of deliveries that have not been received will not be updated.

## Deactivate

Object records are not deleted, except in very specific circumstances. Instead, they are made inactive. SPEC records the person who deactivates an object, the date it became inactive, and requires the deactivator to enter a reason for deactivation.

Object records can be deactivated by selecting **Deactivate** in the action menu to the left of objects in **Object Search** results or in the top right-hand corner of an **Object Record**.

### To deactivate an object:
1. Click **Deactivate**.  
2. The **Deactivate Object Record** window will open. Select a reason for deactivating the object and enter notes as appropriate.

**Note:** You cannot deactivate a container if it contains other objects.

### Deactivating a record will:
- Cross-out the object name.
- Deactivate any existing content estimates and descriptions.
- Resolve all existing issues.
- Change the accessibility status to “not available to public” and the description status to “not described.”

### Acquisition Proposal
To deactivate an object prior to acquisition, click the blue **X** to the left of the object. The object will no longer appear in the proposal inventory, but it will appear in the **Acquisition (Check-In) Inventory**.

### Acquisition (Check-In) Inventory
To deactivate an object, click the blue **X** to the left of the object. To reactivate a record deactivated in error, click the green **X**.

---

## Reactivate

If an object record was deactivated in error, it can be reactivated by selecting **Reactivate** in the action menu to the left of objects in **Object Search** results or in the top right-hand corner of an **Object Record**.

### Reactivating a record will:
- Reassign the object to its last location.
- Make previously resolved issues unresolved (since deactivating a record resolves all associated issues).
- Make all restrictions active again.
- Make all content estimates active.

**Note:** 
- Relationships between the object and any objects it contained, or the container it was in, will not be restored and will need to be re-entered manually.
- The accessibility status will remain “not available to public” and “not described,” and must be adjusted manually.