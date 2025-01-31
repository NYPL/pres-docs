---
title: Issues
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 8
---

{: .note }
> This page is under construction! 
> Content is being edited ...

## Issues
*optional, multiple values*

The issues section of an object record is used to record preservation issues discovered during any assessment, as well as their resolution. Whenever an issue is recorded, SPEC automatically creates a corresponding assessment record if there is no record covering the date the issue was discovered.

### Issue Type
*required, single controlled value*
The type of issue entered determines the available choices for the specific issue field.


### Noted Date
*required, single date value*

The date the issue was noticed. SPEC automatically fills in the date that the issue is entered by default.

### Noted By
*required, single controlled value*

The staff member who noticed the issue. SPEC fills in the username of the logged-in user who entered the record by default.

### Rating
*required for condition issues -> structural damage,  single numeric value*

The severity of structural damage. 1: minimal, 2: moderate, 3: severe.

### Resolved On
*optional, single date value*

The date an issue was resolved.

### Resolved By
*as needed, single controlled value*

Enter the username of the staff member who resolved the issue.

### Assessment
*optional, single controlled value*

Use this field to indicate a named assessment during which the issue was noticed.

### Notes
*optional, free text*

Use this field to enter any additional information about the issue and its resolution.
