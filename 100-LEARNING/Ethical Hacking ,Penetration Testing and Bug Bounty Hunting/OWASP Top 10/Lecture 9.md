# Broken Access Control
- Restricted users access not properly handled==(MFLAC)==.
- **Example :**
	- There is a login portal for school having 3 access levels.
	- 1.Student, 2.Teacher, 3.principle.
	- Students should access and manage his own attendance, Teacher should be allowed to see/modify students data and Principal should have access to teachers and students data.
	- ==IF access control is not configured, student is able to modify other and teachers data also.==
# Why BAC Happens
- Due to lack of effective Access Control between 2 roles.
- Best Example in Banking Sector is **Maker and Checker** Roles.
- ==IF maker is able to bypass checker's functionality, then its a Flaw.==
# What can be achieved by BAC?
- **Privilege Escalation:**
	- Horizontal Escalation - ==user to user==
	- Vertical Escalation - ==user to admin / admin to super admin
- **Cross Origin Resource Sharing.
- Access to API with missing access controls for **POST,PUT,DELETE.**
- **Allowing Primary Key to ==view/edit/modify/change== someone's data.
- **Metadata Manipulation such as replaying JWT access control tokens.**
# How do we fix BAC issues
- Implement Strong Access Control mechanism.
- Only Effective if enforced in trust server side code or server less API.
- Tokens Auth. should be invalidated as soon as Logout.
- Decisions should not be made by plain cookies preas like ==user=admin, acess=super admin, roles=tiktoker.==
