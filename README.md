# Configure-Group-Policy
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Configuring Active Directory Group Policies and Managing Accounts</h1>
In this tutorial, we explore how Group Policy is used to manage user and computer accounts within an Active Directory domain. We configure password policies, account lockout thresholds, and login restrictions to strengthen domain security. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 11 Pro (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Configure Group Policy to set wallpaper and Power options
- Configure Group Policy to Lockouts account after 3 attempts
- Unlock users account

<h2>Actions and Observations</h2>

<p>
<img width="300" height="333" alt="image" src="https://github.com/user-attachments/assets/16fea6c3-3133-479b-bf0a-7b3b94f7c68c" /> 
<img width="427" height="222" alt="image" src="https://github.com/user-attachments/assets/c2dc3f46-b990-4be5-8ad5-8f36a850a7a9" /> <img width="341" height="271" alt="image" src="https://github.com/user-attachments/assets/05450785-6132-463b-87bc-6f38584e69d8" />
<img width="392" height="236" alt="image" src="https://github.com/user-attachments/assets/7a10259d-45f5-4caa-85ba-73d8941b7383" /> <img width="231" height="447" alt="image" src="https://github.com/user-attachments/assets/1aa4ca81-8fb4-40ae-a3b9-1210bdda4fa4" />
<img width="386" height="176" alt="image" src="https://github.com/user-attachments/assets/8c83b8e9-2214-4f50-a925-dc09bca6dc30" /> <img width="533" height="351" alt="image" src="https://github.com/user-attachments/assets/f6b57981-9c8b-4cb2-8a89-b5a5541ab30e" />

</p>
<p>
Using Group Policy, you can enforce a desktop wallpaper across all domain-joined computers (or a specific group). Instead of users choosing their own background, the system applies the wallpaper you configure or power options oue create.
</p>
<br />

<p>
<img width="380" height="307" alt="image" src="https://github.com/user-attachments/assets/016cba1f-dc8a-4829-9e7b-99b1f5bf85df" /> <img width="791" height="172" alt="image" src="https://github.com/user-attachments/assets/14dd9c4f-5ead-4d86-8d64-71afe1c7e7a8" />
<img width="787" height="185" alt="image" src="https://github.com/user-attachments/assets/0f22b031-f0bd-4983-a0a2-e4256eb75547" />

</p>
<p>
By configuring the Account Lockout Policy in Group Policy, you limit the number of failed login attempts before an account locks. This protects against brute force attacks and strengthens domain security. For example, setting a threshold of 3 failed attempts with a 30-minute lockout duration helps balance usability with protection.
</p>
<br />

<p><img width="401" height="557" alt="image" src="https://github.com/user-attachments/assets/fbacb073-f54d-4091-8ea2-c3b838452e1b" />


</p>
<p>
Unlocking a user account is a simple but essential admin task in Active Directory. It restores access when someone is locked out after too many failed login attempts. This can be done through the ADUC console (GUI) or with a PowerShell command. Admins should also review the cause of frequent lockouts to prevent future disruptions or detect potential security risks.
</p>
<br />


