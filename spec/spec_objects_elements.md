---
title: Object Record Elements
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 4
---

# SPEC Object Record Elements

## Type
**Required.** Single controlled value.

There are two types of objects:

### Items
Items are objects that constitute the Research Libraries collection, such as books, sound recordings, manuscripts, and digital files. In the context of SPEC, the term *item* has a more specific and literal meaning than it does in the context of the catalog, where an “item record” can represent one or more items.

An item in SPEC is always a single thing that is not a container. Bound volumes, such as a book or manuscript diary, are considered a single item, although the pages within them are also considered items.

Items in SPEC are physical or digital objects, not intellectual or bibliographic entities. For example, an unbound 40-page manuscript of a short story is not a single (manuscript) item, but 40 items (see the *Relationships* section for details).

### Containers
Containers are objects containing items and/or other containers. Containers are not considered part of the Research Library’s collection and are also distinct from storage locations since they are not fixed to a physical place. The contents of containers can be represented in SPEC in two ways: with related object records or content estimates.

## Status
**Required.** Single controlled value.

An object’s status is either *active* or *inactive*. Inactive objects are no longer held by the Library. Examples of inactive objects are:
- an item or container that was part of a proposed acquisition but was not acquired
- an item that was deaccessioned
- a container that was replaced during rehousing
- a record that was created in error

The SPEC object record displays the status of an object in its header, along with certain qualifying details:
- Active From: the date the object became active, usually the date it was created
- Inactive Since: the date on which the object became inactive
- Reason deactivated: available in the object deactivation window reached by clicking the Inactive Since date.

When objects are inactive, their names are displayed crossed out in the Object Search results list, and other headers.