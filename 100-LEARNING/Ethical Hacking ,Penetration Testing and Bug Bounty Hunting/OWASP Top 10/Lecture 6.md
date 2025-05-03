# 
- when any application functionality is broken/weak and attacker is able to bypass the authentication using session token flaws, brute force, no rate limiting, password compromise using response manipulation or any other flaws which can give any attacker temporary or permanent access to the users identity.
- OTP Bypass
- Captcha Bypass
- Common Passwords Brute Force
- 2FA Bypass
# Why BA Happens
- Manipulated Response is interpreted by the application
- No Rate Limit
- Lack of session Management
# What can be achieved by BA?
- Temporary Access to Useers account(TATO)
- Permanent Access to users account(PATO)
- Attacker can modify and alter the user details
- Accounts can be used for malicious purposes to conduct attacks
# How do we fix BA issues
- **Usage of Strong Auth(JWT,SAML, OAuth)**
	- Input validation
- **Do not allow Default or weak Creds** - Escaping is the primary means to make sure that untrusted data can't be used to convey an injection attack. There is **no harm** in escaping data properly - it will still render in the browser properly. Escaping simply lets the interpreter knows that the data is not intended to be executed, and therefore prevents attacks form working.
- **Rate Limit** -- using safe interfaces
- Usage of Server side secure session management that generates **high entropy secure** sessions