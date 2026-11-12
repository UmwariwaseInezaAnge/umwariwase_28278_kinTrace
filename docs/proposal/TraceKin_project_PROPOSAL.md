# PROJECT PROPOSAL

## TraceKin: A Deceased Persons Identification and Family Location Support System

**Student:** umwariwase Ineza Ange 
**Student ID:** 28278
**Course:** INSY 8311 – Database Development with PL/SQL  
**Institution:** Adventist University of Central Africa (AUCA)

### 1. Problem Statement

Locating the families of identified deceased persons can be challenging in different parts of the world. Information may be maintained by different institutions, making it difficult to coordinate records, handle family enquiries and communicate relevant information to verified family members.

This fragmentation can delay communication and make it difficult for families to establish where their deceased relatives are being held.

### 2. Proposed Solution

TraceKin proposes a centralised database application designed to support the management of identified deceased-person records and facilitate family-location processes.

The system will provide two main interfaces:

- **Institution Portal:** Allows authorised users to register deceased-person records, update holding locations, review family verification requests and manage notifications.
- **Family Portal:** Allows family members to search available records, submit enquiries and provide verification information. Approved family members can access authorised holding-location information.

Official identity confirmation will remain the responsibility of authorised authorities. TraceKin will not independently perform forensic identification or disclose causes of death.

The initial academic prototype will focus on identified deceased persons associated with accidental deaths occurring in public places.

### 3. Data Source

The project will use publicly accessible and appropriately anonymised secondary datasets.

The main dataset candidate is *Deceased Persons Identified Not Returned, Mexico (2005–2026)*, containing 1,405 anonymised records. It is relevant to the problem of locating families of identified deceased persons and is distributed under a Creative Commons Attribution 4.0 licence.

The CDC 2024 Mortality Multiple Cause-of-Death Public Use File has also been examined using Python. A sample of 500 accidental-death records was extracted for statistical research, subject to CDC data-use restrictions.

Where available datasets do not contain the information required to demonstrate operational workflows, clearly labelled test records will be used. These will not be presented as real cases.

### 4. Planned Database Tables

The proposed database will contain the following tables:

1. INSTITUTION
2. DECEASED_PERSON
3. FAMILY_MEMBER
4. RELATIONSHIP
5. SEARCH_REQUEST
6. NOTIFICATION
7. BODY_TRANSFER
8. SYSTEM_USER
9. AUDIT_LOG

The tables will be refined through database design and normalisation to establish appropriate relationships and maintain data integrity.

### 5. Planned PL/SQL Features

The project will demonstrate the following Oracle PL/SQL features:

- Anonymous blocks, procedures and functions.
- Records and collections.
- Implicit and explicit cursors.
- Cursor FOR loops.
- BULK COLLECT and FORALL where appropriate.
- Exception handling.
- Database triggers and packages.
- Transaction management.

These features will support record registration, validation, family verification, holding-location updates, notification management and audit logging.

### 6. Innovation

The proposed innovation is an interactive Java Swing application connected to the Oracle database using JDBC.

The application will provide separate interfaces for institutional users and family members. Users will be able to interact with database records and demonstrate the registration, search, verification and approval workflows.

PL/SQL will handle the main database business rules, while Java will provide the user interface.

### 7. Privacy and Security Considerations

Because the system concerns sensitive information about deceased persons and their families, the prototype will consider role-based access control, restricted information access, verification before disclosure and audit logging.

The project will use anonymised research data and clearly labelled test records. Any real-world deployment would require appropriate institutional authorisation and compliance with applicable data-protection laws.

### 8. References

Kim, W. C., et al. (2016). Vital statistics: Estimating injury mortality in Kigali, Rwanda. *World Journal of Surgery, 40*(1), 6–13. https://doi.org/10.1007/s00268-015-3258-3

Martínez Castillo, G., & López de León, D. (2026). *Deceased Persons Identified Not Returned, Mexico, 2005–2026 [Anonymised dataset]*. Digital.CSIC. https://doi.org/10.20350/DIGITALCSIC/29048

National Institute of Statistics of Rwanda. (2025). *Rwanda Statistical Yearbook 2025*. https://www.statistics.gov.rw/

National Institute of Justice. (n.d.). *NamUs: Frequently asked questions*. U.S. Department of Justice. https://namus.nij.ojp.gov/frequently-asked-questions

Oracle. (2024). *Oracle Database PL/SQL Language Reference, 21c*. https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html

Republic of Rwanda. (2021). *Law No. 058/2021 relating to the protection of personal data and privacy*.