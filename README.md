# Azure-Network-Protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Configure Group Policy to Lockout the account after 3 attempts
- Unlock users account
- Step 3
- Step 4

<h2>Actions and Observations</h2>

<p>
<img width="380" height="307" alt="image" src="https://github.com/user-attachments/assets/016cba1f-dc8a-4829-9e7b-99b1f5bf85df" /> <img width="791" height="172" alt="image" src="https://github.com/user-attachments/assets/14dd9c4f-5ead-4d86-8d64-71afe1c7e7a8" />
<img width="787" height="185" alt="image" src="https://github.com/user-attachments/assets/0f22b031-f0bd-4983-a0a2-e4256eb75547" />

</p>
<p>
By configuring the Account Lockout Policy in Group Policy, you limit the number of failed login attempts before an account locks. This protects against brute force attacks and strengthens domain security. For example, setting a threshold of 3 failed attempts with a 30-minute lockout duration helps balance usability with protection.
</p>
<br />

<p>
<img width="404" height="561" alt="image" src="https://github.com/user-attachments/assets/3018f50a-173b-4762-8ed5-33e2364f5cb8" />

</p>
<p>
Unlocking a user account is a simple but essential admin task in Active Directory. It restores access when someone is locked out after too many failed login attempts. This can be done through the ADUC console (GUI) or with a PowerShell command. Admins should also review the cause of frequent lockouts to prevent future disruptions or detect potential security risks.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
