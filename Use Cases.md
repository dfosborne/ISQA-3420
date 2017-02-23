###Use Case #1
**Title:** Determine License and Vulnerability Information for Software 

**Primary Actor:** Mananger  

**Goal in Context:**  The manager is able to determine license and vulnerability information from information received for specfic software.

**Stakeholders:**  
-Manager: To receive clear and relevant software information   
-Developer: To provide the relevant software package information  

**Preconditions:**  
-Relevant information for the software is in the Licenses and Vulnerabilities of Software database  
-Accurate license and vulnerability information for software has been provided 

**Main Success Scenario:** Manager receives accurate license and vulnerability information for the requested software

**Failed End Conditions:** Manager receives inaccurate or invalid license and vulnerability information for the requested software

**Trigger:** Corporate mananger uploads or identifies software to which license and vulnerability information is provided


###Use Case #2
**Title:** Create New Software Policy 

**Primary Actor:** Manager  

**Goal in Context:** The manager is able to create a new software policy from requested software information 

**Stakeholders:**  
-Manager: To create a new software policy   

**Preconditions:**  
-Requested software license and vulnerabilities are provided  
-Current software policy information is provided to determine if policy exists  
-Accurate information is in the appropriate databases  

**Main Success Scenario:** Manager creates new software policy based on requested software information

**Failed End Conditions:** Manager creates new software policy when policy already exists because inaccurate information was provided to manager

**Trigger:** Manager submits new policy for software to be created


###Use Case #3
**Title:** Scan Software for Open Source Software (OSS) and NIST Vulnerabilities 

**Primary Actor:** Developer  

**Goal in Context:** The developer submits a software package to be scanned for OSS components and NIST vulnerabilites and the results are then returned 

**Stakeholders:**  
-Developer: The developer provides software package to be scanned  

**Preconditions:**  
-NIST Vulnerabilities database contains information about specific software package  
-Developer provides valid software packag

**Main Success Scenario:** The developer submits software package to be scanned and receives valid results

**Failed End Conditions:** The developer submits software package to be scanned but receives invalid results

**Trigger:** Developer submits software pacakge to be scanned
