# Home-Lab-Attack-And-Defense

since i am on macOS i prefer to use UTM instead of VBox. using UTM, i download isos for windows 11 and ubuntu and set up 2 vms 
<img width="1280" height="832" alt="image" src="https://github.com/user-attachments/assets/1d5907b6-edab-455c-9d82-d19bbc71a632" />
then you go ahead and remove security features from windows 11 so we can attack it from ubuntu
<img width="1280" height="832" alt="image" src="https://github.com/user-attachments/assets/122b65e7-25c1-44b4-a28b-aea9dfe06d45" />

so we have:

UTM — I created two VMs on a lab 

Ubuntu (attacker) — I installed Metasploit and used it to run an exploit handler and host test files (HTTP) that the victim downloads.

Windows (victim) — I installed Sysmon to collect detailed Windows telemetry (process starts, network connects, file creations) and I executed the test file 
there to generate events.

Splunk (the SIEM) — I ran Splunk as my central collector and search interface.

I configured the Windows machine to send Sysmon events to Splunk, then used Splunk searches/dashboards to view process creation, outbound connections, and file‑write activity.


Metasploit — I used it on Ubuntu to produce the test payload (lab only) and to receive the reverse session when the payload ran on the Windows VM.

Tuning Sysmon

Sysmon is highly configurable. The key to effective detection is tuning Sysmon to log the right kinds of events. You can customize what Sysmon records through its configuration file

