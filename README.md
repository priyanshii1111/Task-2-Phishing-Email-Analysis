# Task 2 – Phishing Email Analysis Report

## Project Overview
This repo contains my analysis of a phishing email sample for Task 2 of the Elevate Labs Internship Program.  
The goal was to spot phishing signs, analyze email headers, and understand how social engineering attacks work.

The email I analyzed is a fake “Microsoft Security Alert” message.

## Repository Contents
- README.md – This report  
- email_sample.png – Screenshot of the phishing email  
- header_analysis.txt – Header analysis results  
- observations.txt – Observations and phishing indicators  

# Phishing Email Analysis Report

## 1. Email Sample
The phishing email was taken from **CanIPhish**, a phishing simulation site.  
It pretends to come from **“Microsoft 365 Support”**, saying someone accessed your account and asking you to “recover” it.

## 2. Phishing Indicators I Found

**1. Suspicious Sender Address**  
The display name is “Microsoft 365 Support,” but the actual email is `support@office-365-notifications[.]com`.  
The domain isn’t Microsoft, which is a major red flag.

**2. Urgent/Threatening Language**  
The email tries to scare you with phrases like:  
- “Someone else has accessed your account”  
- “We require you to verify your identity”  
- “They might access your personal info”  
This is meant to push you to click fast without thinking.

**3. Suspicious Links/Buttons**  
The “Recover account” button doesn’t link to Microsoft.  
Hovering over it shows a different URL that could steal your credentials.

**4. Email Header Red Flags**  
From my header analysis:  
- SPF check failed or mismatched  
- DKIM signature missing  
- Return-Path doesn’t match the sender domain  
All of this points to spoofing.

**5. Generic Greeting**  
The email just says “Dear User.” Microsoft emails usually use your actual name.

**6. Grammar & Formatting Issues**  
Small spacing and wording mistakes suggest it’s mass-produced.

**7. Masked or Inconsistent Domains**  
Things like `john[.]doe@mybusiness[.]com` are used to hide the real domain.

**8. Fake Legitimacy Attempts**  
The footer has Microsoft’s official address to look real, but that doesn’t prove it’s legit.

## What to do with suspicious emails  
- Don’t click links or attachments  
- Report to your security team  
- Delete or quarantine the email  

## 4. Conclusion
This task helped me:  
- Spot phishing signs  
- Analyze email headers for fake/mismatched info  
- Recognize spoofed domains and shady links  
- Understand social engineering tactics

You can also check attached observation, header analysis files and screenshot of the phishing email sample that I analysed for reference.
 

and you can see the full analysis.
