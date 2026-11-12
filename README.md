TraceKin
A Deceased Persons Identification and Family Location System in Kigali City, Rwanda

1. Project Overview

TraceKin is a database-driven application designed to help families locate deceased relatives who died in accidental circumstances within Kigali City, Rwanda, outside private homes.

The system connects participating institutions responsible for registering and holding deceased persons with family members searching for their loved ones.

It provides a centralized platform for registering identified deceased persons, submitting family search requests, verifying family relationships and sharing authorized location information.

2. Problem Statement

When a person dies unexpectedly in an accident, family members may experience difficulties locating their loved one. They may need to contact or visit different institutions to establish where the deceased person is being held.

The lack of a centralized information-sharing platform can make this process difficult and time-consuming.

TraceKin aims to address this problem by providing a centralized database application that supports deceased-person registration, family verification and location tracking.

 3. Project Objectives

 Main Objective

To develop a centralized database system that facilitates the registration, identification and location tracking of deceased persons and provides secure access to verified family members.

 Specific Objectives

1. Develop a centralized database for registering identified deceased persons and their current locations.
2. Implement search and verification mechanisms for family members.
3. Automate notification tasks for verified next of kin when eligible records remain unclaimed beyond a specified period.
4. Maintain an audit trail of registrations, verification decisions, location updates and notifications.

 4. Project Scope

The initial system will cover:

- Accidental deaths occurring within Kigali City.
- Incidents occurring outside private homes.
- Officially identified deceased persons.
- Participating institutions responsible for holding deceased persons.
- Family search requests and relationship verification.
- Authorized disclosure of current holding locations.

The system will not disclose causes of death or replace official police, forensic or civil-registration processes.

 5. Main System Users

- Institution Administrator: Registers deceased persons and updates their information and locations.
- Verification Officer:Reviews family requests and makes authorization decisions.
- Family Member: Searches for a loved one and submits verification information.
- System Administrator:Manages system users and monitors system activities.

 6. Planned Database Tables

The initial database design is expected to include:

- INSTITUTION
- DECEASED_PERSON
- FAMILY_MEMBER
- RELATIONSHIP
- SEARCH_REQUEST
- NOTIFICATION
- BODY_TRANSFER
- SYSTEM_USER
- AUDIT_LOG

N.B:The final table structure will be determined during database analysis and normalization.

 7. Planned PL/SQL Features

The project will demonstrate:

- Procedures for registering deceased persons and processing search requests.
- Functions for checking records and verification eligibility.
- Explicit and implicit cursors.
- PL/SQL records and collections.
- Packages for organizing business operations.
- Triggers for maintaining audit records.
- Exception handling.
- Scheduled jobs for processing unclaimed-record notification tasks.

 8. Data Source

The project will investigate publicly available and appropriately licensed anonymized datasets related to accidental deaths and injury statistics in Rwanda.

The final dataset source, size, license and limitations will be documented after research.

Fictional demonstration records may be used for testing application functionality and will be clearly distinguished from real data.

 9. Innovation

TraceKin will include two separate interfaces:

1. An administrative interface for institutions to register deceased persons, manage records, review verification requests and update locations.
2. A family interface for searching for loved ones, submitting verification requests and accessing authorized location information.

The system will use a controlled verification workflow and maintain an audit trail of important activities.

 10. Security and Privacy

The system will implement role-based access, verification before disclosure of information, restricted access to sensitive records and activity logging.

The initial prototype will simulate identity and relationship verification. Direct integration with Rwanda's National Identification Agency (NIDA) is considered a possible future enhancement subject to official authorization.

 11. Technology

- Oracle Database 21c XE
- SQL and PL/SQL
- Git and GitHub for version control

 12. Project Status

Currently in Phase 0: Research, Data Source and Project Proposal.

 13. References
to be updated

Research papers, official reports, dataset sources and technical documentation will be added as the research phase progresses.

