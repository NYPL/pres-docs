---
title: References
layout: default
parent: SPEC Objects
grand_parent: SPEC
nav_order: 6
---

{: .note }
> This page is under construction! 
> Content update in progress ...

## References
*as needed, multiple controlled values*

Object references are alternate identifiers assigned to an object, such as an AMI id or other legacy id. In many cases, references point to related records within SPEC or other databases such as ArchivesSpace, Archives Portal, or Sierra; SPEC provides links to those records whenever possible. Often, multiple objects share a particular reference, such as an acquisition id or a collection id, grouping sets of objects together in specific contexts. References are often created and revised in the course of actions taken in SPEC, processes being tracked within SPEC, and data imports from other systems.

References that refer to other record types in SPEC include CMS acq delivery id, CMS acquisition id, and CMS collection id. Each acquisition can be associated with one or more deliveries, however each delivery is only assoicated with one acquistion; adding a delivery reference to an object automatically adds the associated acquisition id. Collections can be associated with one or more acquisitions, and an acquisition can be associated with one or more collections. Linking a collection to an acquisiton does not automatically cause the objects assoicated with the acquisition to inherit the collection reference. ... [MORE DETAILS FORTHCOMING] ... All newly created objects in SPEC should be assoicated with an acquisiton and delivery ids, however objects do not need to be associated with a collection. 

SPEC Project IDs [SPEC PROJECTS DOCUMENTATION FORTHCOMING]

CMS AMI id, also referred to as simply AMI id, is the SPEC generated id assigned to all AMI items. This reference is not editable. See [Basic Fields](https://nypl.github.io/pres-docs/spec/specObjectsBasicFields.html#ami-id) for more information.  

The cat bnumber refers to the corresponding bibilographic record in Sierra (the library catalog) and the cat item record referst to the Sierra item record. Additionally, classmarks can be either imported or added manually to objects. see for more 

References imported from ArchivesSpace are the ASpace archival object id, ASpace top container id, ASpace multiple identifer record id, other id (ASpace); references imported from the Archives Portal are Archives Portal component id, Archives Portal collection id. These references are not editable manually. 

Other editable object references are accession number, conservation id, other legacy id, separation id, TL number.

Additional ids associated with other databases are MMS capture UUID, Preservica ...

Legacy reference types include the CMS AMI dig batch id (superceded by SPEC Project IDs), CMS digital media log legacy id, CMS item id, CMS ingest report import record id, CMS project id (superceded by SPEC Project IDs), Rose Building temporary id.