# Sensitive Data Exposure (SDE)
- When any application or Api do not protect sensitive data properly like user account details, credit card details, passwords etc.
- Attacker can view this sensitive data and get access to internal network.
- GitHub Tokens and API keys Leakages(hackerone Snapchat Report).
- Sensitive Invoices Indexed by Google(Paypal Invoice reports).
- Insecure storage of Data also leads to SDE.

# Why SDE Happens
- No Proper access control over when exchanging sensitive data. 
- **API's not properly protected.**
- Lack of Robots.txt.
- Lack of Data Strip when saving at server.
# What can be achieved by SDE?
- Sensitive Information of the Users leak, ie- Transactions Details, Passwords.
- API keys.
- Tokens of Internal Protals only accessible to Domain Admins.
- Passwords, SSH Keys, aka **anythings that is sensitive**.
# How do we fix SDE issues 
- **Don't store sensitive data unnecessarily.**
- **Make sure to encrypt all SD at rest.**
- Disable caching Responses that has SD.
- Do not put keys, tokens in Github or anywhere in server.
- Implement **Access Control** for users (Maker Checker functionality)