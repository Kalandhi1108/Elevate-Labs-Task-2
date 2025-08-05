# Elevate-Labs-Task-2

Date: 05.08.2025

Objective: Identify phishing characteristics in a suspicious email sample

Legitimate email for comparison
Sample Email:
 From: Netflix info@mailer.netflix.com
 Subject: Your payment was successful
   Hello [Your Name],
   Thanks for your payment.
   Your Netflix membership has been renewed. Here are the details:
   Plan: Standard (HD)
   Monthly Price: ₹499
   Next Billing Date: September 5, 2025
   To view your account details or make changes, visit your Account page.
   Enjoy watching!
                        – The Netflix Team
Need help? Visit the Netflix Help Center

Tools Used for analyse Email Header
  -Mxtool Analyser 
(Legitimate result where attached ..)

STEP 1: Obtain a sample phishing email
Example -  Sample Phishing Email (Fake Netflix Notification)

STEP 2 : Examine Sender's Email Address for Spoofing
Look at this sender:   support@netfliix-help.com
What’s wrong?
*Netflix's real domain is @netflix.com or @mailer.netflix.com
*This one has "netfliix" (extra 'i') and "help.com", which is spoofed and misleading

STEP 3: Check Email Headers for Discrepancies
Check the email headers :Tool used - Mxtool Analyser
    - By pasting the email header on that tool , it maily checks the SPF,DKIM,DMARC mainly these header check the email is authenticated or not

STEP 4 : Identify Suspicious Links or Attachments
Hover over this link:
 ---> Update Account Now
 check the URL on tools like Virustotal , URLVoid it shows the result legitimate or not if it is in database , sometimes it doesnt show any result or it where not in database in that case the link is not meant to be legitimate .
 In this  link : (netfliix-billing-fix.com) - This is fake by the name of the header 
STEP 5: Look for Urgent or Threatening Language

"Your account is on hold"
"Update immediately"
"Failure to act will result in suspension"

STEP 6: Mismatched URLs (Hover to See)
Netflix Account Login - Looks real but actually goes to a .ru domain.

STEP 7:Check for Grammar or Spelling Errors
support@netfliix-help.com - Spelling Mistake

STEP 8:  Summarize Phishing Traits Found

The email shows clear signs of phishing. It uses a **spoofed sender address**, coming from `netfliix-help.com`, which is designed to look similar to Netflix’s legitimate domain. The message likely **fails SPF, DKIM, or DMARC authentication checks**, which can be verified by inspecting the email headers. It contains a **suspicious link** pointing to `netflix-billing-fix.com`, a domain unrelated to Netflix, and employs **urgent and threatening language** urging the recipient to "update immediately" to avoid account suspension. The email includes **mild grammar and spelling errors**, and when hovering over links, the URLs are **mismatched and lead to untrusted domains**. Finally, it opens with a **generic greeting**—"Dear Valued Customer"—rather than using the recipient’s real name, further suggesting it is a phishing attempt rather than a legitimate communication.


Mitigation Strategies:

 For Individuals:

 -->Double-check the sender’s email domain.
 -->Hover over links to see the actual URL before clicking.
 -->Never click suspicious links or download unexpected attachments.
 -->Enable Two-Factor Authentication (2FA) on all major accounts.
 -->Stay educated about common phishing tactics.
 -->Use “Report Phishing” features in Gmail, Outlook, etc.
 -->Avoid responding to emails asking for personal or financial info.
 -->Keep your browser and antivirus software up to date.

 For Organizations:
 
 -->Conduct regular security awareness training for employees.
 -->Implement email filtering and anti-phishing gateways.
 -->Use SPF, DKIM, and DMARC to validate email authenticity.
 -->Monitor inbound/outbound email traffic for anomalies.
 -->Enforce strong password and 2FA policies across the company.
 -->Run phishing simulation campaigns to test staff readiness.
 -->Create and enforce a cybersecurity incident response plan.
 -->Log and audit all email activities for early detection.











