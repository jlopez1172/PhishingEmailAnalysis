# 📧 Phishing Email Analysis – SOC+ Lab

This repository contains a practical walkthrough of analyzing a phishing email using real-world investigation techniques. The lab was conducted in a sandboxed Kali Linux VM and focuses on identifying email-based threats, parsing headers, and verifying sender authenticity.

## 🔍 Case Study

**Phishing Sample**: Spoofed OpenSea NFT sale confirmation 

**Suspicious Indicators**:
- Sender domain `notify.thinkific.com` does not match the display name “OpenSea NFTs”
- Reply-To address (`contacto@pixostudio.com`) differs from the sender address
- Embedded links redirect to malicious domains (flagged by VirusTotal)
- Microsoft authentication (`compauth`) failed; IP sourced from unrelated infrastructure

## 🧪 Tools Used

- Mozilla Thunderbird (for `.eml` viewing and inspection)
- Kali Linux (VirtualBox VM)
- VirusTotal
- MXToolbox
- WHOis / IPVoid
- SPF/DKIM/DMARC checkers

## 💡 Learning Outcomes

- Email header dissection: `From`, `Reply-To`, `Received`, `Message-ID`
- DNS and IP reputation analysis
- Link inspection and redirection tracing
- Identifying misaligned sender fields and spoofing tactics

## 📂 Files

- `Analysing Phishing Emails.docx`: Full lab write-up
- Sample `.eml` files available [here](https://github.com/rf-peixoto/phishing_pot/tree/main/email)

## 🛡️ Notes

Always analyze suspicious emails in a secure, isolated environment. This lab is intended for educational and defensive security purposes only.
