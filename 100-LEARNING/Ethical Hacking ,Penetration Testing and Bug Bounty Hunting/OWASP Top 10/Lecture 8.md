# XML External Entities (XXE)
- Applications those parse XML Input.
- **XML input containing a reference to an external entity is processed by a weakly configured XML parser.**
- XXE may lead to disclosure of **sensitive data, SSRF, Port Scanning, DOS(denial-of-service), or RCE(Remote code execution).**
# Why XXE Happens
- **Incorrect processing on XML input and parsing.**
# What can be achieved by XXE?
-  XXE may lead to disclosure of
	- **Sensitive data**==(/etc/passwd)==
	- **SSRF**==(hit a request to your collabrator /server)==
	- **Port Scanning**==(enumerate 127.0.0.1 and ports)==
	- **Denial Of Service**
	- **RCE**==(Remote code execution OOB)==