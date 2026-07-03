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

## Email Header Analysed 
<img width="1140" height="821" alt="Capture" src="https://github.com/user-attachments/assets/ff36d7a3-08fc-4fff-820b-cfa2cd601c52" />

## Analysis Contd
<img width="1124" height="418" alt="MXToolbox" src="https://github.com/user-attachments/assets/93469d14-178c-4980-b919-3d1fe93b4a31" />

## Relay info
<img width="1466" height="811" alt="Relay info" src="https://github.com/user-attachments/assets/4e6d2c07-a6d0-4485-9e17-e83c726332bd" />

## Relay info contd
<img width="1422" height="592" alt="Relay info2" src="https://github.com/user-attachments/assets/7c7f64d9-c69c-402c-a6b5-933560d31621" />

## SPF & DKIM INFO
<img width="1202" height="830" alt="SPF DKIM" src="https://github.com/user-attachments/assets/167593ff-1a9f-4ca9-bd7e-d1017257e2a9" />
