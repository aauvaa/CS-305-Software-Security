# CS-305-Software-Security
CS 305 coursework focused on software security, secure coding practices, encryption, and vulnerability assessment.

# CS 305 Portfolio Reflection

## Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?

Artemis Financial was the client for this project. The company wanted to improve the security of its software application and protect sensitive financial and client information. My task was to identify security vulnerabilities and refactor the application using secure coding practices. This included adding checksum verification, securing communications with HTTPS, and checking the application's dependencies for known vulnerabilities.

## What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?

I did well identifying areas where additional security could be added without affecting the existing functionality of the application. I used OWASP Dependency-Check to identify known vulnerabilities in third-party dependencies and reviewed the application for security issues. Secure coding is important because vulnerabilities can expose sensitive information or allow attackers to compromise an application. For a financial company like Artemis Financial, strong software security helps protect customer information, maintain customer trust, and reduce the financial and reputational damage that could result from a security incident.

## Which part of the vulnerability assessment was challenging or helpful to you?

One of the most helpful parts of the vulnerability assessment was using OWASP Dependency-Check. It showed me how an automated security tool can identify known vulnerabilities within an application's dependencies. It was also challenging because the scan can identify vulnerabilities that already exist in the provided code base, so I had to understand which issues were already present and make sure my changes did not introduce additional vulnerabilities.

## How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

I increased the layers of security by implementing SHA-256 hashing for checksum verification, generating a certificate, configuring the application to use HTTPS, and performing dependency analysis. Each security control addressed a different area of the application. SHA-256 helped verify data integrity, while HTTPS protected data during transmission. In the future, I would continue using tools such as OWASP Dependency-Check along with manual code review, testing, and current secure coding standards to determine which vulnerabilities need to be addressed and which mitigation techniques are appropriate.

## How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

After refactoring the application, I performed both secondary and functional testing. I verified that the SHA-256 checksum method compiled correctly, the /hash endpoint returned the expected information, the PKCS12 keystore loaded correctly, and the Spring Boot application successfully ran over HTTPS on port 8443. I also ran OWASP Dependency-Check again and reviewed the results to make sure my changes had not introduced additional dependency vulnerabilities.

## What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

Some of the most useful resources and tools were OWASP Dependency-Check, Java's MessageDigest class, Java keytool, Spring Boot, SHA-256, and HTTPS configuration. I also learned the importance of testing an application after making security changes instead of assuming that the changes are secure simply because the application compiles. These tools and secure coding practices will be useful in future software development and security projects.

## Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

I could show employers the Artemis Financial Practices for Secure Software Report as an example of my ability to identify vulnerabilities and improve the security of an existing application. The project demonstrates that I can implement SHA-256 hashing, configure HTTPS using a certificate and keystore, perform dependency vulnerability scanning, and test an application after making security changes. It also shows that I understand why multiple layers of security are important when developing software.
