# TraceKin
### A Deceased Persons Identification and Family Location Support System

**Course:** INSY 8311 – Database Development with PL/SQL  
**Student:** umwariwase Ineza Ange 
**Student ID:** 28278 
**Institution:** Adventist University of Central Africa (AUCA)



## 1. Project Overview

TraceKin is an academic database application designed to address the challenge of locating families of identified deceased persons.

The system proposes a centralised platform that enables authorised institutions to register and manage deceased-person records, process family enquiries, coordinate verification requests and communicate approved information about the location where a deceased person is being held.

The project explores a problem that can occur in different parts of the world. It is designed as a globally adaptable conceptual solution rather than a system restricted to one geographical location.

## 2. Problem Statement

Information about identified deceased persons may be maintained by different institutions, making it difficult to coordinate records, process family enquiries and communicate relevant information to verified family members.

This fragmentation can create delays and difficulties in the process of locating families.

TraceKin proposes a centralised database system to improve record management, verification workflows and communication between authorised institutions and families.

## 3. Project Objectives

### Main Objective
To design and develop a database application that supports the management of identified deceased-person records and facilitates the process of locating their families.

### Specific Objectives
- To register and maintain records of identified deceased persons.
- To allow families to submit enquiries and verification requests.
- To enable authorised users to review and approve family verification requests.
- To manage and update the holding locations of deceased persons.
- To maintain notifications and audit records of important system activities.

## 4. Project Scope

The initial academic prototype focuses on identified deceased persons associated with accidental deaths occurring in public places.

The system will support two main user interfaces:

**Institution Portal**
- Register deceased-person records.
- Update holding-location information.
- Review family verification requests.
- Manage notifications and audit records.

**Family Portal**
- Search available records.
- Submit family enquiries and verification information.
- View approved information about the holding location after verification.

Official identity confirmation remains the responsibility of authorised authorities. TraceKin will not independently perform forensic identification or disclose causes of death.

## 5. Data Sources

The project research will use publicly accessible and appropriately anonymised secondary datasets where permitted.

The following datasets have been examined:

**CDC 2024 Mortality Multiple Cause-of-Death Public Use File**
- A United States mortality dataset.
- Examined and processed using Python.
- Contains records that can support statistical research, subject to its data-use restrictions.
- Not suitable as an operational family-location dataset.

**Deceased Persons Identified Not Returned, Mexico (2005–2026)**
- An anonymised dataset containing 1,405 records.
- Relevant to research on identified deceased persons who have not yet been returned to their families.
- A potential real-data source for academic analysis, subject to its licence and the lecturer's approval.

Clearly labelled test records may also be used to demonstrate operational features that cannot be tested using publicly available datasets.

## 6. Planned Database Tables

The proposed database may include the following tables:

1. INSTITUTION
2. DECEASED_PERSON
3. FAMILY_MEMBER
4. RELATIONSHIP
5. SEARCH_REQUEST
6. NOTIFICATION
7. BODY_TRANSFER
8. SYSTEM_USER
9. AUDIT_LOG

The final table structures and relationships will be refined during database design and normalisation.

## 7. Planned PL/SQL Features

The project will demonstrate Oracle PL/SQL programming concepts, including:

- Anonymous PL/SQL blocks.
- Procedures and functions.
- Records and collections.
- Implicit and explicit cursors.
- Cursor FOR loops.
- BULK COLLECT and FORALL where appropriate.
- Exception handling.
- Database triggers.
- Packages.
- Transaction management.

These features will support database operations, validation, verification workflows, notifications and record management.

## 8. Innovation

The proposed innovation is an interactive application connected to the Oracle database.

It will provide separate interfaces for authorised institutional users and family members.

The interface will allow users to interact with actual database records and demonstrate the system's main workflows rather than relying only on static mockups.

## 9. Privacy and Security Considerations

TraceKin deals with sensitive information concerning deceased persons and their families.

The academic prototype will therefore consider:
- Role-based access control.
- Restricted access to sensitive records.
- Family verification before information is disclosed.
- Audit logging of important activities.
- Use of anonymised research data and clearly labelled test records.

Any real-world use would require appropriate institutional authorisation and compliance with applicable data-protection laws.

## 10. Expected Outcome

The expected outcome is a functional Oracle database application demonstrating how centralised record management, family enquiries, verification workflows and controlled information sharing can be organised within one system.


**Project Status:** Phase 0 – Research, Data Source and Project Proposal





## Phase I – Business Process Modeling

### Selected Business Process
KinTrace focuses on identifying deceased persons and helping their verified relatives locate them. The process includes recording identification information, verifying relatives' submissions, and providing location information when verification is successful.

### Modeling Tool
The business process was modeled using a **UML Activity Diagram** created with **diagrams.net (draw.io)**.

### Business Process Diagram
- [View Published Business Process Diagram](https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&dark=auto#R%3Cmxfile%3E%3Cdiagram%20name%3D%22Page-1%22%20id%3D%22rf4b_fTu_Ps-_7FtR_-Q%22%3E7V1Zc%2BM2Ev41qkwe7OJN6tHy2NlUTapm7alNsi8pmIRExCTBkJBl769fgAQvUAclAjpsp6YqIniY6q%2BPrxsNaGLexq%2B%2FZCANf8MBjCaGFrxOzK8TwzA0w6L%2FYyNv5YjuTfnIIkMBH2sGHtH%2FIB%2FU%2BOgSBTDvXEgwjghKu4M%2BThLok84YyDK86l42x1H3r6ZgAXsDjz6I%2BqO%2Fo4CE5ahna834vyBahNVf1jV%2BJgbVxXwgD0GAV60h825i3mYYk%2FJT%2FHoLIya9Si7lffcbztYvlsGEDLnh31%2BNH6nh%2FT7PsuWd%2FvLHf5Pn6Ep3%2B4%2FhT87JWyUEAl%2FpuVlOMvwMb3GEMzqe4ISens1RFAlDeQp8lCy%2BwTl7otWMPHBBsSH8ArN5VAgkREEAEzqWYQIIeCr%2BrEaPU4wSUgBoz%2Bg%2F%2Bv1utWt7YtN3uqXHenNM%2F7HLM3KLE%2FqaABVfBoKcrGDO3n2OE8K1S6ein61CROAjfS02sqLKS8dCEkfsPP1YiuAFREsuggxGgKAXODGciD0vQC%2F044IU15ZDT5k4QsHoXFc8E2ZUnC1Jc7R%2BgTiGJHujl4QthTK59qwa5XP4EH%2BIzZWdK%2Fqifk6jC%2FQDV4d9VMP7VI1BqpG%2F5QTGitA1Kk8jH9%2FpJ74D8aXw%2FpVggubIp04AJ7Kw1o0u2NZUFdiG9gn2ILBBECNp%2BLpdeF1XGbxr2EAf3gwvkwAGXOj7SibCCyaZez%2BDgED2LXz%2FIEE5awxB70rqqjrmtFGZEzSN8sEw6NHAviTxMvPhNhSMnsjZcx%2F5IdXaEC9wAqK7ZnTWBaW55hvGKYfib0jIG1dqsCS4CxR8ReQPdju1kPLoz9aZr6%2F8ycXBW3WQUOG1bmKHf7bPNbcVR9V9AZyDZUS%2BgScYzYD%2FvCjevnILJZeeRezsdxAE1BMU9xmaVSsUAdkCkm1CtNZrUE3AOgxftj5YUvXBOqU%2B6C1taHRjlz50tKFRjtPpg3lSfaggVOlY8%2BVTjEjxlf5Zsigmy6kaolO1O07VNJR5VV2mFXmfXnW8V52e1IoGpZLjrIgTN43SlJy9z2EkboAZuWaXm%2BjKyIkxKEMbJ7ZlGmEQFG9C%2FwbNcCA7eMJBqR0%2BzoIvacQeV48iJt9nmJKfjyXi%2Bh75nmpP%2F67vFjG%2F%2BDvMEH1HmG3m0%2FiZjixTUd7s%2BK18ceM%2BDVmupUjO%2BlSICKYqOVsyI4JpX0pEOAY%2Fck%2FKl913g%2Bs%2BfHkMri2W4JmmwLcddwdXKI7avkUbriqWN1JViltvsgy8tS7gxZvmyd%2FZQONkDMHJ2JowTyFcb1pbr6cfyjdYf7dlCJUDT6iPl1LidwnaX8tkRECxBwWUEMdPy3x3MMlDkMJfk5xG501xpAoavXmJOdPJiXkvcTbC68cUrxtSDCHJsNSVbhyJrmcNRh83pFR1rJaSyXAcPVvt0Q9N0JUStp6t9l2MNu0qnWEe1egrgakk6vTB1N8bWozynKFK%2FxrMcpz8lHOqqGF2mvNFLVnGT%2Bz649RndWUTF%2BZUJsFwT2rlRyIYQ4njWDYwClfbfD%2B4vo8SkeWcUh%2FMQY0o41xomuE4Je2vxJqJmBJy34pXSfGeX6jHrCd7lVU5xPBne8qc6BHqb6IM5cegXjlbYPquqUh8libTV510UuhAX2U6QqKqubumhtYmqscIa7YMrrp3kmtZXSo73ZK0yqKdljnErHlTR0sZ1pn20J4PEKFFQg%2F90t7NGTNs6imjG34iRkGwRmd7%2FuIN5gd5hiEtU4JfNVW1yHkyU1DrYhzDWCuWnkiajoC4OLOpOP%2BzjjFLHOLVhH0v558laxmeJYy5xID4YZkO1nUgfv4g66pqb5ubmExhbsayVLGW6l3khN0LnEUWasPvIEXYVCE2r13Nmtb%2FdRRsak%2BvXcM9bhnXlurZnVPqnow%2BoJ1s7wjKZ48lduOckTPIxUut60dF%2FpmHKF1T3S9TVDZbL626r%2Bt97y9W%2FnSvG2od171WRa%2BsfVYgnBu%2FZeFZDb0VygaWow4BR2bmW80EnX%2F1tXaD%2BtmFYNs4pRdslr2pI7oBytOoSL4D6EOQw6CY4khAXDSdJ6yytKkj6SCTG1Kq87qk11PWKOPIrIuXyvJJekdZnLNBhY5kcYZ6i3toyuE%2BjiLos0qXRsLGwiRblXIrsmXOGtqnLcx04pahdtpQfmpn2tshV53HDarMnCmFVFgiFWBxlc3fe55MSzxx46cxOqCdPpx5J%2B0XtYe1x40jkDApu9iB78M8b1dEe1l0N8nWEkxKc6tSa%2BFOCUn2mgprvWdE3QHZjZOu2BclD459tn84N%2FeoMMM%2BlvydI6zb9XE8R1k8aa0yiIq0asK7H5puCDXJk7iaw1O2msOROWPgnDZ52qNccXaszxEMaCp2tihmfRV0aqNMVCyDd0DMLk2e8rS4TNvYj%2F0lBhlb8eNHAMXM%2FO4zGOMXGPwsMbwcYI9TZS3ajkzy51zM%2FPgZN%2Fk5J2V%2FzjHmyQnmTK61XYtGqMVRId5w46TsozJCNTZmO4KNqYt5gygcfRBKczjpT0LRzzAJHglzZl2%2BNmEN%2Bey%2FHrmjZ%2BZzfqYHgCxSZnYl6mhdieqassYDV%2BZiRWd6KW7r7GiEK9AIXURcNY0YtP56q2nl9BXJ%2BRuX64pr7lSZliXRtNzTMvRLNi3b7pqWIRYAFZtWBZ1aJkBtb8L2IL0KqSrVLEBRyLdEb6WspurKbE6quubP34jOmFa7J%2B1Ncgf1gcvsTcoJKl5rmdQ8WgPzcgFItWWS9KXFtrDgo7dcVJ5Aj1ClLhIUJgSyKotwC5RTARairNTmsOmfA3yVZRrKeojcC6oxM0eV890ji9kBetDap7IHosQZOktMIIW10coWh3kyO07WFWmS4IZtxN2gE4A8rHfTaSHOxr8DQhFLihFDM2vMq823jR5mo%2FbiqMOQVu68wQPRFR3Qq4EN0YgerN%2BHY%2Bey%2BbYmVDxsbaRoqcc2Rr6B4gk9S70y39DV9WItwxb9rmKu6F3QHP6%2BDoRXqzgx7ZeMeXiVWSG2dgdaITlwTFUrK71Bgfbyi1emINHeAiV5Ev0g5UBTcErq9lb29ukl2xb2%2BnvESYhgZxVyLAEUXdesw2KOJRiMftyQU9HjT8x3F2nFrWA0kakOxbzXZqEa5H3K%2FB8bZF3c81Q%2FdKsm%2FcgNoFPjE%2BSBIHuCzxWR2gnxhvtUI3zJuyA8U6Fk9BX%2BWsbsiwKfQopIsfgFgUUG4i%2F5CsURSOBh29Csa3arOhBrbtpB%2FUpZoWG6T9n6Y5ui7XZN0RDZ7VB361g7HqTaOPfZH%2FZjYy5CZe3tf88Fc54w8Z%2Fk4%2BWPSf1DeG3otyrN2blvqbqWwRQCBlu50MpHmR8d1oNrDtRJgcRdiUnVFh2tbxFmCfB8nkM1WrRP7%2BBaz%2BFHIM%2BRr8p5NIuErzVd2B7LMQ7aHqv8NgNnG9%2Bh4xK3ljmy46qTmoukks1qlduHu5sfdyN3Atq9TEIo9ihbzKlrgyz%2FTGF5uPvx8Ovdf%2B4UgSAQRd1RNY2ra8YFo9AYQ0algWDxQ65qzcPs%2FdySOmguOQVuAFEDg%2FiDAFN1MFzQRGUPhgBGkKgCQewvpc5EXbQYNKd4pihUP66pBgWxVL8tARgJwqDtss4chPtlGihEQ%2BjPOOTHl9gasvoH5EsaTGUW%2FoapNdPB%2FwM%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E)
- [View Business Process Diagram (PDF)](phase_1/docs/business_process/business_process_diagram.pdf)

### Business Process Explanation
[View Business Process Explanation (PDF)](phase_1/docs/business_process/Business_process_explanation.pdf)



