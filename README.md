# CYBERSECURITY-HOME-LAB-PROJECTS
Email header analysis &amp; phishing investigation
## Overview
The Email claims to be from the MicrosoftAccount Team and warns the recipient about a suspicious login attempt from Russia...
## Tools Used
- MXToolbox Header Analyzer
- Raw email header view (mail client)
## Investigation Steps
1. Collected the raw email header.
2. Ran the header through MXToolbox Header Analyzer.
3. Checked SPF, DKIM, and DMARC results.
4. Verified sender domain and Reply-To address.
## Key Findings
- SPF authentication failed
- No DKIM signature
- No valid DMARC record
- Reply-To pointed to a Gmail account instead of Microsoft
- Sender domain did not match the organisation being impersonated
These findings strongly suggesst email spoofing and demonstrate how authentication failures and header analyses can be used to identify phishing attempts.
## Skills Practised
- Email Header Analysis
- Phishing Detection
- Email Authentication (SPF, DKIM & DMARC)
## Future Improvements
- Automate header parsing with scripts
- Compare results across different tools
- Build detection rules for a SIEM
<img width="1140" height="821" alt="Capture" src="https://github.com/user-attachments/assets/c22eecb8-e2a9-4021-bb11-f4aece720af8" />
