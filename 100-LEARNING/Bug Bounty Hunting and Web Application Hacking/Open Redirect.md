- Open redirect happen when the web application takes an untrusted  input and redirects a user from web application to untrusted site or resource that will further form malicious purposes.
- The impact for Open Redirect is usually low , unless you are using it to escalate other vulnerabilities.
- Sometime the application may have security measures in place where developers defines a list of either trusted  or untrusted resources. In some cases, you may be able to bypass it, if you fully understand how it works 

# Filtering and Bypasses 
- https://example.com/login/?nextPage=https://google.com (allowed)

- https://example.com/login/?nextPage=https://evilsite.com (not allowed)

- https://example.com/login/?nextPage=https://evilsite.com/?google.com (allowed)