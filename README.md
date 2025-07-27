# Cybersecurity-Portfolio
Welcome to my cybersecurity portfolio! I'm a student at Montgomery College passionate about cloud security, penetration testing, and defensive operations.

Burp Suite Web Application Security Lab

Overview

This repository lab takes my hands-on work with Burp Suite, focusing on identifying and exploiting common web application vulnerabilities. Scenarios based on real-world activity are what this structured lab was designed to show. in which case, I searched for traffic patterns, exploited inputs, and examined application behavior to uncover weaknesses, including Reflected XSS, SQL Injection, and insecure session magament.
This project highlights both the offensive techniques used to uncover flaws and the defensive strategies developers can adopt. It mirrors a growing sense of proficiency in web application security and commitment to ethical hacking.


🛠️ Tools & Environment

Burp Suite Community Edition
Firefox browser with Burp proxy configured
PortSwigger's intentionally vulnerable labs
Kali Linux as the testing environment

 
 Objectives
 
Configure the browser and proxy to route traffic through Burp Suite

Set up both the browser and Burp Suite so that all web traffic passes through the proxy for inspection.
Observe and analyze HTTP and HTTPS requests and responses during web app interactions.
Noted what happened after successful exploits to better understand the kind of risks they pose to users and systems.
Took screenshots along the way and wrote up short summaries to explain what each finding meant and why it mattered.


Key Findings

VulnerabilityDetailsImpactRecommendation

Reflected XSS	JavaScript executed via unsanitized query string input	Can hijack sessions or deface content	Validate and encode all user input
SQL Injection	Raw user input passed directly into SQL queries	Access or alter sensitive database content	Use prepared statements and ORM practices
Insecure Cookies	Session cookies lacked HttpOnly or Secure flags	Susceptible to theft or tampering	Enable proper cookie attributes
Information Disclosure	Detailed errors revealed server-side technologies	Aids attackers in reconnaissance	Display generic error messages

 What I Learned
 
Effective Burp Suite setup and integration with the browser
Deconstructing and altering HTTP traffic manually
Payload crafting for different vulnerability types
Practical application of security testing concepts
Importance of layered defenses and secure defaults

Repo Contents

BurpSuite-LabReport.pdf: Complete write-up of vulnerabilities and findings

Screenshots showing intercepted traffic and payload outcomes

Notes, payload samples, and reflections

Re-doing the Lab 

To follow along or reproduce:

Install Burp Suite Community Edition
Configure the browser proxy to 127.0.0.1:8080
Use PortSwigger Labs or DVWA
Follow the test methodology: intercept → modify → observe

💡 Final Reflection

This lab opened my eyes to how I understand web app flaws and how attackers exploit them. Looking at each finding, we see how even minor oversights can compromise an entire system. More importantly, I saw how Burp Suite enables both discovery and analysis in a structured and repeatable manner.
"Security is about mindset, not just tools." — This experience helped me think like an attacker to build better and defend secure applications.

