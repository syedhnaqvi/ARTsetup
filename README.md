# # Atomic Red Team Installation & Setup 
<img src="https://img.shields.io/badge/-Atomic%20Red%20Team-blue?style=for-the-badge"></img><br>
<div style="text-align:center;">    
  <img src="https://camo.githubusercontent.com/0ed20b85516f7c35f6a1c48ba69ec3803b32a8a936fd3c9c6bfb04a8311d4839/68747470733a2f2f72656463616e6172792e636f6d2f77702d636f6e74656e742f75706c6f6164732f41746f6d69632d5265642d5465616d2d4c6f676f2e706e67" width=300 height=200></img>
</div>

## Objective
The step by step guidance on how to setup Atomic Red Team for generating telemetry data and see detctions in Splunk  .

### What is Atomic Red Team
Atomic Red Team is a library of tests that every security team can execute to simulate adversarial activity and validate their defenses. Tests are focused, have few dependencies, and are defined in a structured format that can be used by automation frameworks.

### Skills Learned

- ART installtion
- POwershell


### Tools Used

-Atomic Red Taam 

### Step -1 Windows 10 VM
Open Powershell with Amdin Privileges
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/6e26c209-a3de-406e-8ad1-3e37b2fb60f6)

### Step -2 
Logon using Administrative account
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/c0d5f8ad-f2d7-4f5d-b3bd-ef8ca84e5cab)

### Step -3
Run command in Powershell console 
The Bypass policy allows us to run scripts from anywhere, and will execute the scripts without warning regardless of the source Select Y then Enter.

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/2710f52b-5d1b-4b81-bdb0-f251d29f5501)

### Step -4 
Create exclusion for entire C drive as defedner will detect and remove installation!
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/7e0d5a0a-a8d0-4998-b790-65f899314b08)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/9593c5a8-4818-4ff8-8b52-f251269442dc)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/9554cae0-c63f-4f4b-972f-493982472662)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/b8eb5abb-8b90-4b04-828c-d632328d7adc)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/fbdac193-ad3e-4ccf-b614-11a7e27b1b40)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/565ef8e8-3d27-42cd-a49c-723cef1c330f)

### Step -5
Install Atomic Red Team using powershell IEX
IEX (IWR 'https://raw.githubusercontent.com/redcanaryco/invoke-atomicredteam/master/install-atomicredteam.ps1');Install-AtomicRedTeam.<br>
<a href="[https://github.com/redcanaryco/invoke-atomicredteam/wiki/Installing-Atomic-Red-Team/f70bafb8afd571ae91a01bc7b974cf2a3a4dc93e](https://github.com/redcanaryco/invoke-atomicredteam/wiki/Installing-Invoke-AtomicRedTeam)https://github.com/redcanaryco/invoke-atomicredteam/wiki/Installing-Invoke-AtomicRedTeam">Installing Red Team</a>

Once installed then go got C: drive then go to Atomic red Team folder.
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/f828c8a0-0286-496c-9622-5119e066232b)
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/ae1899f4-61c4-4970-acf0-210e6c4c3ae8)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/b7d7bdf4-c777-49e3-bbfe-11f20ea29629)

Run this before using Invoke-AtomicTest command.
Import-Module "C:\AtomicRedTeam\invoke-atomicredteam\Invoke-AtomicRedTeam.psd1" -Force

Run specific MItre Mapped speciifc test from AtomicRed .
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/82e7334c-f0da-4c10-88d4-e970137c3825)

![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/1461a854-725c-47dc-bd20-a4d5d3202311)


Go to Splunk and search 
![image](https://github.com/syedhnaqvi/ARTsetup/assets/39069507/a0dd1005-9b18-41fd-a20f-7494bdf8d6f6)


