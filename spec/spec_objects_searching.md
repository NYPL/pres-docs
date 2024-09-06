---
title: Searching SPEC Objects
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 1
---

# Searching SPEC Objects

## Basic Search

Click **Search all objects** on the **SPEC landing page** to navigate to the **Object search page**.

You can search for objects using one or a combination of the following elements:

| **Search Field**                    | **Use to search for:**                                                                                     |
|-------------------------------------|------------------------------------------------------------------------------------------------------------|
| **Description Keyword**             | Keywords that may appear in the object title/label, collection, or acquisition title.                       |
| **Any ID**                          | Object barcodes, label numbers, any references, or location barcodes.                                       |
| **Format Keyword**                  | Formats (of individual objects and content estimates), container types, and media.                          |
| **ID / Classmark**                  | Any part of any ID associated with a collection, including barcodes.                                        |
| **Division**                        | Curatorial division acronyms.                                                                               |
| **Barcode**                         | Object barcode.                                                                                             |
| **Object ID**                       | Object identifier.                                                                                          |
| **Shelf Barcode**                   | Shelf identifier.                                                                                           |
| **Label Number**                    | Object label details, including AMI identifiers.                                                            |
| **Object Type**                     | Select "container" or "item."                                                                               |
| **Status**                          | Search for objects whose status is active, inactive, or both.                                               |

> **Note:** Searches, by default, will only return Active records unless Inactive is selected in the Status search field.

---

## Advanced Search

> **Note:** The Advanced Search feature is currently in beta/testing. Some functionalities may be subject to change or limited availability.

**Advanced searches** allow users to search using a single field or a combination of over 90 object fields. Click **Advanced search** on the **Object search page** to open the Advanced Search window, which offers the following options:

- **Exclude Inactive Records**:  
  Searches automatically exclude inactive records. Click the box next to **Include inactive records** to include them.

- **Include Objects on Shelf**:  
  Searches automatically include objects on the shelf and objects contained in other objects. Click the box next to **Include only objects on shelf** to exclude objects contained in other objects.

- **Format Searches**:  
  Format searches include formats associated with objects and their content estimates.

- **Date and Number Ranges**:  
  Enter date and number ranges using "..." between terms (e.g., `12/4/2021…1/22/2022`, `17…25`). Click the **?** icon for tips on using wildcards and other special search characters.

- **Clear Terms**:  
  Clears all entered values for the fields selected.

- **Reset**:  
  Resets all fields and clears any entered values.

### Adding Search Criteria:
1. Click **+** to add a search criterion.
2. Select a **boolean operator** (AND is the default).
3. Click the gray **(** to parenthesize the current and following criteria, turning the parenthesis green.
4. Select a **field** to search.
5. Enter or select a **search term**.
6. Click the gray **)** to close any open parentheses, turning it green.

---

## Object Barcode App

The **Object Barcode App** allows users to quickly look up and view basic details about objects and container contents.

To access this tool, click **Object Barcode App** on the **SPEC Landing page**. From there, users can click on an object name to view the full Object Record.

---

## Collection Records

From the **SPEC Landing page**, select **Search all collections**, search for a collection, and click on the collection name to open the **Collection Summary**.

### Search
Use any combination of the following fields to formulate a search. Results will include records matching all of the search criteria.

| **Search Field**                | **Use to search for:**                                                        |
|---------------------------------|-------------------------------------------------------------------------------|
| **Collection Creator or Title** | Keywords that may appear in the collection title or creator.                  |
| **Division**                    | Curatorial division acronym.                                                  |
| **ID / Classmark**              | Collection ID or collection-assigned classmark.                               |
| **Center**                      | Research center.                                                              |

---

### Searching Within a Collection

From the **Collection Record**, you can call up a list of objects in two ways:

1. **From the SPEC Records section**:  
   Click on the **object count** next to **Objects**. This will show you a list of all known objects related to the collection.

   > **Note:** When navigating to a list of objects from a Collection Summary, all new object records you create will be assigned to that collection. Click **Clear** to deactivate this function.

2. **From the Object Counts by Format Category section**:  
   Click **View list** to the right of any **FORMAT** listed to call up a list of objects filtered by format.

### Searching Objects Within a Collection

You can perform a search of objects within a collection by clicking the **magnifying glass icon** next to the Objects count. The fields available in this search are:

- **Object Type**
- **ID Number Prefix**
- **ID or Sequence Number**
- **Title or Label**

---

## Acquisition Records

You can find objects through an **Acquisition Record** in three ways:

1. In the **Extent Summary** section of the **Acquisition Summary**, click **Go to inventory** to call up a list of objects.
2. In the **Extent Summary** section of the **Acquisition Summary**, click **Go to format summary** to call up a list of objects grouped by format. From here, you can click on any category to call up a format-specific list of objects.
3. In the **Inventory** section of the **Acquisition Proposal / Edit** page, click **Go to inventory**

---

## Searching Objects Within an Acquisition

You can also perform a search for objects within a collection by clicking the **magnifying glass** next to the **EXTENT SUMMARY** label. The available fields in this search are: Object Type, ID Number Prefix, ID or Sequence Number, and Title or Label.

## Interpreting Search Results

The object list provides key details for each object, including:
- **Icon**: Visually represents the format or container type. Hover over the icon to see the format name displayed in a tooltip.
- **Object Name**: The name of the object.
- **Curatorial Division**: The division responsible for the object.
- **Acquisition Name**: Displays if the object is part of an acquisition but hasn't been associated with a collection yet, or if the object has been received but not yet linked to a collection.
- **Collection Name**: Displays if the object is assigned to a collection.
- **Current Location**: Where the object is currently stored.
- **Container Icon**: Represents the container storing the object. Hover over the icon to see the container's name, or click to view the container’s object record.

### Object Status Colors:
Objects that are part of acquisitions appear with different colors, indicating their status:
- **Gray**: Object is part of a delivery that has not yet been received.
- **Green**: Object is part of a received delivery but hasn’t been marked as received.
- **Blue**: Object has been marked as received.

---

## Sorting

Search results are typically returned unsorted. You can sort them by clicking any of the search result headers to sort alphabetically either in ascending or descending order.