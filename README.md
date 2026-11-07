# Phishing-Email-Analysis


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
the analysis, it was discovered that the reply-to doesn't align with the return-path, giving a true-positive alert that bill was not the actual sender rather 
the reply-to email negeja3921@pashter.com was the actual author. This was confirmed with the DNS text-records, 


