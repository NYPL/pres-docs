---
title: SPEC
layout: default
nav_order: 8
has_children: true
---

# SPEC
SPEC is a FileMaker based internal database application. It functions primarily as a collection management tool supporting efforts to preserve, maintain, and enhance access to NYPL’s special collections. 

SPEC allows Research Library staff to record information on the object level. Unlike other systems such as the Library Catalog and the Archives Portal, which focus on description for search and discovery, SPEC is tailored to record and surface detailed information about each object. These records complement data from other systems and provide a more granular level of tracking supporting various internal workflows.

In addition to objects, SPEC stores information about acquisitions, collections, processing and preservation projects, outgoing loans, and storage locations. These records are interrelated and linked through the objects they describe, offering a comprehensive view of each object’s lifecycle and associations.


## Accounts and Privileges 
To request a [new account 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=583fa04c1b9c305090088550cd4bcb3e){:target="_blank"} or a [password reset 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=7a94d5bb1b88fc1090088550cd4bcb66){:target="_blank"} file a ServiceNow ticket.

Staff privileges to view, edit, or create records in SPEC vary based on the requirements of their job and their division or department. Generally, division staff have access to records that are assigned to their division.


## Connecting
SPEC can be accessed via the FileMaker client or browser. Most SPEC functionality is available via both client and browser. Connection options may depend on a user's SPEC account type. Working remotely or using wifi requires a working and properly configured connection to NYPL's VPN. Requests for [installation of FileMaker software 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=194f82c0e91ac1006a42bcaec0898ac1){:target="_blank"} and for [VPN access 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=3ae790c0878db9006a42c74d19434d00){:target="_blank"} can be made through ServiceNow. See also instructions on connecting to [OpenVPN 🔒](https://docs.google.com/document/d/1BQ-k__gyTYMnTP0RmDxcfY4-Tm6dkdMw5mQEivNUt-4/edit?usp=sharing){:target="_blank"}.

If connecting to SPEC using the FileMaker client for the first time, follow these steps:  
- Open FileMaker and select File > Hosts from the menu
- Click on FileMaker PRODUCTION. If the production server in not listed, file a ServiceNow ticket for instructions on connecting to the server manually 
- If an SSL certificate warning message appears, check “Always permit connection to this host” and then click on the Connect button
- Log in to the server using the SPEC credentials provided via email
- Right click on CollectionInfo and select "Add to Favorites." From now on CollectionInfo will appear under File > Favorites and in the Favorites window when opening FileMaker 
- Click on CollectionInfo and log in with the SPEC credentials provided via email

If connecting to SPEC using the browser, use the url provided in your account set-up email.


## SPEC Landing Page
The SPEC landing page opens when first logging into the database. From the landing page navigate to the different SPEC modules and access select SPEC functionality. The links visible on the landing page vary based on user account privileges. 

To navigate back to the **SPEC landing page** from other SPEC interfaces click on the **SPEC logo** found in the upper left corner. If using the browser, do not use the browser's back button; all navigation must be done within the SPEC interfaces. 


## SPEC Modules
There are several different record types, or modules, in SPEC. SPEC objects refer to collection materials and are associated with acquisitions, collections, and/or projects. 

Additionally, a controlled location hierarchy for NYPL storage locations is maintained in the locations module (CLMGT only), and the outgoing loans module (Registrar only) records outgoing loan information. 


## Reporting Bugs and Other Requests
File a [ServiceNow ticket 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=5e3263d3e982c1006a42bcaec0898a27){:target="_blank"} to report a bug, connection issue, or request a custom data report.
