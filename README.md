# cyber-internship-task-2
Task 2 of Cybersecurity Internship – Phishing Email Analysis with header breakdown, social engineering indicators, and professional report. ``
# 🎯 Task 2 – Phishing Email Analysis (Cybersecurity Internship)

## 📌 Objective:

The goal of this task is to **analyze a phishing email**, identify red flags using **header & content inspection**, and document the **tactics used by attackers** to manipulate or trick users. This task strengthens skills in **email forensics**, **threat recognition**, and **social engineering detection**.

---

## ✉️ Phishing Email Sample

```
Subject: 🚨 Urgent: Account Access Limited Until Verification
From: support@paypa1.com
To: rohithrachapudi@gmail.com

Dear Rachapudi Rohith,

We’ve detected unusual activity on your PayPal account which may indicate fraudulent access. For your security, we’ve temporarily limited access to your account.

Please confirm your identity and secure your account by verifying your details immediately:

🔗 https://paypa1.com-update@is.gd/kU2qKS

To restore full access, complete this verification within 24 hours. Failure to do so may result in permanent account suspension.

Thank you for choosing PayPal.

Regards,  
PayPal Account Security Team
```

---

## 🧠 Red Flags in Email Body

| 🔍 Indicator                    | 📌 Reason                                                    |
| ------------------------------- | ------------------------------------------------------------ |
| **Fake Sender Domain**          | `paypa1.com` instead of `paypal.com`                         |
| **Personalized But Inaccurate** | Real companies don’t use your full name from unknown sources |
| **Suspicious Link**             | `is.gd` shortening with embedded spoofed domain              |
| **Urgency and Threat**          | “Complete within 24 hours” triggers fear response            |
| **Brand Spoofing**              | Pretends to be PayPal with copied signature formatting       |

---

## 🧾 Header Analysis

*(Performed using tools like [MxToolbox](https://mxtoolbox.com/EmailHeaders.aspx) or [Google Admin Toolbox](https://toolbox.googleapps.com/apps/messageheader/). Screenshots included in the repository.)*

### 🔎 Simulated Header Sample

```
From: support@paypa1.com
Reply-To: attacker@darkwebmail.cn
Return-Path: <attacker@darkwebmail.cn>
Received: from unknown202.evilnet.ru (IP: 185.203.26.91)
SPF: Fail
DKIM: None
DMARC: None
Message-ID: <PP-34847712@darkwebmail.cn>
```

### 🚩 Header Red Flags:

* ❌ Fake sender domain mimicking PayPal (`paypa1.com`)
* ❌ Reply-To and Return-Path point to attacker-controlled server
* ❌ No SPF/DKIM/DMARC – no authentication validation
* ❌ Received path shows non-legit Russian domain server
* ❌ Message-ID domain doesn’t match PayPal structure

---

## 🛡️ What I Learned

* Deep inspection of phishing emails using both **visual and technical methods**
* How attackers use **personalization and fear** for manipulation
* Role of **email headers and authentication records** (SPF/DKIM/DMARC)
* Real-world tools for header inspection
* Greater awareness of how threat actors **exploit trust and urgency**

---

## 🗂️ Repository Structure

```
cyber-internship-task-2/
├── phishing_email_sample.txt
├── header_analysis.txt
├── screenshots/
│   ├── email_body_screenshot.png
│   ├── header_analysis_tool_result.png
├── README.md
```

---

## 🏁 Final Words

This task gave me a practical understanding of how phishing emails operate. By using real-world examples and professional inspection methods, I strengthened my ability to detect threats, analyze malicious behavior, and apply defensive strategies. These are critical skills for any future cybersecurity professional.

> 📢 I am committed to growing further and proving my capabilities throughout this internship.
