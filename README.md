# CloudSEK_CTF-Writeup
Absolutely ✅ A **professional and polished README.md** will make your repo stand out. Here’s a draft tailored for your CloudSEK Hiring CTF writeup repo:

---

# 🕵️ CloudSEK Hiring CTF Writeup

Hello Dear Reader, my name is **ZestyPesky** and this is my detailed write-up for the **CloudSEK Hiring CTF**.

I managed to solve **4 out of 5 flags within the time limit**, and even discovered the **5th flag** after the event had ended.
This repository documents my **step-by-step solutions, methodology, and thought process** behind each challenge.

---

## 📑 Table of Contents

* [Overview](#Overview)
* [Challenges](#Challenges)

  * [Welcome Challenge – Flag 1](#welcome-challenge--flag-1)
  * [Hacking the Hacker – Flag 2](#hacking-the-hacker--flag-2)
  * [Attacking the Infrastructure – Flag 3](#attacking-the-infrastructure--flag-3)
  * [Bypassing Authentication – Flag 4](#bypassing-authentication--flag-4)
  * [The Final Game – Flag 5](#the-final-game--flag-5)
* [Key Takeaways](#key-takeaways)
* [Disclaimer](#disclaimer)

---

## 🔎 Overview

The **CloudSEK Hiring CTF** was designed to test candidates on real-world cybersecurity challenges, ranging from **OSINT and prompt injection** to **GraphQL exploitation, authentication bypass, and AWS SSRF attacks**.

It was an incredibly fun and challenging experience that tested both **technical skills** and **time management under pressure**.

---

## 🚩 Challenges

### Welcome Challenge – Flag 1

* OSINT investigation using email address.
* Repository commit analysis.
* Discovered the first real flag hidden in an older commit.

### Hacking the Hacker – Flag 2

* Telegram bot reverse engineering.
* Prompt injection to bypass bot restrictions.
* Audio (Morse code) analysis to retrieve the flag.

### Attacking the Infrastructure – Flag 3

* CloudSEK BeVigil APK analysis.
* Hardcoded GraphQL endpoint discovery.
* GraphQL introspection + privilege escalation via JWT forgery.

### Bypassing Authentication – Flag 4

* Leveraged credentials from previous step.
* Discovered MFA/backup code bypass via **hardcoded API keys**.
* Session cookie analysis to obtain user ID and generate admin backup codes.

### The Final Game – Flag 5 *(Solved after CTF ended)*

* SSRF via profile picture upload API.
* Exploited AWS metadata service to retrieve IAM credentials.
* Queried S3 bucket to uncover the final flag.

---

## 📌 Key Takeaways

* **OSINT is powerful** – even a small clue can lead to the next flag.
* **Prompt injection** is a real-world problem in chatbot security.
* **GraphQL misconfigurations** can lead to privilege escalation.
* **Hardcoded secrets** in code are dangerous.
* **SSRF into cloud metadata** can escalate into full cloud account compromise.

---

## ⚠️ Disclaimer

This writeup is strictly for **educational purposes**.
All vulnerabilities and flags mentioned here are part of the **CloudSEK Hiring CTF challenge** and **do not exist in any production environment**.

---
