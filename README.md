# CS-305 Artemis Financial Retrospective

> Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

Artemis Financial needed their financial planning software to be secure. Therefore, I modernized their software to incorporate industry standard security best practices. This allowed their customer's data and financial information. I did this by implementing file verification through SHA3 hashing to create a checksum. The HTTPS protocol was also implemented to further enhance the web interface's security.

> What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

I believe I was able to correctly identify all of the software vulnerabilities after analyzing the client's requirements and running a dependency check. This allowed me to securely code the hashing function.

Applying industry standard best practices for secure coding is essential for a company’s overall wellbeing. Without secure coding best practices, company assets such as money, card numbers, trade secrets, personal information, and passwords could be accessed by attackers. 

These attackers could use this obtained information to steal money from the company or its consumers. They could also use obtained trade secrets to gain an advantage in the market. Or they could DDOS attack your website and create downtime that results in major losses in revenue.

If any of these attacks successfully occur, there could be major regulatory fines and penalties that could cost your company great sums of money as well as consumer confidence that may not ever be re-obtained. Therefore, security vulnerabilities could ultimately lead to the collapse of the company, and secure coding practices should be taken into consideration throughout the entire SDLC.

> What part of the vulnerability assessment was challenging or helpful to you?

I believe the most challenging part of the velnerability assessment report was interpretting the client's needs. This led to many questions that needed answered before an implementation was done. I needed to determine how secure communications would value the company, if the company made international transactions, what government restrictions would affect the application, what the external threats were, and how modernization requirements of open-source libraries would affect the security of the application. After answering these questions, it became more clear on how to proceed with the security implementation.

> How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

In order to increase the security of the application, a vulnerability assessment report was conducted. This included interpretting the client's security needs, determining which areas of security were affected by the application, manually reviewing the codebase for security vulnerabilities, and then analyzing a dependency report through static testing. This allowed me to come up with a complete mitigation plan for the identified security vulnerabilities.

> How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

After implementing the checksum verification and HTTPS protocol, functional testing was performed. This allow me to test wether the application could be successfully deployed. It also allowed me to check wether the hashing function was producing the desired results. After the code was refactored, another static dependency check was performed to see if any new vulnerabilities were introduced.

> What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

Many tools were used to identify security vulnerabilities. These tools included the OWASP Maven Dependency-Check plugin, the CVE List Database, and the National Vulnerability Database. 

Throughout this course, knowlege was gained on the following topics:

* Establishing secure authentication and session management processes.
* Implementing a robust access control design for multi-tenant web applications.
* Defending against cross-site scripting, cross-site request forgery, and clickjacking.
* Protecting sensitive data while it is stored or in transit.
* Preventing SQL injection and other injection attacks.
* Ensuring safe file I/O and upload.
* Using effective logging, error handling, and intrusion detection methods.
* Following a comprehensive secure software development lifecycle.

> Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

After completing the Artemis Financial Vulnerability Assessment Report and the Practices for Secure Software Report, it would be worthwhile to demonstrate my ability to assess a client's security needs, identify current security vulnerabilities, and implement mitigations for identified security vulnerabilities. From this assignment, it is noteworthy to point out that after functional testing, the refactored code worked correctly. Therefore, I successfully implemented a checksum function using SHA3-256 and the HTTPS protocol in a Spring Boot application. It is important to be able to perform static security testing through dependency tests, which I was able to successfully complete using the OWASP Maven Dependency-Check plugin.
