# Home Lab

## Overview
This is my personal IT and security homelab where I practice setting up systems, testing different scenarios, and understanding how Windows and Linux behave in a small network.

I started using VirtualBox but later switched to UTM since I’m on macOS and it fits my setup better.

The goal is to learn how systems work in practice, how logs are created, and how IT teams investigate issues.

---

## Setup

I currently run two virtual machines using UTM:

- Windows 11 (main Windows system for testing)
- Ubuntu (used for testing tools and generating activity)

Both machines are connected in a simple lab network so they can interact with each other.

<img width="1280" height="832" alt="Screenshot 2025-09-24 at 1 09 36 PM" src="https://github.com/user-attachments/assets/c5e58224-6653-44f6-9ab0-efa391881d39" />

---

## What I’ve built so far

- Built and maintained a small IT/security homelab using virtual machines on macOS  
- Set up different test scenarios to understand system behaviour in normal and controlled testing situations  
- Practised basic IT support and troubleshooting across Windows and Linux systems  
- Previously worked with Active Directory in earlier lab setups  
- Set up logging and monitoring tools to observe system activity  

---

## Active Directory (earlier lab work)

In an earlier setup, I used Active Directory to practise basic IT support tasks.

This included:
- Creating and managing user accounts  
- Resetting passwords  
- Organising users into groups  
- Applying basic Group Policy settings  

<img width="969" height="702" alt="Screenshot 2025-10-16" src="https://github.com/user-attachments/assets/6f8b5031-38d9-4d31-9f28-b32f01a414b1" />

---

## Attack & Defence Practice (lab environment)

### Ubuntu system
On Ubuntu, I installed tools like Metasploit and used them in a controlled lab environment for learning.

I used it to:
- Run test payloads in a safe environment  
- Host simple files over HTTP for testing  
- Simulate basic attacker-style activity for learning how systems respond  

---

### Windows system
On Windows, I set up logging so I could see what happens inside the system during different actions.

I installed Sysmon, which records things like:
- Which programs are running  
- Network connections being made  
- Files being created or changed  

This helped me understand how normal system activity and unusual activity appear in logs.

## Splunk (log analysis)

I used Splunk as a central place to collect logs from the Windows system.

Once set up, I could:
- Search through system activity  
- Track running processes  
- View network connections  
- Review file activity in one place  

This helped me connect actions in the system with what appears in logs.

## What I learned

- How Windows and Linux behave in a small network setup  
- How Active Directory is used in IT support environments  
- How system logs are generated and used for troubleshooting  
- How tools like Splunk are used to analyse system activity  
- How to investigate issues step by step using logs and system output  
