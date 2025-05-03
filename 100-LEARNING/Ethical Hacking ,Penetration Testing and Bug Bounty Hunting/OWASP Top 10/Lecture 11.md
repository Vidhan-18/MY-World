# Cross Site Scripting (XSS)
- The attack allows attacker to execute **JavaScript :)**
- There are 3 types of XSS:
	- Reflected XSS
	- Stored XSS
	- DOM XSS
- RXSS : The application includes invalidated or unescaped users input as part of HTML Output, which can be used further for **ATO's**.
	- ==This attack, allows attacker to execute js in victims browser and hijack the session cookie leading to ATO.==
- SXSS : which is later viewed by another user or admin. (**V-ATO**)
- DXSS : client side attack, where untrusted input is passed in source and comes out of sink and executes.
# Why XSS Happens
- No sanitization or Escaping.
- Input is directly taken as the HTML output.
- bas Coding practices.
# What can be achieved by XSS?
- Account Takeovers
- Keyloggers
- Redirection
- and a lot more ...
# How do we fix XSS issues
- Input Sanitization
- Escaping and Encoding
- Web Application Firewall(WAF)