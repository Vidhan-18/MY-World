# What is No Rate Limit?
- An attacker will send x number of requests to a web server and the server will act on each request. Since the web server does not validate the number of requests and does not limit them this makes it more dangerous.
# What can be done using No Rate limit Attacks?
- Account takeover
- Multiple Account Creation
- DOS
# Steps to perform No Rate Limit Attacks:
- Capture the request in Burp
- Send the request to Intruder
- Choose the target position
- Choose the payload
- Enter the payloads
- Start the Attack
# Create Multiple Accounts using No-RL Attack:
- As we saw in the Voot vulnerable application, we could use a set of different emails to create multiple accounts on Voot web application by setting the payload position on email id and choosing the correct payload.
# Account Takeover dure to OTP Bypass using No-RL Attack:
- Here we will send web application x requests and the server will act on each request. In each request we will be changing the OTP usually incrementing it by 1 so that one such request will be present which shall bypass the OTP thus leading to an Account Takeover.

- Note : remember to use the throttle option so that before two requests sent to the web server Burp Suite can wait for considerable time, else the web server might block the request.

- To check if the OTP is right or not always keep an eye on the following
	- Grep Parameter
	- Content Length
	- Status
# No Rate Limit Protection Bypass:
- We will bypass the protection by RACE and Rotating IP Address thus sending x number of right OTP Token, Password we can successfully crack the code 
- Example Instagram : https://www.hackread.com/hacker-reports-hack-instagram-flaw/
- Adding Headers like X-originating-IP
# No Rate Limit Python Script:
- We automated the entire process and created a python script to check if the website is vulnerable to No RL. Although automation is inevitable the results can be tentative from the scrip, confirm with burp for a thorough No RL Attack!
- **Link to script :** https://www.hackread.com/hacker-reports-hack-instagram-flaw/
# BurpFakeIP Tool :
- There's a tool which can be loaded to Burp Suite in order to generate Fake IP’s.
- **Link to tool:** [https://github.com/TheKingOfDuck/burpFakeIP.git](https://github.com/TheKingOfDuck/burpFakeIP.git)
# No RL Mitigations:
- Limit requests based on user
- Do not verify only at client side 
- Never Rate Limit users based on IP