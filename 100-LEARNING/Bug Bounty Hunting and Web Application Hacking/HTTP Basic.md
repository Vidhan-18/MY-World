- What  page (or endpoint) to fetch  --> GET/HTTP/1.1
- What website (or host) to fetch from  --> HOST: nahamsec.com
- Browser information including name version and etc.  --> User-Agent: Mozilla/5.0 (Macintosh;intel Mac OS X 10.9; rv:50.0 )
- What type of data to send/receive  --> Contain-type:
- Authorization header allowing you to fetch data  --> Authorization: Bearer SOMETHING_HERE
- What site/page sent you this new page  -->  Referrer: http://www.google.com/

# Commonly Used HTTP Methods
- GET to fetch data 
- HEAD does the same thing as get but doesn't shown the full response 
- POST to create or change data 
- PUT to replace or modify data 
- DELETE to delete data 
- OPTIONS to see communication option (GET POST DELETE HEAD PUT etc.)

# Most Common Response Status Codes
- 200 range - Successful response
- 300 range - Redirects 
- 400 range - 
	- 401 - Unauthorized Access
	- 403 - Forbidden or no access to resources
	- 404 - Not found or file doesn't exist
	- 405 - HTTP method not allowed 
- 500  -  Internet error where server doesn't know how to handle the request 