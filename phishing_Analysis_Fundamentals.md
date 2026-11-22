# TryHackMe Writeup: Phishing Analysis Fundamentals
Platform:TryHackMe  
Internship:DG Interns Hub  
Week:Week 5 
Date Completed:11/16/2026  
Status:Completed

## Task 2: The Email Address
Identify the domain used in the following email address:
hatsalesman@tryhatme.com

tryhatme.com


## Task 3: Email Delivery
Which protocol is responsible for sending an email from a client to a mail server?

SMTP


Which service is used to look up the recipient domain’s mail server?

DNS


Bob wants to access his email from multiple devices, including his phone and laptop.
Which protocol should he use?

IMAP


## Task 4: Email Headers
What is the full subject line of email1.eml?

Help protect your budget by protecting your home


View the message source of email1.eml using Thunderbird in your VM.
What the IP address listed as the X-Originating-Ip?

43.255.56.161


## Task 5: Email Body

Open up the email2.txt file to view the source of an attachment.
What is the Content-Type of the attachment?

application/pdf


What is the name of the attachment from the previous question?

zmqpalgh.pdf


Decode the base64 string using either a PDF converter or CyberChef.
What is the hidden flag value?

THM{BENIGN_PDF_ATTACHMENT}


## Task 6: Types of Phishing
Which reputable organization is being spoofed in this phishing attempt?

Home Depot


What is the sender's email address?

support@teckbe.com


Inspect the email message source.
What is the defanged X-Originating-IP?

103[.]234[.]236[.]83


Continue analyzing the email message source.
Which mail server generated the Authentication-Results header?

atlas102.free.mail.gq1.yahoo.com


## Task 7: Conclusion
What attack, signified by the acronym BEC, uses a compromised email to trick employees into fraud?

Business Email Compromise


