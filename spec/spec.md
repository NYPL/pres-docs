---
title: SPEC
layout: default
nav_order: 8
has_children: true
---

{: .alert }
> SPEC documentation has migrated to a new site: [spec-docs](https://nypl-research.github.io/spec-docs/). Please update any bookmarks or links.

# SPEC
SPEC is a FileMaker based internal database application. It functions primarily as a collection management tool supporting efforts to preserve, maintain, and enhance access to NYPL’s special collections. 

SPEC allows Research Library staff to record information on the object level. Unlike other systems such as the Library Catalog and the Archives Portal, which focus on description for search and discovery, SPEC is tailored to record and surface detailed information about each object. These records complement data from other systems and provide a more granular level of tracking supporting various internal workflows.

In addition to objects, SPEC stores information about acquisitions, collections, processing and preservation projects, outgoing loans, and storage locations. These records are interrelated and linked through the objects they describe, offering a comprehensive view of each object’s lifecycle and associations.


## Accounts and Privileges 
To request a [new account 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=583fa04c1b9c305090088550cd4bcb3e){:target="_blank"} or a [password reset 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=7a94d5bb1b88fc1090088550cd4bcb66){:target="_blank"} file a ServiceNow ticket.

Staff privileges to view, edit, or create records in SPEC vary based on the requirements of their job and their division or department. Generally, division staff have access to records that are assigned to their division.


## Connecting
SPEC can be accessed via the FileMaker client or browser. Most SPEC functionality is available via both client and browser. Connection options may depend on a user's SPEC account type. Working remotely or using wifi requires a working and properly configured connection to NYPL's VPN. Requests for [installation of FileMaker software 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=194f82c0e91ac1006a42bcaec0898ac1){:target="_blank"} and for [VPN access 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=3ae790c0878db9006a42c74d19434d00){:target="_blank"} can be made through ServiceNow. See also instructions on connecting to [OpenVPN 🔒](https://docs.google.com/document/d/1BQ-k__gyTYMnTP0RmDxcfY4-Tm6dkdMw5mQEivNUt-4/edit?usp=sharing){:target="_blank"}.

Follow these steps when connecting to SPEC using the FileMaker client for the first time, either on a new workstation or after a software update:  
- Open FileMaker and select File > Hosts from the menu
- Click on FileMaker PRODUCTION. *If FileMaker PRODUCTION is not listed, file a ServiceNow ticket (see link below) to request the IP address of the server. Once you have the IP address, click on the + button in the left panel of the Hosts pop-up window (next to the Hosts Search bar), enter the IP address in the Host Internet Address field and "FileMaker PRODUCTION" in the Favorite Host's Name field*
- If an SSL certificate warning message appears, check “Always permit connection to this host” and then click on the Connect button
- Log in to the server using the SPEC credentials provided via email
- Right click on CollectionInfo and select "Add to Favorites." From now on CollectionInfo will appear under File > Favorites and in the Favorites window when opening FileMaker 
- Click on CollectionInfo and log in with the SPEC credentials provided via email

If connecting to SPEC using the browser, use the url provided in your account set-up email.


## Reporting Bugs and Other Requests
File a [ServiceNow ticket 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=5e3263d3e982c1006a42bcaec0898a27){:target="_blank"} to report a bug, connection issue, or request a custom data report.
