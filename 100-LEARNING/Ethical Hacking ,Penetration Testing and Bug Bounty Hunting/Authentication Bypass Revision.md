# How does the Authentication Bypass work 
- When an attacker modifies the request and when the web application only checks the client side code, authentication bypass takes place.
# Different Methods of Authentication Bypass we learnt:
- OTP Bypass
- Captcha Bypass
- true/false - 0/1 conditions to bypass
# live Authentication Bypass methods which we saw:
1. Healthie : 
		Changed status from 0 to 1
2. BMW India : 
		Change "error" to "success"
3. 99 Acres : 
		Changed parameter "verificationStatus" to true from false
4. Star Quik : 
		Sometimes such websites show a logic flaw where 0000 OTP can be bypassed for which the developer did not set any restrictions.
5. Stylecracker : 
		Sometimes websites do not have a response when the OTP is incorrect. By trial and Hit  Method we find out that by inserting value live 1 (in this example) or true or sometimes status code 200 or such other characters we can bypass the logic.
# live Captcha Bypass:
- Here we understood that by manipulating response to positive values we can bypass captcha which are only validated at the client side and not at the server side.
# Live Authentication Bypass to Account Takeover:
1. **WforWoman**
	- Here we logged in using the right OTP, intercepted the response and changed the "id" parameter to another value so that we could log in into someone else's account using our correct OTP.
2. Misrii
	- Here again we entered the right OTP, and to login into another user's account we changed the "user_id" parameter's value.
# Authentication Bypass due to OTP Exposure
- Sometimes web applications revel the OTP sent to the victim in the response itself. The attacker can use the OTP to login on behalf of the user. Two such websites which we saw were, tokree and Bank Website.
# Authentication Bypass of 2FA
- Here after logging out, we changed the "mfa_enabled" parameter to 0 from 1 due to which the 2FA authentication got disabled and the attacker was able to bypass the 2FA. such attacks can harm the user when the user highly relies on 2FA.
# Authentication Bypass Mitigations
- Do not rely on Client side verification instead make checks on server side too 
- User authentication based on strong tokens such as JWT Tokens.
- Use authentication using encrypted data like AES, SHA-1 etc.
# Severity of Authentication Bypass
- Vulnerability with highest severity as an account takeover can be done.
# Impact on Business due to Authentication Bypass.
- Any attacker can see other  user's details.
- Loss of PLL