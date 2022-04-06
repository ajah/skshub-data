# "Something" Nonprofit Sector Data - Entities and Activities

- **Entities:** This CSV contains information about individual organizations in the nonprofit sector. The data includes all organizations that are registered with the CRA as a Public Foundation, Private Foundation or Charitable Organization.
- **Activities:** This CSV contains grant data from the federal Grants & Contributions database. This data allows us to understand more about the activities and programs carried out by organizations in the nonprofit sector

## Overview

Ajah is exploring building common, open source infrastructure for the information already available about the sector, focusing on existing open data sources about nonprofit organizations, grants, and evaluations. Through this work, Ajah is looking to make this information more accessible to the whole sector.

These CSVs will become the building blocks of a data infratsructure prototype for the nonprofit sector. We hope the prototype will show the benefits of open, sharable and organized data, as well as allow different stakeholders to better understand the organizations that make up our sector and the activities and programs they run.

The data we are currently using comes from the federal government, and thus only allows us to have access to the grants given by the government. The prototype is meant to showcase how data infratsructure can help facilitate research for the sector. We hope that the sucess of the prototype will convince private foundations to share their data in order to gain a better picture of the philanthropic landscape in Canada.

## Download

To download, navigate to the "data" folder above and select the CSV. From there, click "Raw" and save the resulting output as a CSV.

## Data Sources

**Canada Revenue Agency - 2019 List of charities**

[3.1 Identification](https://open.canada.ca/data/en/dataset/d4287672-3253-4bb8-84c7-4e515ea3fddf/resource/5d63e096-8c51-4bbf-8157-6e987bddf0b5)

[3.6 General Information](https://open.canada.ca/data/en/dataset/d4287672-3253-4bb8-84c7-4e515ea3fddf/resource/7cd2936e-3641-448d-85cc-78cabcb8f557)

[3.7 Financial Data](https://open.canada.ca/data/en/dataset/d4287672-3253-4bb8-84c7-4e515ea3fddf/resource/21537a95-1abe-4ef8-ada9-793e2ad41521)

[3.13 Compensation](https://open.canada.ca/data/en/dataset/d4287672-3253-4bb8-84c7-4e515ea3fddf/resource/7e114f09-208c-46a3-ac48-98fc7f0cd43c)

[3.2 Charity Contact Web Addresses](https://open.canada.ca/data/en/dataset/d4287672-3253-4bb8-84c7-4e515ea3fddf/resource/0aaae18a-be7b-4866-ad08-9bac5a7e592f)

**Treasury Board of Canada Secretariat - Proactive Disclosure - Grants and Contributions**

[Proactive Disclosure - Grants and Contributions](https://open.canada.ca/data/en/dataset/432527ab-7aac-45b5-81d6-7597107a7013/resource/1d15a62f-5656-49ad-8c88-f40ce689d831)

## Data Dictionary

### Entities

**BN:** Business Number issued by the Canada Revenue Agency (CRA) - [Dataset: 3.1 Identification & Field: BN]

**FPE:** Fiscal period end of the organizaton - Dataset: 3.6 General Information & Field: FPE

**Focus Area:** A category broadly defining the sector in which the organization operates, using the 3 programe area codes concatenated into one - [Dataset: 3.6 General Information & Fields: Program #1 Desc, Program #2 Desc, Program #3 Desc]

**Legal Status:** Active or Inactive (organization has been wound-up, dissolved or terminated) - [Dataset: 3.6 General Information & Field: 1570]

**Name:** Legal name of organization - [Dataset: 3.1 Identification & Field: Legal Name]

**Location municipality:** City based on organization's mailing address - [Dataset: 3.1 Identification & Field: City]

**Location Postal Code:** Postal Code based on organization's mailing address - [Dataset:3.1 Identification & Field: Postal Code]

**Legal Designation Type:** Designation code (Public Foundation, Private Foundation or Charitable Organization) - [Dataset: 3.1 Identification & Field: Designation]

**Location Region:** Province based on organization's mailing address - [Dataset: 3.1 Identification & Field: Province]

**Location Country:** Country based on organization's mailing address - [Dataset: 3.1 Identification & Field: Country]

**Revenue:** Organizations' total revenue in the given fiscal year - [Dataset: 3.7 Financial Data & Field: 4700]

**Employees:** Number of permanent, full-time, compensated positions - [Dataset: 3.13 Compensation & Field: 300]

**Website:** URL of the organization’s website - [Dataset: 3.2 Charity Contact Web Addresses & Field: Contact URL]

**Ent SKS ID:** Unique ID for use by entities in the Sector Knowledge Sharing (SKS) project only - [Dataset: N/A & Field: Automatically assigned value]

**Regulating Authority:** This defines where the record was sourced from, all Canadian data is sourced from the CRA - [Dataset: N/A & Field: Automatically assigned value]

**Revenue Currency:** The currency of the revenue - [Dataset: N/A & Field: Pull from a standard ISO - CAD (124)]

**Revenue Year:** Year that the revenue given was reported - [Dataset: Dataset: 3.6 General Information & Field: Year of the FPE]

**Data Source:** URL of where the data was obtained, it is the same for every organization and changes yearly - [Dataset: N/A & Field: Automatically assigned value]

**Legal Status Date:** Year that the legal status of the organization was recorded (year T3010 form was filed) - [Dataset: 3.6 General Information & Field: Year of the FPE]

### Activities

**Act SKS ID:** Unique ID for use by activities in the Sector Knowledge Sharing (SKS) project only - [Field: Automatically assigned value]

**Source ID:** ID assigned to the record by the source authority, for the Grants and Contribution data this is the reference number that is populated by each department - [Field: Ref Number]

**Source Authority:** This defines where the record was sourced from, all Canadian data is sourced from the Proactive Disclosure Grants and Contributions - [Field: Automatically assigned value]

**Source URL:** URL of where the data was obtained, it is the same for every organization and changes XXX - [Field: Automatically assigned value]

**Grant Title:** The title of the project or agreement that the recipient is undertaking (In cases where there is no title, the agreement number will be duplicated here) - [Field: Agreement Title]

**Funding Amount:** The dollar amount given to the organization as stated in the grant or contribution agreement - [Field: Agreement Value]

**Funding Type:** Indicates what the funding amount corresponds to. For Canadian data this is "Amount Applied For". - [Field: Automatically assigned value of "Amount Applied For"]

**Funder:** The distinct organization issuing the grant - [Field: Owner Org]

**Recipient Organization:** The legal name of the recipient organization - [Field: Recipient Legal Name]

**Recipient ID:** A unique and legal identifier for the recipient Organization, for the for the Grants and Contribution data this is the Business Number issued by the Canada Revenue Agency (CRA) - [Field: Recipient Business Number]

**Grant Description:** The description explains why the recipient received funding, what the recipient is undertaking and describes the activities or objectives the recipient organization hopes to achieve with the funds - [Field: Description (English)]

**Funder ID** The legal ID corresponding to the name of the Funder (currently blank)

**Grant Region:** Province based on recipient organization's mailing address - [Field: Recipient Province]

**Grant Municipality:** City based on recipient organization's mailing address - [Field: Recipient City]

**Date:** The assumed start of the agreement, or when the project is supposed to begin, as captured in the initial agreement - [Field: Agreement Start Date]

**Date Type:** Indicates the Date field reflects the "Agreement Start" date - [Field: Automatically assigned value of "Agreement Start"]

**End Date:** The assumed end of the agreement, or when the project is supposed to end, as captured in the initial agreement - [Field: Agreement End Date]

**End Date Type:** Indicates the Date field reflects the "Agreement End" date - [Field: Automatically assigned value of "Agreement End"]

**Expected Results:** The assumed final results the recipient organization aims to achieve with the given funds - [Field: Expected Results (English)]

**Actual Results:** The actual results obtained as a result of receiving the grant funds - [Field: NO idea where this info is coming?]

**Program Name:** The name of the program under which the funds are issued - Field [Program Name (English)]
