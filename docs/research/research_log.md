# TraceKin — Research Log

**Project:** TraceKin: A Deceased Persons Identification and Family Location Support System  
**Status:** Phase 0 — Research and Data Source

| No. | APA Reference | Type | Link | Key Finding | Research Gap / Relevance |
|---|---|---|---|---|---|
| 1 | Kim, W. C., Byiringiro, J. C., Ntakiyiruta, G., Kyamanywa, P., Irakiza, J. J., Mvukiyehe, J. P., Mutabazi, Z., Vizir, J. P., Ingabire, J. de la Croix A., Nshuti, S., Riviello, R., Rogers, S. O., & Jayaraman, S. P. (2016). Vital statistics: Estimating injury mortality in Kigali, Rwanda. *World Journal of Surgery, 40*(1), 6–13. https://doi.org/10.1007/s00268-015-3258-3 | Research paper | https://pubmed.ncbi.nlm.nih.gov/26464156/ | Analysed death records from major emergency-care institutions in Kigali during 2012 to study injury-related mortality. | Provides evidence about injury-related deaths but does not describe a system for managing family enquiries and locating relatives. |
| 2 | Laurent, F.-X., Fischer, A., Oldt, R. F., Kanthaswamy, S., Buckleton, J. S., & Hitchin, S. (2022). Streamlining the decision-making process for international DNA kinship matching using worldwide allele frequencies and tailored cutoff log10LR thresholds. *Forensic Science International: Genetics, 57*, 102634. https://doi.org/10.1016/j.fsigen.2021.102634 | Research paper | https://pubmed.ncbi.nlm.nih.gov/34871915/ | Examines international DNA kinship matching to support identification of missing persons and human remains. | Focuses on forensic DNA identification, while TraceKin focuses on records, family enquiries and verification workflows after identification. |
| 3 | National Institute of Statistics of Rwanda. (2025). *Rwanda Statistical Yearbook 2025*. https://www.statistics.gov.rw/sites/default/files/documents/2026-01/RWANDA_STATISTICAL_YEARBOOK_2025_0.pdf | Statistical report | Same link | Reports 769 road-traffic-injury deaths in Rwanda in 2024. | Provides statistical background but does not contain individual case or family-location records. |
| 4 | Martínez Castillo, G., & López de León, D. (2026). *Deceased Persons Identified Not Returned, Mexico, 2005–2026 [Anonymised dataset]*. Digital.CSIC. https://doi.org/10.20350/DIGITALCSIC/29048 | Dataset | https://datos.cchs.csic.es/en/dataset/deceased-persons-identified-not-returned-mexico-20052026-anonymised-dataset | Contains 1,405 anonymised records extracted from institutional family-tracing bulletins. Includes demographic and geographical variables. Licensed under CC BY 4.0. | Highly relevant to the project, but does not contain family contact information or holding locations. Its records also do not establish whether families eventually received the deceased persons. |
| 5 | National Institute of Justice. (n.d.). *NamUs: Frequently asked questions*. U.S. Department of Justice. https://namus.nij.ojp.gov/frequently-asked-questions | Existing system | Same link | NamUs provides a centralised database for missing, unidentified and unclaimed person cases, with restricted access to sensitive information. | Demonstrates centralised case management and controlled access. It operates within the United States. |
| 6 | International Criminal Police Organization. (n.d.). *I-Familia: Identifying missing persons globally through family DNA matching*. INTERPOL. https://www.interpol.int/How-we-work/Forensics/I-Familia | Existing system | Same link | I-Familia supports international identification through family DNA matching and applies data-protection safeguards. | Focuses on forensic DNA matching rather than the institutional record management and family enquiry workflow proposed by TraceKin. |
| 7 | Oracle. (2024). *Oracle Database PL/SQL Language Reference, 21c*. https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/index.html | Technical source | Same link | Documents PL/SQL programming, including collections, records, subprograms, triggers, packages and error handling. | Provides the technical foundation for implementing TraceKin's database operations and business rules. |
| 8 | Republic of Rwanda. (2021). *Law No. 058/2021 of 13 October 2021 relating to the protection of personal data and privacy*. Official Gazette of the Republic of Rwanda. https://www.risa.gov.rw/fileadmin/user_upload/RISA/Publications/2.Laws/Law_relating_to_the_protection_of_personal_data_and_privacy.pdf | Legal / privacy source | Same link | Establishes requirements concerning personal data processing, privacy and safeguards. | Provides an important privacy reference when discussing sensitive information in the project. |

## Additional dataset assessment

**CDC 2024 Mortality Multiple Cause-of-Death Public Use File**

This dataset was downloaded and examined using Python. Its fixed-width format was investigated, accidental-death records were filtered using the relevant manner-of-death code, and 500 records were extracted and checked.

The dataset is from the United States and is intended for statistical use. It does not provide the family contacts or institutional holding-location information required for TraceKin's operational workflow. Its applicable data-use restrictions must be respected.

## Research conclusion

The reviewed sources demonstrate the importance of injury-mortality research, deceased-person identification, family tracing, centralised case management and privacy protection.

Existing systems provide useful examples, but TraceKin proposes to focus on the management of identified deceased-person records, institutional holding-location updates, family enquiries and controlled verification workflows.

The project will use suitable anonymised secondary data for research and clearly labelled test records for demonstrating operational features.