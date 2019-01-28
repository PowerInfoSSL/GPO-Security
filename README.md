# GPO-Security
Advanced Windows Security


After windows 7 and windows server 2008, Microsoft changed her policy about Auditing in Group Policy, as we know Group Policy is one of the best management tools in Domain Networks, in the oldest GP it have just nine Item for Auditing but in new version or new GP it have 53 different Items for Audit.

Its have an more advanced items to audit and we can set custom audit to dont capture so many log we didn't need them , for example we can set disconnect terminal connection audit in the login section not every login event .

But it have a very small change to how it apply to computers and objects, and in this article we explain how to implement Advanced Security Auditing correctly.

How to Access Advanced Security Audit: from GPO Editor expand this path:

Computer Configuration > Policies > Windows Settings > Security Settings > Advanced Audit Policy Configuration 

you can see different category of Auditing Policy each category have different Auditing option you can decide to enable it or disable.

Note: if you configure one of nine Audit Policy and some items in Advanced Audit Policy , when you execute RSOP.msc , what you see is just simple 9 Audit policy and not Advanced Audit Policy for better understand your Audit Policy applied to you system, we recommend to use auditpol.exe with this parameter:

auditpol.exe /get /category:*



or you can set defined category.
