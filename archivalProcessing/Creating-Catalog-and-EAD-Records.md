---
title: Creating Catalog and EAD Records
layout: default
parent: Final Steps
grand_parent: Archival Processing
nav_order: 8
has_children: false
---
# Creating Catalog and EAD Records
{: .no_toc }
Once your finding aid has been approved by the curator, your supervisor will move the collection’s Trello card to the _Ready to Ship_ column of the _Processing Projects_ Trello. Collections need to be cataloged before they can be shipped offsite. Below are the steps to create a catalog record and to generate an EAD record. 

**If you are cataloging an addition, you should skip directly to the section on [Updating Existing Catalog Records]()** 

Catalog records will appear in both [WorldCat](https://www.worldcat.org/) and the [NYPL catalog](https://www.nypl.org/research), and uploaded EAD records will appear in the [Archives Portal](http://archives.nypl.org/).

## Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Initial Steps in ArchivesSpace

1. Open the collection's resource record in ArchiveSpace.

2. The following fields are required. Make sure they are all included and written correctly.

| FIELD NAME | DACS RULE | EAD TAGS | RDA RULE | MARC FIELDS | SUMMARY |
| ---------- | --------- | -------- | -------- | ----------- | ------- |
| Languages and Scripts of the Material | [DACS 4.5](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/05_languages_and_scripts_of_the_material.html#purpose-and-scope) | <[langmaterial](https://www.loc.gov/ead/tglib/elements/langmaterial.html)> | [RDA 6.11](https://original.rdatoolkit.org/document.php?id=rdachp6\&target=rda6-3469#rda6-3469) | [MARC 041](https://www.loc.gov/marc/bibliographic/bd041.html) | The language(s), script(s), and symbol systems employed in the materials being described. |
| Main Entry[^1] | [DACS 2.6](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/06_name_of_creators.html) | [\<origination> \<persname>](https://www.loc.gov/ead/tglib/elements/origination.html)[\<origination> \<famname>](https://www.loc.gov/ead/tglib/elements/origination.html)[\<origination> \<corpname>](https://www.loc.gov/ead/tglib/elements/origination.html) | [RDA 19.2](https://original.rdatoolkit.org/document.php?id=rdachp19\&target=rda19-393#rda19-393) | [MARC 100](https://www.loc.gov/marc/bibliographic/bd100.html) (Main entry-- personal name)[MARC 110](https://www.loc.gov/marc/bibliographic/bd110.html) (Main entry-- Corporate name) [MARC 111](https://www.loc.gov/marc/bibliographic/bd111.html)(Main entry -- meeting name) [MARC 130](https://www.loc.gov/marc/bibliographic/bd130.html)(Main entry -- uniform title) | Identifies the corporate bodies, persons, and families associated with the creation, assembly, accumulation, and/or maintenance and use of the materials being described.ASpace will automatically add the “$ecreator” relator term.  Add a relator term if the main entry is not the creator (this is uncommon).Each collection can have only ONE main entry. |
| Date | [DACS 2.4](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/04_date.html) | [\<unitdate>](https://www.loc.gov/ead/tglib/elements/unitdate.html) | [RDA 2.7.6](https://original.rdatoolkit.org/document.php?id=rdachp2\&target=rda2-6289#rda2-6289) | [MARC 264](https://www.loc.gov/marc/bibliographic/bd264.html)$c | Date or date range of materials being described. |
| Extent | [DACS 2.5](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/05_extent.html) | [\<physdesc>](https://www.loc.gov/ead/tglib/elements/physdesc.html) [\<extent>](https://www.loc.gov/ead/tglib/elements/extent.html) | [RDA 3.4](https://original.rdatoolkit.org/document.php?id=rdachp3\&target=rda3-2079#rda3-2079) | [MARC 300](https://www.loc.gov/marc/bibliographic/bd300.html) | Total collection extent, including physical and digital materials. |
| Conditions Governing Access | [DACS 4.1](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/01_conditions_governing_access.html) | [\<accessrestrict>](https://www.loc.gov/ead/tglib/elements/accessrestrict.html) | [RDA 4.4](https://original.rdatoolkit.org/document.php?id=rdachp4\&target=rda4-120#rda4-120) | [MARC 506](https://www.loc.gov/marc/bibliographic/bd506.html) | The portal automatically generates this note for each division. Optional additional notes regarding access to audio and moving image material, electronic records, and any other restrictions can be added here. |
| Abstract | Commentary to [DACS 3.1](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/01_scope_and_content.html) | [\<abstract>](https://www.loc.gov/ead/tglib/elements/abstract.html) | [RDA 7.10](https://original.rdatoolkit.org/document.php?id=rdachp7\&target=rda7-773#rda7-773) | [MARC 520](https://www.loc.gov/marc/bibliographic/bd520.html) | A brief summary overview of the collection.This can include biographical and content information. |
| Immediate Source of Acquisition | [DACS 5.2](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/02_immediate_source_of_acquisition.html) | [\<acqinfo>](https://www.loc.gov/ead/tglib/elements/acqinfo.html) | [RDA 2.19](https://original.rdatoolkit.org/document.php?id=rdachp2\&target=rda2-8636#rda2-8636) | [MARC 541](https://www.loc.gov/marc/bibliographic/bd541.html) | The source of the acquisition and the year in which it was received. |
| Reference Code/ Call number/ Identifier | [DACS 2.1](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/01_reference_code.html) | [\<unitid>](https://www.loc.gov/ead/tglib/elements/unitid.html) | [RDA 2.20](https://original.rdatoolkit.org/document.php?id=rdachp2\&target=rda2-8658#rda2-8658) | [MARC 852](https://www.loc.gov/marc/holdings/hd852.html) | If this field is missing the 949 (item records) will not export. |

[^1]: If the collection is an artificial collection created by the Library, do _not_ include a _main entry._ Instead record the Library division as a _creator/contributor_. If a record does not have a 1xx field, change the first indicator of  the 245 field to 0. See the [Main Entry](https://nypl.github.io/pres-docs/archivalProcessing/Controlled_Access_Terms.html#main-entry) section of this documentation for more information.

3. Verify all [Agents](https://nypl.github.io/pres-docs/archivalProcessing/Controlled_Access_Terms.html#agents) are formed correctly.

Add [relator terms](https://nypl.github.io/pres-docs/archivalProcessing/Controlled_Access_Terms.html#creatorcontributor) for [MARC 700](https://www.loc.gov/marc/bibliographic/bd700.html)/[710](https://www.loc.gov/marc/bibliographic/bd710.html) (i.e. added authors).

![Relator Term](/Images/127-Relator-term.png)

**Contributor (ctb)** is the most common relator term. See the [LSCH MARC Code List for Relators](https://www.loc.gov/marc/relators/relaterm.html) for more information. 

[MARC 600](https://www.loc.gov/marc/bibliographic/bd600.html)/[610](https://www.loc.gov/marc/bibliographic/bd610.html) (subjects) DO NOT need relator terms. Make sure all agents being used as subjects have been added to the agents section, not as topical subjects. 

If the Library of Congress authority record indicates an agent uses RDA rules,  add _Resource Description and Access_ in the _Rules_ field in ASpace.

![MARC RDA](/Images/128-MARC-RDA.png)

![ASpace RDA](/Images/129-ASpace-RDA.png)

If the agent is from a source other than the Library of Congress, or if the Library of Congress authority record does not indicate a name was derived using RDA rules, then leave the _Rules_ field blank as illustrated below. 

![Not RDA](/Images/130-not-RDA.png)

![ASpace Not RDA](/Images/131-ASpace-not-RDA.png)

Make sure the authority identifier is entered correctly. For Library of Congress authority records, make sure to copy the number exactly as it appears in the authority record, preserving any spaces that may be present. 

4. Verify that [Subjects](https://nypl.github.io/pres-docs/archivalProcessing/Controlled_Access_Terms.html#subjects) are formed correctly.

For complex subjects, make sure there is only one term in each field. Remember that subdivision terms each get their own field.



