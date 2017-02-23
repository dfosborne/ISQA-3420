##Data Flow Diagram Dictionary  
###Entities  
**Developer:** The developer is responsible for uploading or submitting a software package in the system to be scanned by the "Check Software for OSS Components" process and then added to the "Licenses and Vulnerabilities of Software" datastore. They also have the ability to request for this information from the "Retrieve Software License and Vulnerability Info." process.

**Manager:** The manager is responsible for the retrieval and modification of software policy in the "Company Software Policy" datastore. They also request for software license and vulnerability information like the developer does.  

###Processes
**Check Software for OSS Components:** This process takes in a software package from the developer and then sends that data to the "NIST Vulnerabilities" datastore to determine known vulnerabilities, as well as to another process "Scan for OSS Components." It then receives "Vulnerability Results" and "License Scan Results." The "Check Software for OSS Components" then sends these to the "License and Vulnerabiities of Software" datastore and back to the developer.

**Scan for OSS Components:** This process receives data "Software Package" from process "Check Software for OSS Components" and determines if it contains any open source software. It then sends these results back to the process "Check Software for OSS Components."

**Retrieve Software License and Vulnerability Info.:** This process takes in a request from the developer or the manager for software licennse and vulnerability information. It then sends this request to the "Licenses and Vulnerabilities of Software" datastore to retrive that information. It receives "Software License and Vulnerability Results" and sends it back to the developer or the manager.

**Retrieve Software Policy:** 
###Data Flows


###Data Repositories
t
