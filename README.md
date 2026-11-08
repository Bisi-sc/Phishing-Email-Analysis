# Phishing-Email-Analysis


Time: Mon, 25 Jan 2021 22:41:18 -0800 (PST)
Delivered to: themajoronearth@gmail.com
Subject: A Hope to CoCanDa
From: "Bill" <billjobs@microapple.com>
Return-path: <billjobs@microapple.com>
Reply-to: negeja3921@pashter.com
Email service used: emkei.cz



## Case Study - The Planet's Prestige (CoCanda)
    - Virtual environment was setup to investigate this email threat
    - Analyzing email content was carry out with different tools such as;
      VirusTotal, AbuseIPDB, CyberChef, Browserling
    - For Header analysis and File analysis, MxToolbox, Hybrid Analysis, Gary Kessler file signature
      and online tools such as ExifTool, ExcelTool.io and Hexed.it was used for this investigation
    - The analysis was a challenge to help develop analytical skill in investigating and reporting

## Summary

I investigated a suspected phishing email threat that was received by the CoCanda Representative, an Amry Major 
after a Tabletop-exercise which was presided by the President of the Planet was carried out to discuss the civil unrest and abduction 
of Cocanda citizens. The email was analyzed to identify the threat actor - sender, investigate the spoofed and suspicious attachments & files, 
file signature analysis, and write a report on related to the puzzle the threat actor in discovering the citizens.

## Investigation

There were several indicators of phishing on the email header, which the email claimed to be delivered from billjobs@microapple.com. Looking at the 
the analysis, it was discovered that the reply-to doesn't align with the return-path, showing a mismatch and true-positive alert that bill was not the actual sender rather 
the reply-to email negeja3921@pashter.com was the actual author. This was confirmed with the DNS text-records, after the carrying out open source research to investigate 
the domain since the Sender Policy Framework failed. In the email header, the email claimed to originate from microapple.com which after checking the IP address 93.99.104.210 
it belongs to another domain and the threat actor used another email service called emkei.cz which is a fake mail service used to send spoofed email and demanding a ransome.

On the other hand, an attachment was sent named PuzzleToCoCanDa.pdf, which Gary Kessler's file signature franework was used to check the integrity of the attachment.
Further investigation revealed that the attachment was not a PDF file but a ZIP extension with three (3) file evidence. The files integrity were checked and renamed to the right 
extensions.
        - DaughtersCrown.JPEG which shows proof of the abducted President's daughter
        - GoodJobMajor.PDF which confirms the threat actor's motives and proof.
        -Money.xlsx containing an excel sheets which was used to decode Base64 hidden message that decoded the attacker's location.

## Outcome 

I documented my findings and answered the below investigation questions:

    * What is the email service used by the malicious actor? - emkei.cz
    * What is the Reply-To email address? - negeja3921@pashter.com
    * What is the file-type of the received attachment which helped to continue the investigation? - .ZIP
    * What is the name of the malicious actor?- Pestero Negeja
    * What is the location of the attacker in this Universe? - The Martian Colony, Beside Interplanetary Spaceport
    * What could be the probable C&C domain to control the attacker’s autonomous bots? - pashter.com

After my documentations, I was able to draw out conclusion that this was a true positive alert with several indicators and sent my investigation report to the responsible team for decision 
making. 

## Conclusion

The investigation identified several indicators such as disguised attachments, SPF failure,a suspicious return-path that doesn't match with the reply-to and a masqueraded spoofed sender. The 
report pointed out hat Pestero Negeja was responsible for the malicious email and that the domain pashter.com is associated with the attacker's C2 infrastructure.

It is recommended that DNS text-record email authentication controls such as SPF, DKIM, and DMARC be enforced in order to identify suspicious senders and blocked domains that are not public. 
Users should also receive phishing awareness training. Malicious attachments should always be purged and open in an isolated environment. However, users should be trained on the phishing 
awareness campaigns to help minimize social engineering attacks that are commonly directed to users.

## Final Assessment

Emails should be treated as potentially malicious if they are not verified and content checked. The email was malicious and formed part of a targeted social engineering attack. Email-header 
analysis, file signature verification, and metadata examination were essential in revealing the attacker's identity and location to solve this case.




