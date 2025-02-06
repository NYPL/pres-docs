---
title: Finding Aid Notes
layout: default
parent: Archival Description
grandparent: Archival Processing
nav_order: 4
has_children: false
---
# Finding Aid Notes
{: .no_toc }
This section identifies the notes fields included in a finding aid’s front matter, detailing the required and optional elements, DACS rules, equivalent MARC fields (when applicable), and EAD tags. This section will explain which notes to add in ASpace, and includes recommendations about how to structure narrative sections. Also be sure to reference the [Inclusive Description and Style Guidelines](/Inclusive_Description.md) section of this manual to make sure your notes correspond to the Archival Processing unit’s description standards. 

The [Archives Portal](https://archives.nypl.org/) automatically generates certain notes fields including:

Preferred Citation \[[DACS 7.1.5](https://saa-ts-dacs.github.io/dacs/06_part_I/08_chapter_07/01_notes.html#citation)]

Repository Name and Location \[[DACS 2.2](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/02_name_and_location_of_repository.html)]

General Conditions Governing Access Statement \[[DACS 4.1](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/01_conditions_governing_access.html)]

Series Arrangement Note \[[DACS 3.2](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/02_system_of_arrangement.html)]

## Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Required Fields
The Archival Processing unit requires the following notes fields in all finding aids:

| Field Name | DACS Rule | EAD Tag | MARC Field |
| ---------- | ----------| -------- | --------- |
| Abstract | Commentary note to [DACS 3.1](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/01_scope_and_content.html) | [\<abstract>](https://www.loc.gov/ead/tglib/elements/abstract.html) | [MARC 520](https://www.loc.gov/marc/bibliographic/bd520.html) |
| Conditions Governing Access | [DACS 4.1](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/01_conditions_governing_access.html) | [\<accessrestrict>](https://www.loc.gov/ead/tglib/elements/accessrestrict.html) | [MARC 506](https://www.loc.gov/marc/bibliographic/bd506.html) |
| Immediate Source of Acquisition | [DACS 5.2](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/02_immediate_source_of_acquisition.html) | [\<acqinfo>](https://www.loc.gov/ead/tglib/elements/acqinfo.html) | [MARC 541](https://www.loc.gov/marc/bibliographic/bd541.html) |
| Administrative/Biographical History | [DACS 2.7](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/07_administrative_biographical_history.html) | [\<bioghist>](https://www.loc.gov/ead/tglib/elements/bioghist.html) | n/a |
| Processing Information | [DACS 7.1.8](https://saa-ts-dacs.github.io/dacs/06_part_I/08_chapter_07/01_notes.html#processing-information) | [\<processinfo>](https://www.loc.gov/ead/tglib/elements/processinfo.html) | [MARC 583](https://www.loc.gov/marc/bibliographic/bd583.html) |
| Scope and Content | [DACS 3.1](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/01_scope_and_content.html) | [\<scopecontent>](https://www.loc.gov/ead/tglib/elements/scopecontent.html) | n/a |

### Abstract
A finding aid’s abstract should serve as a clear and concise synopsis of the collection’s scope, content, and creator biography. Ideally, an abstract should be three sentences, briefly summarizing the collection creator’s biography in a single sentence, and the scope and content in two sentences. The abstract should clearly reveal what the collection documents, as well as the types of materials it contains. It is best to avoid simply listing out the formats a collection holds, and instead to clarify the types of records a researcher can expect to find. While [DACS](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/01_scope_and_content.html_system_of_arrangement.html#32-system-of-arrangement-added-value) does not require abstracts, it is a required field at NYPL.

The abstract is the only narrative descriptive element that is included in the catalog record, since neither the _scope and content_ or _biographical/historical_ note have MARC equivalents in NYPL catalog records. The abstract, along with the access terms, have a great deal of significance in quickly summarizing a collection’s content in the catalog. Additionally, the abstract appears directly under a finding aid’s basic information in the archives portal, and may be the first descriptive details a researcher encounters. 

### Conditions Governing Access
The purpose of this statement is to describe access restrictions imposed by NYPL, or those which were stipulated in the deed of gift or purchase agreement. [DACS 4.1](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/01_conditions_governing_access.html) describes when to use a _Conditions Governing Access_ note. The archives portal will automatically generate a _Conditions Governing Access_ statement for each curatorial division. If the collection you are processing has no special access restrictions, then you do not need to complete this field. The automatically generated [standard access notes](aspace/aspace.md) are listed in the ASpace User Guide. If the collection has additional restrictions, such as electronic records or audio and moving image material that is unavailable, or restrictions requested by the donor, then you must create a _Conditions Governing Access_ note to explain the restrictions.

For collections containing audio and moving image, use the correct division statement, both in the front matter, and at the level immediately above the audio and moving image components. See the [Description of Audio and Moving Image Material in ArchivesSpace]() section of this documentation for each division's access note language. 

When a component in a finding aid is restricted or should not be requested in the reading room, you use use the terms **_closed_** or **_Unavailable_** in the <accessrestrict> note at the component-level. This will assure that the item is not requestale in Aeon. 

### Immediate Source of Acquisition 
This field describes the source from which NYPL acquired the collection, the date it was acquired, and whether it was purchased or donated. A typical _Immediate Source of Acquisition_ statement is constructed liked this: Purchased \[or donated] from \[by] \[donor/seller name] in \[year]. This information is found in the deed of gift or purchase agreement, which is located in the collection’s acquisition record (or in the dossier for legacy collections). For further guidance on this note, see [DACS 5.2](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/02_immediate_source_of_acquisition.html).

### Administrative/Biographical History
Although you most likely already drafted a solid _Administrative/Biographical History_ note in your [processing proposal](/Processing_Proposal.md), it is common to encounter additional pertinent information as you process the collection. Therefore, your note will often change slightly from its initial iteration. Remember that it is not your job to construct an overly detailed biography of the collection’s creator. Instead, you should aim to summarize the collection creator’s history in a manner that reflects the content of the collection.

Typically an _Administrative/Biographical History_ is written in chronological order, and includes the creator’s date and place of birth, or the founding members and date of creation, if the collection’s creator is a corporate body. The _Biographical/Historical_ note should also include the creator’s activities as they relate to the materials held in the collection, or the primary functions of the institution for corporate bodies. It is also recommedned that you include the individuals with whom the creator collaborated, the creator’s current activities, and the date of death/dissolution if known/applicable.

[DACS 2.7](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/07_administrative_biographical_history.html) lays out the guidelines for writing a _Biographical/Historical_ note for various types of collections, and includes guidance on what types of details should be included, as well as what belongs in different note fields. In general, collections from famous and well-documented individuals do not require extensive biographical details because that information is easily attainable elsewhere. Your _Biographical/Historical_ note should be sourced from the collection materials as much as possible. When you need to verify certain dates or facts, consult external primary source databases that index documents such as census records, draft cards, and death certificates. The Archival Processing unit has compiled a [list](https://docs.google.com/spreadsheets/d/1IALH_cfVpQqFGuezhwXk8GIFglJqinsXqw3lRtqp9RQ/edit?usp=sharing) of recommended resources for this purpose. 

If you use external sources to write your _Biographical/Historical note_, it is good practice to compile your sources and research, and to save this information in the acquisition folder. When applicable, you can choose to cite your sources using [Chicago Style](https://www.chicagomanualofstyle.org/home.html) citations at the end of your _Biographical/Historical note_. This is generally not necessary. 

For most finding aids the only _Administrative/Biographical History_ note will be at the collection level. It is very uncommon and not usually necessary to add additional biographical notes to the series or subseries levels of a finding aid. If the collection was created or assembled by multiple individuals, you should describe all of them and their relationships to each other in the _Administrative/Biographical History_ note. 

When writing the biographical note, make sure you are describing individuals using the terms and identities they would use to describe themselves. Avoid using overly laudatory language when writing a biography,[^1] and also be sure to not conceal problematic or racist histories when these are known. It is okay to be uncomfortable with a creator’s biography, but it is not okay to allow this discomfort to prevent you from constructing a historically accurate biography.[^2]

When working with additions being processed as a discrete collection, or if the materials are separated from a collection with an existing finding aid on the archives portal, it is often preferable to reuse the existing _administrative/biographical history_ note. If you do use the existing note, you may still need to edit the note for clarity, or modify it to correspond more accurately with the materials you are describing. If you reuse existing description, you must always attribute the note to its original author. Examples of finding aids that utilize this practice include:

- [Harry Belafonte photographs](https://archives.nypl.org/scp/186084)
- [Stormé DeLarverié photographs](https://archives.nypl.org/scp/186079)
- [George Westerman photographs](https://archives.nypl.org/scp/186080)

If there is additional interesting information that you encountered during processing that is outside the scope of an _Administrative/Biographical History note_, you can always include these details in a Wikipedia article and mention them in your closing memo. Consult the [Updating and Creating Wikipedia Entries]() and [Closing Memo]() sections of this manual for more information.

### Processing Information
All finding aids must include a _Processing Information_ note, which states the name of the archivist that processed the collection, and the year(s) it was processed. All processing notes must be formatted like this with EAD tags: Processed by \<name>Archivist Name\</name> in \<date>Year\</date>.[DACS 7.1.8](https://saa-ts-dacs.github.io/dacs/06_part_I/08_chapter_07/01_notes.html#processing-information) contains more information on processing notes.  

### Scope and Content
A finding aid’s _scope and content_ note is the central tenet of a collection’s description, serving as the core narrative to convey the types of materials that comprise a collection, and the function of those materials. The _scope and content_ note should be utilized to describe why the records were created, how they were used, and what activities they chronicle. It is also a space to describe the types of materials the collection holds. 

A _scope and content_ note should be structured hierarchically, beginning with a general overview of the collection, and using successive paragraphs to address each subsequent level. Begin your note with the most high-level information, such as the collection’s date range and a synopsis of what information the collection conveys. This opening paragraph should be similar to what you would include in an _abstract_, and the following paragraphs should get progressively more granular in a manner that adequately describes what the collection holds, and also explains this in a way that mirrors how the collection is arranged. 

The focus of your _scope and content_ note should be on why the records were created, their value to the individual who created them, and what events, subjects, or topics the collection documents. While it can be useful to note that a collection contains certain genres of material, it is not advisable or useful to simply list format types, or to go into a great level of detail about the specific media formats held in a collection. 

The amount of detail included in a _scope and content_ note depends upon the degrees of hierarchy and levels of description the collection requires. The [Levels of Description](/Guidelines_for_Levels_of_Description.md) section of this documentation is included to help you determine how much description is necessary in your finding aid. If you choose to use series and/or subseries, then the _scope and content_ note in the front matter should contain only a high-level description of the collection as a whole, and more detailed description of the materials held within each series or subseries should be relegated to the series or subseries-level _scope and content_ notes. In multilevel description, you should avoid repeating the same information you stated at a higher level of the finding aid. DACS [Requirements for Multilevel Description](https://saa-ts-dacs.github.io/dacs/06_part_I/02_chapter_01.html#requirements-for-multilevel-descriptions) indicates that higher-level description is inherited by each subsequent level. 

In archival description it is just as important to note what is not found in the collection, as it is to describe what is contained in the boxes, folders, and files of a collection. The context of certain files may be unclear, or noticeable omissions may be present. Always try to be cognisant of what you choose to describe, and consider if you may be inadvertently excluding marginalized or underrepresented voices. Attempt to highlight silences when you encounter them, and consider the power dynamics that may have resulted in these exclusions. [^3]

[DACS 3.1](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/01_scope_and_content.html) provides general guidance on writing an effective and succinct _scope and content_ note. 

## Optional Fields
The following notes are optional and should only be added when applicable:

| Field Name | DACS Rule | EAD Tag | MARC Field |
| ---------- | --------- | ------- | ---------- |
| Arrangement | [DACS 3.2](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/02_system_of_arrangement.html) | [\<arrangement>](https://www.loc.gov/ead/tglib/elements/arrangement.html) | [MARC 351](https://www.loc.gov/marc/bibliographic/bd351.html) |
| Language of Material | [DACS 4.5](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/05_languages_and_scripts_of_the_material.html) | [\<langmaterial>](https://www.loc.gov/ead/tglib/elements/langmaterial.html) | [MARC 546](https://www.loc.gov/marc/bibliographic/bd546.html) |
| Conditions Governing Use and Reproduction | [DACS 4.4](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/04_conditions_governing_reproduction_and_use.html) | [\<userestrict>](https://www.loc.gov/ead/tglib/elements/userestrict.html) | [MARC 540](https://www.loc.gov/marc/bibliographic/bd540.html) |
| Other Finding Aids | [DACS 4.6](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/06_finding_aids.html#46-finding-aids-added-value) | [\<otherfindaid>](https://www.loc.gov/ead/tglib/elements/otherfindaid.html) | [MARC 555](https://www.loc.gov/marc/bibliographic/bd555.html)[^4] |
| Custodial History | [DACS 5.1](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/01_custodial_history.html) | [\<custodhist>](https://www.loc.gov/ead/tglib/elements/custodhist.html) | [MARC 561](https://www.loc.gov/marc/bibliographic/bd561.html) |
| Accruals | [DACS 5.4](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/04_accruals.html) | [\<accruals>](https://www.loc.gov/ead/tglib/elements/accruals.html) | [MARC 584](https://www.loc.gov/marc/bibliographic/bd584.html) |
| Existence and Location of copies | [DACS 6.2](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/02_existence_and_location_of_copies.html) | [\<altformavail>](https://www.loc.gov/ead/tglib/elements/altformavail.html) | [MARC 530](https://www.loc.gov/marc/bibliographic/bd530.html); [MARC 535](https://www.loc.gov/marc/bibliographic/bd535.html) |
| Separated Materials | [DACS 6.3](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/03_related_archival_materials.html) | [\<separatedmaterial>](https://www.loc.gov/ead/tglib/elements/separatedmaterial.html) | [MARC 544](https://www.loc.gov/marc/bibliographic/bd544.html) |
| Related Archival Materials | [DACS 6.3](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/03_related_archival_materials.html) | [\<relatedmaterial>](https://www.loc.gov/ead/tglib/elements/relatedmaterial.html) | [MARC 544](https://www.loc.gov/marc/bibliographic/bd544.html) |

### Arrangement
The _arrangement note_ should be used to describe the current organization of the collection, and should not include any statements regarding prior rearrangement by the archivist or creator. Any significant arrangement change that warrants documentation should be described in the _processing note._  

It is best practice to use an _arrangement note_ in the front matter of the finding aid only when you describe a collection that does not have series. This differs slightly from the guidance in [DACS 3.2](https://saa-ts-dacs.github.io/dacs/06_part_I/04_chapter_03/02_system_of_arrangement.html) because the [Archives Portal ](https://archives.nypl.org/)automatically generates a statement when a collection is arranged into series. Therefore it is not necessary to repeat that information in a separate arrangement note. It is recommended to use arrangement notes on the series level.

### Language of Material 
This note is only used when a significant portion of the collection is in a language other than English. First change the language field in the _basic information_ section to state _multiple languages_, and then add a _language of material_ note to describe the languages in the collection. If the bulk of the collection contains English language materials, then there is no need to include this note. [DACS 4.5](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/05_languages_and_scripts_of_the_material.html) has general guidance on how to construct this note.

### Conditions Governing Use and Reproduction
This note is to provide specific details about certain copyright restrictions regarding use, reproduction, and publication of collection materials. Only use this note if the deed of gift or purchase agreement includes specific stipulations, restrictions, or language about use of certain collection materials. [DACS 4.4](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/04_conditions_governing_reproduction_and_use.html) has further guidance on this topic. 

### Other Finding Aids
This field should be used when a collection includes additional documentation such as inventories, indexes, or descriptive guides that are available to researchers. When a link to these documents is embedded in the finding aid on the [archives portal](https://archives.nypl.org/), this field should be used to describe the content and origin of the additional resource documents.[ DACS 4.6](https://saa-ts-dacs.github.io/dacs/06_part_I/05_chapter_04/06_finding_aids.html#46-finding-aids-added-value) provides more detailed guidance on this element, as well as commentary that explains that the term _finding aid_ “covers any type of description or means of reference made or received by an archival repository in the course of establishing administrative or intellectual control over archival materials.

### Custodial History 
This note should only be used if it is necessary to document changes of ownership of collection material which may have occurred between being in possession of the collection creator and NYPL’s acquisition of the materials. This is not to be confused with the details recorded in the _immediate source of acquisition_ field, which details information about the donor or seller. [DACS 5.1](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/01_custodial_history.html) contains information about when it is appropriate to use a _custodial history_ note.

### Accruals
This note is used to describe when additions to the collection are anticipated. This information is typically found in the deed of gift or purchase agreement and should be included in the finding aid when it is known that future accruals will be added to the existing description. [DACS 5.4](https://saa-ts-dacs.github.io/dacs/06_part_I/06_chapter_05/04_accruals.html) offers further clarity about this element.

### Existence and Location of Copies 
Use this field to describe copies or reproductions of the materials being described that are available at NYPL or another institution. This does not include copies made for preservation or access purposes. [DACS 6.2](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/02_existence_and_location_of_copies.html) provides further information and guidance on this note field.

### Separated Materials 
This note should be used to describe materials that have been physically separated from a collection, but which share a provenance with the materials described in the finding aid. This may include formats that were removed for special processing and description in a separate finding aid, commercial media that was removed and retained by the curatorial unit, or other collection material that is accessible, but not described in the finding aid. This does not include discarded or suppressed materials. See [DACS 6.3](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/03_related_archival_materials.html) for additional information about this note.

#### Schomburg Separation Notes
{: .fs-4 }
Schomburg Center collections are routinely separated and described in discrete finding aids or catalog records for [Manuscripts, Archives and Rare Books Division](https://www.nypl.org/locations/schomburg/manuscripts-archives-and-rare-books-division) (MARB), [Photographs and Prints Division](https://www.nypl.org/locations/schomburg/photographs-and-prints-division) (SCP), the [Moving Image and Recorded Sound Division](https://www.nypl.org/locations/schomburg/moving-image-and-recorded-sound-division), the [Art and Artifacts Division](https://www.nypl.org/locations/schomburg/art-and-artifacts-division), and the [Jean Blackwell Hutson Research and Reference Division](https://www.nypl.org/locations/schomburg/jbh-research-and-reference-division). 

Use the following _Separated Materials_ notes when working with Schomburg collections:

See the \[division] for the \[collection title], \[collection call number]. 

- _Example: See the Manuscripts, Archives, and Rare Books Division for the Alexis De Veaux papers, Sc MG 802._ 

If the separated collection does not have a title/call number assigned: 

See the \[division] for \[general term for relevant material, e.g. _artworks_, _photographs,_ etc.]

- _Example: See the Photographs and Prints Division for the photographs._

### Related Archival Materials
Use this note to indicate the names and locations of collections that share a provenance, or have a close association with the collection being described in the finding aid. For further information see [DACS 6.3](https://saa-ts-dacs.github.io/dacs/06_part_I/07_chapter_06/03_related_archival_materials.html).

[^1]: Jarret Drake criticizes this pratice writing that “In this note, archivists often write massive memorials and monuments to wealthy, white, cisgendered and heterosexual men, including selective details about the creator that have minimal bearing on the records, and instead serve to valorize and venerate white western masculinity. Jarrett M. Drake, “RadTech Meets RadArch: Towards A New Principle for Archives and Archival Description,” _On Archivy_, April 7, 2016, <https://medium.com/on-archivy radtech-meets-radarch-towards-a-new-principle-for-archives-and-archival-description-568f133e4325>.

[^2]: Archives for Black lives suggests “Do not let your discomfort with the terms censor the material. It is okay to be uncomfortable with racist material. It is not okay to privilege your discomfort above accurate description.” Alexis A. Antracoli et al., “Archives for Black Lives in Philadelphia: Anti-Racist Description Resources,” October 2019,[https://github.com/a4blip/A4BLiP/tree/master/Resources](https://github.com/a4blip/A4BLiP/tree/master/Resources).

[^3]: Tonia Sutherland emphasizes that “Just as archivists create ‘the archive,’ so, too, do they influence what narratives and stories can and cannot emerge from the archives.” Tonia Sutherland, “Archival Amnesty: In Search of Black American Transitional and Restorative Justice,” _Journal of Critical Library and Information Studies_ 1, no. 2 (June 5, 2017): 11, [doi:10.24242/jclis.v1i2.42](https://journals.litwinbooks.com/index.php/jclis/article/view/42).

[^4]: In a MARC21 record, a note in the 555 field would mention the existence of the EAD-encoded finding aid, but no specific EAD element maps to this field, <https://www.loc.gov/ead/tglib/appendix_a.html#foot5>.









