---
title: Editing SPEC Objects
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 3
---

# Objects Editor

[Screenshot pending]

To access and edit the most common object record elements, use the Objects Editor. The Editor can be accessed from a number of different contexts:
- **Object Search or List Object Editor:** click on the action button to the left of an object’s name in the search results and select Edit object record.
- **Object record:** click directly on any blue-underlined field (for example, a barcode) to open the Editor.

You can edit most object elements from the Basic Fields screen. For a list of object elements and their definitions, see [SPEC Object Record Elements](https://nypl.github.io/pres-docs/spec/spec_objects_elements.html#spec-object-record-elements).

The Basic Fields screen includes a navigation bar at the top that can be used to toggle between other common object elements/element groups, including Media, Relationships, References, Restrictions, Issues, Locations and Estimates.

# Object Editing Guide

# SPEC Object Elements

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

---

## Formats / Container Types

In the **List Object Editor** and the **AMI object list**, you can add or edit an object’s format or container type using dropdown menus for each field. The available values depend on the type of object (item or container) and other selected values.

### Keyword Search

To navigate format hierarchies more easily, SPEC provides an option to keyword search available format terms in the **Basic Fields Editor**.

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

Objects are often related to other records within and outside SPEC. For example, an object may be linked to a **SPEC acquisition record**, a **finding aid** in the Archives Portal, or a **record** in the NYPL catalog. These relationships are called **references**.

To add or edit a reference:

1. Click **View All / Edit / Add** in the **REFERENCES** section of the **Object Record**.
2. Click the `+` button to add a new reference.
3. Select the reference type from the dropdown menu.
4. Manually enter the reference; some references may be searched for (Collections, Acquisitions, or Acquisition Deliveries).

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