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
