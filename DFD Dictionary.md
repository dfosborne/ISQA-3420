##Data Flow Diagram Dictionary  
###Entities  
**Developer:** The developer is responsible for uploading or submitting a software package in the system to be scanned by the "Check Software for OSS Components" process and then added to the "Licenses and Vulnerabilities of Software" repository. They also have the ability to request for this information from the "Retrieve Software License and Vulnerability Info." process.

**Manager:** The manager is responsible for the retrieval and modification of software policy in the "Company Software Policy" repository. They also request for software license and vulnerability information like the developer does.  


###Processes
**Check Software for OSS Components:** This process takes in a software package from the developer and then sends that data to the "NIST Vulnerabilities" repository  to determine known vulnerabilities, as well as to another process "Scan for OSS Components." It then receives "Vulnerability Results" and "License Scan Results." The "Check Software for OSS Components" then sends these to the "License and Vulnerabilities of Software" repository and back to the developer.

**Scan for OSS Components:** This process receives data "Software Package" from process "Check Software for OSS Components" and determines if it contains any open source software. It then sends these results back to the process "Check Software for OSS Components."

**Retrieve Software License and Vulnerability Info.:** This process takes in a request from the developer or the manager for software license and vulnerability information. It then sends this request to the "Licenses and Vulnerabilities of Software" repository to retrieve that information. It receives "Software License and Vulnerability Results" and sends it back to the developer or the manager.

**Retrieve Software Policy:** This process is responsible for the retrieval of current software policies. It takes in a "Request for Current Software Policies" from the Manager, then sends this request to the "Company Software Policy" repository. It then receives "Current Software Policies" and sends this back to the Manager.

**Create New Policy Software:** This process enables the Manager to submit "New Policy for Software" and then adds it to the "Company Software Policy" repository.

**Edit Existing Policy for Software:** This process enables the Manager to submit an "Edit of Software Policy" and then it will add the edit to the "Company Software Policy" repository.


###Data Flows  
**Software Package:** The software package that is being sent from the Developer to "Check Software for OSS Components."  
**Software Package Name:** The name of the software package submitted by the Developer to be checked for vulnerabilities in the "NIST Vulnerabilities" repository.  
**License Scan Results:** The open source software results of the scanned software package.
**Vulnerability Results:** The vulnerability results of the software package.  
**Request for Software License and Vulnerability Info.:** A request submitted by the Manager or the Developer to receive software license and vulnerability information.  
**Software License and Vulnerability Results:** The retrieved results from the "Licenses and Vulnerabilities of Software" repository for the request submitted by the Developer or the Manager.  
**Request for Current Software Policies:**  A request submitted by the Manager to receive current policies for a specific software.  
**Current Software Policies:** The retrieved results from the "Company Software Policy" repository for the request submitted by the Manager for a specific software.  
**New Policy for Software:** New policy information for a specific software submitted by the Manager.  
**Edit of Software Policy:** Edit of existing policy for a specific software submitted by the Manager.  



###Data Repositories
**NIST Vulnerabilities:** This is an external database that contains information about known vulnerabilities with software.  
**Licenses and Vulnerabilities of Software:** This is an internal database that includes NIST vulnerabilities and open source software components for relevant company software.  
**Company Software Policy:** This is an internal database that contains the company's policies for software.
