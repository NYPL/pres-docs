---
title: Controlled Access Terms
layout: default
parent: Archival Description
grandparent: Archival Processing
nav_order: 2
has_children: false
---
# **Controlled Access Terms**
In ArchivesSpace, controlled access terms are divided into [_Agents_]() (personal names, corporate bodies, family names) and [_Subjects_]() (topics, genre/form, occupations), which are used as access points in the [archives portal](http://archives.nypl.org/), the [NYPL catalog](https://browse.nypl.org/iii/encore/homepage), the [NYPL research catalog](https://www.nypl.org/research/research-catalog), and in [WorldCat](https://www.worldcat.org/). Once a finding aid is complete, the MARC XML is exported in order to create a record in WorldCat and in Sierra. It is important that your agents and subjects are formed correctly, otherwise the terms will not properly validate. All finding aids must include controlled access terms. The [ArchivesSpace Documentation](/aspace.md) contains detailed information about how to add agents and subjects to your finding aid, as well as how to create and add new terms. The section of this documentation on [Inclusive Description]() provides further explanation on how to choose access terms that are not offensive or harmful. 

## **Agents**
Agents are the individuals, corporate entities, or families that created the collection, contributed to its content, or are the subject matter of the records. Each agent must be designated as either a _main entry_, _creator/contributor_, or _subject._ There are already many agents included in ASpace from other processed collections, so be sure to check if the agent you wish to add already has a record in ASpace before creating a new one. If you need to create a new agent record, see the [Creating New Agents]() section of this documentation.

## **Main Entry** 
Most collections must include a _main entry_ \[[DACS 2.6](https://saa-ts-dacs.github.io/dacs/06_part_I/03_chapter_02/06_name_of_creators.html)]. The _main entry_ is the person \[[MARC 100](https://www.loc.gov/marc/bibliographic/bd100.html)], corporate entity \[[MARC 110](https://www.loc.gov/marc/bibliographic/bd110.html)], or family \[[MARC 100](https://www.loc.gov/marc/bibliographic/bd100.html)] responsible for the creation of the records. A collection can only have one _main entry._ If a collection was created by multiple people, the other individuals or corporate entities should be added as a _creator/contributor_ \[[MARC 700](https://www.loc.gov/marc/bibliographic/bd700.html)/[MARC 710](https://www.loc.gov/marc/bibliographic/bd710.html)].

![main entry](/Images/59-main-entry.png)

When the collection’s EAD is exported, ASpace will automatically fill in the relator field of the _main entry_ with the $ecreator \[cre] relator term, which is the most common relator for a _main entry_. If the _main entry_ of your collection is not also the creator of the materials, choose the appropriate term from the [LSCH MARC Code List for Relators](https://www.loc.gov/marc/relators/relaterm.html). 

If the collection is an artificial collection created by the Library (e.g. [Schomburg Daguerreotypes collection](https://archives.nypl.org/scp/186032)), do _not_ include a _main entry_ \[[MARC 100](https://www.loc.gov/marc/bibliographic/bd100.html)/[MARC 110](https://www.loc.gov/marc/bibliographic/bd110.html)]. Instead record the Library division as a _creator/contributor_ \[[MARC 710](https://www.loc.gov/marc/bibliographic/bd710.html)] with the appropriate relator term.

Note that the first inidcator in the [MARC 245](https://www.oclc.org/bibformats/en/2xx/245.html) field (Title Statement) must be changed from 1 to 0 when there is no main entry. 

## **Creator/Contributor**
Any individual \[[MARC 700](https://www.loc.gov/marc/bibliographic/bd700.html)] or corporate entity \[[MARC 710](https://www.loc.gov/marc/bibliographic/bd710.html)] that created material in the collection or contributed in a significant way to the collection’s content should be added as a _creator/contributor_. This can include an agent that is a co-author, frequent correspondent, or artistic collaborator. It is not necessary to list every individual that appears in the collection, just those that made meaningful contributions to the content.

![creator/contributor](/Images/60-creator-contributor.png)

When adding a _creator/contributor_, you should also add a relator term from the dropdown menu to describe the agent’s role. The most common term is _contributor_, but there are many other possibilities which are defined in the [LSCH MARC Code List for Relators](https://www.loc.gov/marc/relators/relaterm.html).

## **Agents as Subjects**
An agent that is not the _main entry_ or _creator/contributor_ can be added as a _subject._ This is appropriate for individuals \[[MARC 600](https://www.loc.gov/marc/bibliographic/bd600.html)] or corporate entities \[[MARC 610](https://www.loc.gov/marc/bibliographic/bd610.html)] that are represented, discussed, or are a prominent subject matter in the collection. 

![agent as subject](/Images/61-agent-subject.png)

When adding an agent as a subject, you also have the option to add a subdivision (e.g. Pratt Institute -- Students). As with all agents, make sure you are using authorized terms, and if you add a subdivision, be sure to select the correct type of subdivision from the dropdown list. 

![subdivision](/Images/62-subdivision.png)

Family names should always be sourced from the Library of Congress. Do not use a family name sourced from Library of Congress Name Authority Files (LCNAF) as a subject; instead, use the form of the family name from Library of Congress Subject Headings (LCSH) in accordance with the rules in the [Subject Heading Manual](https://www.loc.gov/aba/publications/FreeSHM/H1631.pdf). Family names in LCNAF that are ineligible for use as subjects will be noted as such in its MARC authority record as illustrated below.

![LC note](/Images/63-LC-note.png)

Family names are created in ArchivesSpace as Family Agents, regardless of source; take care when applying these headings, as the list contains both LCNAF and LCSH headings. If you wish to add a meeting or conference name \[[MARC 611](https://www.loc.gov/marc/bibliographic/bd611.html)] as a subject, enter the authorized term as an Agent Subject. The term will be exported as a MARC 610 field, and will need to be manually changed to MARC 611 when creating the catalog record. See the section of this documentation on [Creating Catalog Records]() for further information. 

## **Creating New Agents**

If you would like to add a person, family, or corporate entity as an agent, but they do not have an agent record in ASpace, then you will need to create a new agent entry. The ArchivesSpace documentation contains detailed instructions on how to create a [new agent entry](). For a person or corporate entity, use an authorized name from the[ Library of Congress Name Authority Headings](https://authorities.loc.gov/). If the agent does not have a Library of Congress authority record, first check the Getty’s Union List of Artist Names ([ULAN](https://www.getty.edu/research/tools/vocabularies/ulan/)), then Social Networks and Archival Context ([SNAC](https://snaccooperative.org/)), and finally the Virtual International Authority File ([VIAF](http://viaf.org/)). If there is no authority record from any of these sources, then create a new agent record and select _local (unauthorized)_ from the dropdown menu in ASpace.

When you create a new authorized agent record, you must also include the term’s authority ID in the authority ID field \[[DACS 13.2](https://saa-ts-dacs.github.io/dacs/08_part_II/06_chapter_13/02_authority_record_identifier.html#132-authority-record-identifier-required)]. The authority ID is included in the agent’s authority record, and is often the digits and sometimes letters at the end of a URI. Examples of an authority record and where to find the unique identifier are illustrated below. Note that the space between the letter and numbers in the LC control number is important to include. 

**Library of Congress Authorities**

![LC identifer](/Images/64-LC_identifer.png)

**ULAN**

![ULAN](/Images/65-ULAN.png)

**SNAC**

![SNAC](/Images/66-SNAC.png)

**VIAF**

![VIAF](/Images/67-VIAF.png)

Before adding an authority identifier to an Agent record, verify that the authority record is for the person described by the Agent record (e.g. same time periods and fields of activity). If a name is being authorized against SNAC, verify that the SNAC record has finding aids (Resources) from repositories other than NYPL; otherwise, there is a risk of circular authorization.

Select the _authority source_ from the dropdown menu (NACO is the most common source for names and corporate bodies).

When entering a name in a new agent record into ASpace, do so in the way in which it is constructed in the authority record. If a person’s name is listed in indirect order as _last name, first name_, then make sure to put each part of the name in its own field as illustrated below. Do not include additional information, such as dates, suffixes, or titles unless that information has been included in the authority record. 

![ASpace Agent](/Images/68-ASpace-agent.png)

The Library of Congress usually only includes these additional fields for disambiguation purposes. Dates included in an authority record should be entered into the _dates_ field as illustrated below.

![ASpace Agent with Dates](/Images/69-ASpace-Agent-Dates.png)

Other disambiguation terms should be entered into the _qualifier_ field, as illustrated below.

![ASpace Agent with Qualifier](/Images/70-ASpace-Agent-Qualifier.png)

If the Library of Congress authority record indicates an agent uses RDA rules (as illustrated below), add _Resource Description and Access_ in the _Rules_ field in ASpace. This will be indicated in the _descriptive conventions_ field of the Library of Congress Name Authority Record as well as in the authority’s MARC record in subfield e of the 040 field. 

![LC Record RDA](/Images/71-Belafonte-RDA.png)

![MARC Record RDA](/Images/72-Belafonte-RDA-MARC.png)

![Agent Record RDA ASpace](/Images/73-Belafonte-Agent-ASpace.png)

If the agent is from a source other than the Library of Congress, or if the Library of Congress authority record does not indicate a name was derived using RDA rules, then leave the _Rules_ field blank as illustrated below. 

![LC Record not RDA](/Images/74-non-RDA.png)

![Non RDA ASpace](/Images/75-not-RDA-ASpace.png)

### **Family Agent Records**
When creating new _family_ agents, never create a local agent entry. Family names should always be sourced from either the LCNAF or LCSH, depending on its application. Family names that are applied as _Creator/Contributor_ or _Main Entry_ should come from LCNAF and include the appropriate form and identifier; names that are applied as _subjects_ should come from LCSH.

## **Creating Local Access Terms**

If you are processing a collection in which the _main entry_, a _creator/contributor_, or _subject_ does not have an authority record, you should create a new agent record, and select _Local (unauthorized)_ as the source. Only create a local heading if the agent name can not be located in any of the sources listed previously, or if you have determined that the authorized form of the agent’s name is incorrect. See the section of this documentation on [Inclusive Cataloging Guidelines]() for more information on the rationale for creating local unauthorized agent records. 

Local access points should be created according to [RDA 9.19](http://original.rdatoolkit.org/rdachp9_rda9-5463.html). Locally-created headings should be clearly disambiguated from names in existing authorities. A local name should never match one in an existing authority record. Refer to [RDA 9.19.1.3](http://original.rdatoolkit.org/rdachp9_rda9-5621.html) - [9.19.1.8](https://original.rdatoolkit.org/rdachp9_rda9-9950035.html) for more information regarding disambiguating names. All NYPL staff have access to the [RDA toolkit](https://original.rdatoolkit.org/) via an NYPL login. If you are unable to login to RDA Toolkit, let your supervisor know.

When creating a local agent access point, you should always choose _Local (Unauthorized)_ from the dropdown list in ASpace.

![Local Terms ASpace](/Images/76-Local-terms-ASpace.png)

It is also good practice to add an identifying term to the _qualifier_ field, as well as birth and death dates, if this information can be verified.

![Local Agent in ASpace](/Images/77-local-agent-ASpace.png)

# **Subjects**
In ArchivesSpace, subjects are divided into _topical_ subjects; _geographic_ terms; _genre/form_; _occupations_; and _uniform titles_. There are many subjects already in ASpace from other processed collections, so make sure to search through the ASpace subjects before creating a new term. ASpace will not allow you to make a new term identical to an existing one in the database. 

There is more information below about which controlled vocabularies to use for specific types of subjects, the way in which the term will appear in the portal, and the equivalent MARC field. If you need to create a new subject, see the section of this documentation about [Creating New Subjects]().

| Name in ASpace | Name in Portal | MARC Field | Sources and Notes |
| -------------- | -------------- | ---------- | ----------------- |
| Topical | Subjects | [MARC 650](https://www.loc.gov/marc/bibliographic/bd650.html) | Use Library of Congress Subject Headings \[[LCSH](https://id.loc.gov/authorities/subjects.html)] for topical subjects. When applicable, add subdivisions to subjects to make them more specific. Each LCSH entry will note if a term can be subdivided, and if a term is intended _only_ as a subdivision. You can use _topical_, _geographic_, _temporal,_ or _genre/form_ terms as subject subdivisions. |
| Geographic | Places | [MARC 651](https://www.loc.gov/marc/bibliographic/bd651.html) | Use the Library of congress Name Authority File \[[LCNAF](https://id.loc.gov/authorities/names.html)] and [LCSH](https://id.loc.gov/authorities/subjects.html) to find valid geographic terms. Geographic terms are also often used as subdivisions of topical terms. If you add a geographic subdivision, be sure to [format it correctly](https://www.loc.gov/aba/publications/FreeSHM/freeshm.html0.pdf). The [authority record](https://authorities.loc.gov/) will include the correct structure for subdivisions. Not all geographic terms are valid as subdivisions. |
| Genre/Form | Material Types | [MARC 655](https://www.loc.gov/marc/bibliographic/bd655.html) | This [list](https://docs.google.com/spreadsheets/d/1IWhJ4wShYuAdD8IgwTguXXvDOgSYS5l0CBpKtrfIqx0/edit?usp=sharing) includes the most commonly used and preferred genre/form terms. Always consult this list first. Always try to use [LCGFT](https://id.loc.gov/authorities/genreForms.html) terms first. There is a [PDF](https://www.loc.gov/aba/publications/FreeLCGFT/GENRE.pdf) of all the terms available as well.[AAT](https://www.getty.edu/research/tools/vocabularies/aat/) is an acceptable source if LCGFT does not have an appropriate term. [LCGFT](https://id.loc.gov/authorities/genreForms.html) terms can also be used as subdivisions of topical terms. It is best to avoid creating local _genre/form_ terms. |
| Occupation | Occupations | [MARC 656](https://www.loc.gov/marc/bibliographic/bd656.html) | Use the [ITOAMC](https://folgerpedia.folger.edu Index_terms_for_occupations_in_archival_and_manuscript_collections_\(ITOAMC\)) list of occupations or [LCSH](https://id.loc.gov/authorities/subjects.html). |
| Uniform Title | Titles | [MARC 630](https://www.loc.gov/marc/bibliographic/bd630.html) and [MARC 730](https://www.loc.gov/marc/bibliographic/bd730.html) | Use the [LCNAF](https://id.loc.gov/authorities/names.html) and [LCSH](https://id.loc.gov/authorities/subjects.html) to find valid titles. |
| Temporal | n/a | [MARC 648](https://www.loc.gov/marc/bibliographic/bd648.html) | _Temporal_ terms should only be used as subdivisions of _topical_ and _geographic_ terms. |

## **Creating New Subjects**

If you need to create a new subject, follow the instructions in the [ASpace User Guide](https://sites.google.com/nypl.org/specialcollections/special-collections-processing/archival-processing/archivesspace-guide) for making new access terms. When creating a new subject, only use existing controlled vocabularies from the Library of Congress ([LCSH](https://id.loc.gov/authorities/subjects.html)), Index Terms for Occupations in Archival and Manuscript Collections ([ITOAMC](https://folgerpedia.folger.edu/Index_terms_for_occupations_in_archival_and_manuscript_collections_\(ITOAMC\))), Library of Congress Genre and Form Terms ([LCGFT](https://www.loc.gov/aba/publications/FreeLCGFT/freelcgft.html)), or the Art and Architecture Thesaurus [(AAT](https://www.getty.edu/research/tools/vocabularies/aat/). 

When creating a complex subject with subdivisions, be sure to only include one _term_ per field, and also select the correct _type_ of term in the dropdown menu. The Library of Congress’ [Subject Headings Manual](https://www.loc.gov/aba/publications/FreeSHM/freeshm.html) contains extensive information about how to form complex subjects and how to use various subdivisions. 

When creating new headings from the LCSH, if the heading does not have any subdivisions, provide the LC Authority Control Number as part of the record. If the heading includes subdivisions, the Authority Control Number is not necessary.

### **Complex Subjects**

Adding subdivisions to a subject is a good way to make a very general subject more specific. You can add a _geographic_ location, _temporal_ term, or _genre/form_ term. For example a term such as _Actors--United States--20th century_ looks like this is ASpace:
![complex subjects ASpace](/Images/78-complex-subjects-ASpace.png)

Remember that _geographic_ and _topical_ terms can both be subdivided and used as subdivisions. _Temporal and genre/form_ terms can be used as subdivisions, but they can never be subdivided with topical or geographic terms. A good general rule of thumb is to not exceed two subdivisions for a single subject heading. An overly complex subject heading does not aid in discovery. 

There is extensive information available about how to form complex through the Library of Congress’ [online training modules](https://www.loc.gov/catworkshop/lcsh/). The illustration below shows the different possibilities for creating complex subjects, and the order in which to list the terms.

![LC Module Example](/Images/79-LC-Module.png)

### **Geographic Subdivisions**

When adding a geographic subdivision to a subject, first make sure the term includes a note stating that the term can be geographically subdivided as illustrated below.

![LC Collection Membership](/Images/80-LC-collection-membership.png)

Note that geographic terms are usually formatted differently when they are used as a subdivision to a [topical](https://www.loc.gov/marc/bibliographic/bd650.html) term, than if they are being used as a [geographic name](https://www.loc.gov/marc/bibliographic/bd651.html) subject. A geographic term’s record in the [Library of Congress authorities](https://authorities.loc.gov/) contains information on how to properly format a term. Information on subdividing geographic subjects is available in [H 830](https://www.loc.gov/aba/publications/FreeSHM/H0830.pdf) of the _Subject Heading Manual_.  Specific rules regarding New York City are available in [H 990](https://www.loc.gov/aba/publications/FreeSHM/H0990.pdf).

For example, the geographic term for New York City is [New York (N.Y.)](https://lccn.loc.gov/n79007751), but when you use it as a subdivision, it is formatted like this: **__New York (State)--New York_** . Each [authority record](https://authorities.loc.gov/) will include a _Geographic subdivision usage_ note like the one shown below. 

![Geographic Subdivision LC](/Images/81-LC-geographic-subdivision.png)

Also note that not all geographic headings are valid for use as a subdivision, so check the authority record for a note like this: 

![Geographic invalid LC](/Images/82-LC-Geographic-not-valid.png)

Typically, geographic subdivisions will include a state, followed by the city. In ASpace it should be entered like this:

![ASpace Geographic Subdivision](/Images/83-ASpace-Geographic-subdivision.png)

Remember that _topical_ terms can be subdivided with _geographic_ terms, and _geographic_ terms can be subdivided topically. Regardless of which order works best for your collection, _temporal_ and/or _genre/form_ subdivisions will always be listed last as illustrated in the image at the beginning of this [section]()

### **Genre/Form Subdivisions**

There are some terms that can only be used as subdivisions, and others that may seem as if they should be _genre/form_ subdivisions, but are classified as _topical_. The best way to confirm that you are selecting the correct _type_ of subdivision is to consult the term’s Library of Congress [authority record](https://id.loc.gov/authorities/subjects.html). When adding a _genre/form_ subdivision only use Library of Congress [genre/form terms](https://www.loc.gov/aba/publications/FreeLCGFT/freelcgft.html), never add an AAT or ITOAMC term as a subdivision. Remember that _genre/form_ terms can never be subdivided, but they can be used as subdivisions. _Genre/form_ subdivisions will always be listed last in a complex subject as illustrated in the image at the beginning of this [section](). 

### **Temporal Subdivisions**

Add a temporal subdivision to specify a more precise time period for a subject term. A term such as [_20th Century_](https://id.loc.gov/authorities/subjects/sh2002012476.html) is a temporal subdivision, while an authorized topical term that includes a year, such as [_World War, 1939-1945_](https://id.loc.gov/authorities/subjects/sh85148273.html), is not a temporal term and cannot be used as a temporal subdivision. If you are unsure of the type of term or subdivision you are adding, always consult the [Library of Congress Subject Authorities](https://authorities.loc.gov/) or [Library of Congress Subject Heading Manual](https://www.loc.gov/aba/publications/FreeSHM/freeshm.html). Temporal subdivisions will always be listed after _geographic_ and/or _topical_ terms, and always followed by _genre/form_ subdivisions when one is included. See the illustration at the beginning of this [section]() for information on the correct order for complex subjects.

















 




