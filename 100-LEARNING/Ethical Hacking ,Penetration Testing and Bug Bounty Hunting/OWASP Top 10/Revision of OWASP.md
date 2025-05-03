# What is OWASP?
- OWASP stands for Open Web Application Security project which is a standard awareness document for developers and web application security. It represents a broad consensus about the most critical security risks to web applications. It categorizes vulnerability of each type.
# What is Injection?
- injection flaws, such as SQL occur when untrusted data is send to a web application as part of command or query. The attacker's payload can trick the web application into execution unintended commands or accessing data without proper authorization.
# What is Broken Authentication? 
- Application functions related to authentication and session management are often implemented incorrectly, allowing attackers to compromise passwords, keys, or session tokens, or to exploit other implementation flaws to assume other users  identities temporarily or permanently.
# What is Sensitive Data Exposure?
- When web application and APIs do not properly protect sensitive data, such as financial, healthcare, and Pll. Attackers may steal or modify such weakly protected data to conduct credit card fraud, identity theft, or other crimes.
# What are XML External Entities?
- Many older or poorly configured XML processors evaluate external entity references within XML documents. External entities can be used to disclose internal files using the file URI handler, internal file shares, internal port scanning, remote code execution, and denial of service attacks.
# What is Broken Access Control?
- Restrictions on what authenticated users are allowed to do are often not properly enforced. Attackers can exploit these flaws to access unauthorized functionality and /or data, such as access other users accounts, view sensitive files, modify other users data, change access rights, etc.
# What is Security Misconfiguration?
- Security misconfiguration is the most commonly seen issue. This is commonly a result of insecure default configurations, incomplete or ad hoc configuration, open cloud storage, misconfigured HTTP headers, and verbose error messages containing sensitive information. Not only must all operation systems, frameworks, libraries, and applications be securely configured, but they must be patched / upgraded in a timely fashion.
# What is Cross Site Scripting?
- XSS flaws occur whenever an application includes untrusted data in a new web page without proper validation or escaping, or updates an existing web page with user-supplied data using a browser API that can create HTML or JavaScript. XSS allows attackers to execute scripts in the victim's browser which can hijack user sessions, deface web sites, or redirect the user to malicious sites.
# What is Insecure Deserialization?
- Insecure deserialization often leads to remote code execution. Even if deserialization flaws do not result in remote code attacks, injection attacks, and privilege escalation attacks.
# What is Using Components with Known Vulnerabilities?
- Components, such as libraries, frameworks, and other software modules, run with the same privileges as the application. if a vulnerable component is exploited, such an attack can facilitate serious data loss or server takeover. Applications and APIs using components with known various attacks and impacts.
# What is Insufficient Logging and Monitoring?
- Insufficient logging and monitoring, coupled with missing or ineffective integration with incident response, allows attackers to further attack systems, maintain persistence, pivot to more systems, and tamper, extract, or destroy data. Most breach studies show time to detect a breach is over 200 days, typically detected by external parties rather than internal processes or monitoring.