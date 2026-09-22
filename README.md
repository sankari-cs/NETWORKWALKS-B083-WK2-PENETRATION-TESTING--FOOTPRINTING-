# NETWORKWALKS-B083-WK2-PENETRATION-TESTING--FOOTPRINTING-
````markdown
# 🔎 Networkwalks — Week 2
## Footprinting & Reconnaissance

> **Cybersecurity Internship | Practical Security Assessment**

---

## 📖 About This Week

As part of my **Networkwalks Cybersecurity Internship**, Week 2 focused on the initial information-gathering stage of a security assessment.

The practical work involved studying an authorized web target and collecting publicly observable information related to its **domain, DNS configuration, web technologies, HTTP behavior, and security controls**.

This exercise helped me understand how reconnaissance builds a technical picture of a target before deeper security testing.

---

## 🎯 What I Practiced

- Understanding the role of reconnaissance in penetration testing
- Gathering publicly available information about an authorized target
- Examining domain and DNS information
- Identifying technologies used by a web application
- Reviewing HTTP response information
- Checking for the presence of web application security controls
- Recording technical observations with supporting evidence
- Following responsible and authorized security-testing practices

---

## 🧰 Reconnaissance Toolkit

| Tool | Purpose |
|---|---|
| **WHOIS** | Examine publicly available domain registration information |
| **WhatWeb** | Fingerprint technologies used by a website |
| **Nslookup** | Query DNS information and resolve domain details |
| **cURL** | Inspect HTTP responses and headers |
| **Wafw00f** | Check for detectable Web Application Firewall technologies |
| **DNSRecon** | Gather DNS-related information |
| **Wappalyzer** | Identify web technologies through browser-based analysis |

---

## 🧭 Reconnaissance Workflow

```text
                 Authorized Target
                        │
                        ▼
                Domain Information
                        │
                        ▼
                  DNS Enumeration
                        │
                        ▼
             Technology Identification
                        │
                        ▼
               HTTP Header Review
                        │
                        ▼
                 WAF Detection
                        │
                        ▼
              Evidence & Observation
````

The purpose was to understand what information could be identified **without moving into exploitation**.

---

# 🔬 Practical Work

## 01 — Domain Intelligence

The first stage involved examining publicly available information associated with the target domain.

**Tool:** `WHOIS`

### Focus

* Domain registration information
* Domain-related metadata
* Publicly available registration details

### Evidence

Add your screenshot here:

```text
screenshots/
└── whois.png
```

---

## 02 — Web Technology Fingerprinting

I used **WhatWeb** to identify technologies that could be detected from the target web application.

**Tool:** `WhatWeb`

### Focus

* Web server information
* Frameworks and technologies
* Technology fingerprints exposed by the application

### Evidence

```text
screenshots/
└── whatweb.png
```

---

## 03 — DNS Investigation

DNS information was examined to understand how the authorized domain resolves within the DNS infrastructure.

**Tool:** `nslookup`

### Focus

* Domain resolution
* IP information
* DNS responses

### Evidence

```text
screenshots/
└── nslookup.png
```

---

## 04 — HTTP Response Analysis

I used **cURL** to inspect the HTTP response returned by the web server.

**Tool:** `cURL`

### Focus

* HTTP status information
* Response headers
* Server-side information exposed through HTTP

### Evidence

```text
screenshots/
└── curl.png
```

---

## 05 — WAF Identification

The target was checked using **Wafw00f** to determine whether a detectable Web Application Firewall was present.

**Tool:** `Wafw00f`

### Purpose

Understanding defensive technologies visible during reconnaissance can provide useful context for later authorized security testing.

### Evidence

```text
screenshots/
└── wafw00f.png
```

---

## 06 — DNS Enumeration

I performed additional DNS reconnaissance using **DNSRecon**.

**Tool:** `DNSRecon`

### Focus

* DNS records
* DNS infrastructure information
* Additional publicly observable DNS details

### Evidence

```text
screenshots/
└── dnsrecon.png
```

---

## 07 — Browser-Based Technology Analysis

I also used the **Wappalyzer** browser extension to identify technologies detected from the web application through browser-based analysis.

### Why Use It?

Using both command-line and browser-based tools provides different perspectives during reconnaissance and helps compare technology fingerprints.

### Evidence

```text
screenshots/
└── wappalyzer.png
```

---

# 📊 Observation Summary

| Area       | Technique  | Security Context                   |
| ---------- | ---------- | ---------------------------------- |
| Domain     | WHOIS      | Public domain intelligence         |
| Technology | WhatWeb    | Web technology fingerprinting      |
| DNS        | Nslookup   | Domain and IP resolution           |
| HTTP       | cURL       | Response/header analysis           |
| Protection | Wafw00f    | WAF identification                 |
| DNS        | DNSRecon   | DNS infrastructure enumeration     |
| Web Stack  | Wappalyzer | Browser-based technology detection |

> **Important:** Reconnaissance observations should not automatically be treated as vulnerabilities. Additional authorized validation is required before classifying an observation as a security issue.

---

# 🛡️ Security Perspective

This exercise demonstrated that information exposed through normal public interfaces can contribute to an external view of an organization's technology environment.

From a defensive perspective, organizations should regularly review:

* Publicly exposed technology information
* DNS records
* HTTP response headers
* Web server configuration
* Security-control exposure
* Unnecessary infrastructure information

Reducing unnecessary information disclosure can make reconnaissance less informative to unauthorized parties.

---

# 🧠 Key Takeaways

Through this week's practical work, I gained hands-on experience with:

* The reconnaissance stage of penetration testing
* Domain and DNS investigation
* Web technology fingerprinting
* HTTP response inspection
* WAF detection
* DNS enumeration
* Browser-based technology discovery
* Evidence collection and technical documentation
* Responsible security assessment practices

The main takeaway was understanding that **reconnaissance is the foundation for a structured security assessment** because it helps establish the technical scope and attack surface before further testing.

---

# ⚠️ Responsible Security Testing

All activities documented in this repository are intended for **educational and authorized cybersecurity testing**.

Reconnaissance and security-testing techniques should only be performed against:

* Systems you own
* Lab environments
* CTF platforms
* Targets for which explicit authorization has been provided

Unauthorized scanning, enumeration, or testing may violate applicable laws, policies, or terms of service.

---

# 👩‍💻 About Me

**Sankari A.**

Cybersecurity Student | Python | Flask | OWASP | Web Application Security

🔗 GitHub: [sankari-cs](https://github.com/sankari-cs)

🔗 LinkedIn: [Sankari](https://www.linkedin.com/in/sankaria1)

---

## 📌 Internship Learning Series

**Program:** Networkwalks Cybersecurity Internship
**Week:** 02
**Focus:** Footprinting & Reconnaissance

This repository documents my practical learning and hands-on cybersecurity activities during the internship.

````

### How to use it

In your `sankari-A` repository:

1. Open **Add file → Create new file**
2. Name it:
   ```text
   README.md
````

3. Paste the entire code above.
4. Click **Commit changes**.
5. Later, create a folder:

   ```text
   screenshots
   ```
6. Upload your actual screenshots there.
7. Change the screenshot filenames in the README if your files have different names.

For example, once you upload `whois.png`, you can replace the placeholder with:

```markdown
![WHOIS Analysis](screenshots/whois.png)
```

That will make the screenshots **actually appear inside your GitHub README** rather than just showing the filename.
