afa- Insecure Direct Object Reference occur when an application provides direct access to objects based on user-supplied input. This is allow a malicious attacker to access data belonging to other user by manipulating the request.
--> **Retrieve Data :** 
			    Will allow you to retrieve data such as **Personally identifiable information(PII), Phone Number, Address, Receipts/invoices,** etc.
--> **Modify or Delete Data :**
				Allows you to modifies someone else's information such as **Email address, Password, Account Details,** etc

- Understand how the application works :
	- How does if fetch data 
	- how does it create new data 
	- how does it modify or delete data
- Look for any numerical IDs in the requests
- Create two users in order to have accurate data (userID, objectID, etc).
- Sometime application use "encryption" to obfuscate information such as the userID (such as base64)
- Automate using burp
- Sometime application use UUID's instead of numeric id's. UUID's are unpredictable long strings. They look like this : bfe5ca-9afa-11ea-bb37-0242ac130002. They don't protect against IDOR's but they do make it harder to exploit. Sometimes applications leaks the UUID, on purpose or by accident. For example, when you visit another user's profile, they may have profile photo that's stored on the website in a folder the as there UUID.
- 