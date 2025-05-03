# What is XSS?
- XSS allows an attacker to execute arbitrary clint-side code on a victim's browser. XSS can be used for **Phishing, exfiltration data, account takeovers and more.**

# How does XSS works? 
- An attacker inserts a malicious script (or a Payload) into a victim's browser.
- When the victim encounters the script it executes in the victim's browsers.
- A malicious payload is able to perform any actions that the victim is able to perform.
- If the victim has special privileges it can be a serious vulnerability.
# Impact 
- Read / Modify / Delete content of any pages..
- Steal a users cookies or session and gain access to their accounts.
- serve malicious content like phishing.

# different type of XSS
- **Reflected XSS:**
			Payload is injected from the victim's request. 
			victim must click a malicious link or navigate to attacker-control property.
- **Stored XSS:**
			Payload is stored server-side and can be triggered by victim with no interaction outside of application.
- **Document Object Model (DOM) XSS:**
			The vulnerability is in the clint-side code versus the server-side.
			injection is still typically from the victim's request.

# Reflected XSS

| Request                          | Response             | Explanation     |
| -------------------------------- | -------------------- | --------------- |
| site.com/page?name=john          | hello, john          | Normal Request  |
| site.com/page?name=`<u>john</u>` | hello, `<u>john</u>` | No XSS Possible |
| site.com/page?name=`<u>john</u>` | hello, <u>john</u>   | Possible XSS    |
- In this example, the payload is injected into victims request using the "name" parameter. In order to work, the victim must click this this malicious link or navigate to an attacker-control property. `http://example.com/page?param=<payload>` 

# Stored XSS
- Also knows as persistent XSS
-  It stored the payload in the database.
- The payload is reflected back to the user when visiting a particular page.
--> One of the most famous stored XSS is on Tweetdeck.
![[Pasted image 20250308134059.png]]
- The payload  is stored server-side and can be triggered by a victim without any interaction outside of using the application.
-->Payload inserted at dropbox.com as the filename. Later on imported and shared via Facebook.
![[Pasted image 20250308134511.png]]


# DOM XSS
- DOM-based XSS vulnerabilities usually arise when JavaScript take data from an attacker-controllable source, such as the URL, and passes it to a sink that support dynamic code execution, such as `eval()` or `innerHTML`. This enables attackers to execute malicious JavaScript, which typically allow them to hijack other user account.
- DOM XSS happens when JavaScript reflect data from attacker control resources (for example the within the URL) and passes it to a function later on.
- 