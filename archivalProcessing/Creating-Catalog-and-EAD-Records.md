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

![Complex subjects](/Images/132-complex-subjects.png)

Also be sure that locations are labeled as _geographic_ in the _type_ field.

![Geographic subdivision](/Images/133-geographic-subdivision.png)

Make sure authorized terms are not marked as _local_, and that the _source_ and _authority ID_ are included. 

![ASpace subject](/Images/134-ASpace-subject.png)

5. Check that all containers were assigned a **container type**, **indicator**, and **barcode** in the top containers list for the collection. If the container type is omitted, terms like “box” or “tube” will be omitted in the XML.

6. Export the MARCXML.

Go to the export menu and select _Download MARCXML_ as illustrated below.

![export XML](/Images/135-export-xml.png)

## Converting XML to MRC in MarcEdit
Since ASpace generates the catalog information as MARCXML, you need to use MarcEdit to convert this data into a MARC format that can be imported into OCLC Connexion. 

**NOTE** 
**If you are cataloging an addition, you should skip directly to the section on 
[Updating Existing Catalog Records]().**

To convert XML to MRC, follow the steps below:

1. Open MarcEdit.

2. Go to the File menu and select Open.

3. A navigator window will open that only shows mrk files.

4. In the dropdown menu at the bottom right of the menu select all files.

5. Open the MARCXML file that was exported from ASpace.

6. The **MARC 901** field will look like this: 

        901  \\$a---$b---

- Replace the three dashes after _&a_ with your initials
- Replace the dashes after _$b_ with: **archv**

7. The **MARC 949** (container list) will include the following fields:
        - collection identifer (call number)
        - 5 digit location code
        - barcode
        - container type and number
  
  Each line of the container list will end like this:
        
        - $v---/---

  Replace the dashes after _$v_ with **archv**
  Replace the --- after the / with your inititials

It is recommended you do this with a find and replace.

8. When you have finished editing the record, save it as a .mrc file. Do this by going to _file_ and _save as_, or select the compile records icon.

9. Once you have saved your _.mrc_file you are ready to import the record into OCLC Connexion. 

## OCLC Connexion: Importing Catalog Record into WorldCat and Exporting into Sierra

**_\*NOTE: If you are cataloging an addition skip directly to the section on_** [**_Updating Existing Catalog Records_**]()**_. Do not import a new MARC record into OCLC. Instead you will be editing the existing Worldcat record._**

All catalog records are published via OCLC on [Worldcat](https://www.worldcat.org/). OCLC also has extensive [documentation](https://help.oclc.org/Librarian_Toolbox) available, including information on their [Bibliographic Formats and Standards](https://www.oclc.org/bibformats/en.html) site, which includes rules for MARC fields, indicators, and subfields. Before you can catalog in OCLC you will need to request an OCLC account through ServiceNow.

1. Log in to OCLC Connexion.

The first time you login to OCLC Connexion, or if you are logging onto OCLC Connexion for the first time on a new device or newly updated device, you will need to set up your OCLC Connexion Gateway Connection. There are [instructions](https://docs.google.com/document/d/1jHuEKAkd8eODzWFgioFsBN_lArdyln-L2t66Y5CBMj0/edit?usp=sharingkUcbRIIpfp/edit?usp=sharing\&ouid=101547597784973669792\&rtpof=true\&sd=true) available from BookOps to set up your account.

2. Import the .mrc file. 

Go to the File menu and select Import Records.

![OCLC Import](/Images/136-OCLC-Import.png)

Navigate to your saved .mrc file, and check the _Import to Online Save File_ radio button.

![online save file](/Images/137-online-save-file.png)

When the dialogue box asks _Do you want to delete your original import file?_ select _No_.

![Delete file box](/Images/138-delete-file-box.png)

3. Locate and open the newly imported file.

Go to _Cataloging > Search > Online Save File,_ and search for the collection by title.

![search online save file](/Images/139-search-online-save-file.png)

4. When the new record opens, validate it to check for errors.

Select _Edit > Validate_ or the green check icon to identify errors in the record.

There will be no message if there are no errors.

Select _Edit > Reformat or the _R_ icon to organize the order of the record’s fields.

5. Correct errors if any are indicated after validation. 

**Some common errors include:**

**Diacritics**

You need to add diacritics manually in OCLC. 

Place the cursor after the letter that the diacritic will modify, and navigate to _Edit_ > _Enter Diacritics._

![Enter Diacritics Menu](/Images/140-enter-diacritics.png)

A menu of diacritics will open. You can select the correct language from the dropdown menu, which will show the most common diacritics for that language. 

![Diacritics Menu](/Images/141-diacritics-menu.png)

Choose the correct diacritic, and then select _insert and close._

**Dates**

If the whole collection contains only a _single date_, not inclusive dates, change the **_DtSt_** field at the top from **_i_** for _inclusive dates_ to **s** for _single date_.

**Meeting Names** 

[MARC 611](https://www.oclc.org/bibformats/en/6xx/611.html) (e.g. names of conferences, festivals, etc.)

These are entered into ASpace as corporate names and will output into the MARC record as a [MARC 610](https://www.oclc.org/bibformats/en/6xx/610.html) field. Change the field to a [MARC 611](https://www.oclc.org/bibformats/en/6xx/611.html). 

**245 Field Error**

If you are cataloging an artificial collection that does not have a _main entry_, you will get an error message about the _Title Statement_ \[[MARC 245](https://www.oclc.org/bibformats/en/2xx/245.html)] field. 

![MARC 245 Error](/Images/142-MARC245-error.png)

Change the first indicator in the 245 field from a 1 to a 0. This indicates that there is no added entry for the title field, and will allow the record to validate.

**910 Field**

All materials cataloged for the Research Libraries must include a 910 field. Make sure this field is included. This field is automatically generated by ArchivesSpace in the MARCXML export.






