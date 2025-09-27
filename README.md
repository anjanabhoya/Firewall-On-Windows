# Task 4: Firewall Configuration on Windows

[cite_start]This repository documents the completion of Task 4 for the Elevate Labs Cybersecurity Internship[cite: 1]. [cite_start]The objective was to configure and test a basic firewall rule to block network traffic on a Windows system[cite: 1].

[cite_start]**Tool Used:** Windows Defender Firewall with Advanced Security [cite: 2]

---

## Steps Performed

[cite_start]The following steps were taken to configure, test, and document the firewall rule[cite: 3]:

1.  **Opened Firewall Tool:** Launched "Windows Defender Firewall with Advanced Security" to access the firewall settings.
2.  **Navigated to Inbound Rules:** Selected "Inbound Rules" from the left panel to view all current rules for incoming traffic.
3.  [cite_start]**Created a New Rule:** Initiated the "New Inbound Rule Wizard" to add a rule for blocking a specific port[cite: 4].
4.  **Configured the Rule:** The rule was configured with the following specifications:
    * **Rule Type:** Port
    * **Protocol:** TCP
    * [cite_start]**Specific Port:** 23 (Telnet) [cite: 4]
    * **Action:** Block the connection
    * **Profile:** Applied to all profiles (Domain, Private, and Public)
5.  **Named and Saved:** The rule was named `block telnet(port 23)` and saved, making it active.
6.  [cite_start]**Documented the Rule:** A screenshot was taken of the active rule in the "Inbound Rules" list to serve as the deliverable[cite: 3].
7.  [cite_start]**Restored Original State:** The test rule was deleted to clean up the configuration and restore the system to its previous state[cite: 7].

---

## Deliverable: Screenshot

[cite_start]The screenshot below shows the successfully created inbound rule blocking all traffic on TCP Port 23, as seen in the Windows Defender Firewall console[cite: 3].

*Replace the line below with your actual screenshot.*
`![Firewall Rule Screenshot](screenshot.png)`

---

## Summary: How a Firewall Filters Traffic

[cite_start]A firewall filters network traffic by inspecting data packets and checking them against a predefined set of security rules[cite: 8]. Based on these rules, the firewall either allows the packet to pass through or blocks it.

In this task, the firewall was configured to filter traffic based on:
* **Direction:** The rule was an **inbound** rule, meaning it only applied to traffic coming *into* the computer.
* **Port Number:** It specifically targeted traffic destined for **Port 23**.
* **Protocol:** The rule was set for the **TCP** protocol.

[cite_start]By enforcing these rules, the firewall acts as a critical barrier, preventing unauthorized access and enhancing the overall security of the system[cite: 11].
