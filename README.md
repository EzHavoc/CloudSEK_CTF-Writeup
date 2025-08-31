Got it ✅ — right now your README is solid in content but the **routing/structure/navigation** can definitely be improved for readability and quick access.
I’ll reorganize it with a **cleaner flow, clickable links, consistent headings, and better visual hierarchy**.

Here’s an updated version:

---

# 🕵️ CloudSEK Hiring CTF — Writeup

Hello! I’m **ZestyPesky** and this repository contains my detailed write-up for the **CloudSEK Hiring CTF**.

I managed to solve **4 out of 5 flags during the event** and later cracked the **final challenge (Flag 5)** after the CTF ended.
This repo documents my **approach, methodology, and key learnings** from each stage.

---

## 📚 Navigation

* [🔎 Overview](#-overview)
* [🚩 Challenges](#-challenges)

  * [Flag 1 — Welcome Challenge](#flag-1--welcome-challenge)
  * [Flag 2 — Hacking the Hacker](#flag-2--hacking-the-hacker)
  * [Flag 3 — Attacking the Infrastructure](#flag-3--attacking-the-infrastructure)
  * [Flag 4 — Bypassing Authentication](#flag-4--bypassing-authentication)
  * [Flag 5 — The Final Game](#flag-5--the-final-game)
* [📌 Key Takeaways](#-key-takeaways)
* [⚠️ Disclaimer](#-disclaimer)

---

## 🔎 Overview

The **CloudSEK Hiring CTF** tested a wide spectrum of skills — from **OSINT, prompt injection, and reverse engineering** to **GraphQL exploitation, authentication bypass, and AWS SSRF attacks**.

It was a mix of real-world security scenarios and fun puzzles that tested both **technical depth** and **time management**.

---

## 🚩 Challenges

### Flag 1 — Welcome Challenge

* OSINT using an email address.
* Commit history analysis in GitHub.
* Extracted the **first flag** hidden in an older commit.

---

### Flag 2 — Hacking the Hacker

* Reverse-engineered a Telegram bot.
* Used **prompt injection** to bypass restrictions.
* Analyzed an audio file (Morse code) → **second flag obtained**.

---

### Flag 3 — Attacking the Infrastructure

* Decompiled the **CloudSEK BeVigil APK**.
* Found a **hardcoded GraphQL endpoint**.
* Performed introspection → privilege escalation via **JWT forgery**.

---

### Flag 4 — Bypassing Authentication

* Leveraged GraphQL creds from previous step.
* Found **hardcoded API keys** enabling MFA/backup code bypass.
* Analyzed session cookies → generated **admin backup codes**.

---

### Flag 5 — The Final Game *(post-CTF solve)*

* Found **SSRF** in profile picture upload API.
* Exploited AWS metadata service → obtained IAM creds.
* Queried S3 bucket to extract the **final flag**.

---

## 📌 Key Takeaways

* 🔍 **OSINT can snowball** into bigger breakthroughs.
* 🤖 **Prompt injection** is a rising concern in chatbot security.
* 📊 **GraphQL misconfigs** often expose more than intended.
* 🔑 **Hardcoded secrets** = disaster waiting to happen.
* ☁️ **SSRF in cloud environments** can escalate into **full account compromise**.

---

## ⚠️ Disclaimer

This write-up is for **educational purposes only**.
All vulnerabilities described exist **only in the CloudSEK Hiring CTF environment**, not in production systems.

---