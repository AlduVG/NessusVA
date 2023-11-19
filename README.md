# NessusVA
## Introduction.
A vulnerability assessment is the process of identifying, quantifying, and prioritizing vulnerabilities within an information system. This process helps by bringing awareness to the security posture of an organization to remediate these weaknesses before a threat can take advantage.

## Prerequisites.
For this project, I'll be using the following:

- Oracle's VirtualBox.

- A virtualized Windows 10 OS.

- Tenable's Nessus Essentials.


For the sake of simplicity, I'll be skipping the process of downloading Nessus and creating the Virtual Machine.

## Windows VM setup.

![SettingUpdateSecurity-1](https://github.com/AlduVG/NessusVA/assets/131760637/ac3870f0-841e-46d5-bb5a-a7a79e6d25e3)
![AdvancedOptions-2](https://github.com/AlduVG/NessusVA/assets/131760637/2be7a56d-1d17-469d-96a1-80fb55ab86fd)
![PausingForDays-3](https://github.com/AlduVG/NessusVA/assets/131760637/e4363744-63dd-45f6-9a64-aca3f114d52a)
![ViewUpdateHistory-4](https://github.com/AlduVG/NessusVA/assets/131760637/15475fe6-b321-4ea6-a35f-7a3a5982270c)
![UninstallingSecUodates 5](https://github.com/AlduVG/NessusVA/assets/131760637/ac0d6147-9c15-477e-b403-3394aa6bc0cf)
![WindowsDefenderOff 6](https://github.com/AlduVG/NessusVA/assets/131760637/2300848e-630b-4c2a-8a2b-961e6c8dce69)
![HostOnlyAdapater 7](https://github.com/AlduVG/NessusVA/assets/131760637/acf8725a-415a-4f47-a324-a0b1b81c05d4)
![Services 8](https://github.com/AlduVG/NessusVA/assets/131760637/e3168993-b133-4e85-a921-709e5e5b9696)
![UserAccountcontrol 9](https://github.com/AlduVG/NessusVA/assets/131760637/287a05f5-8346-467a-8042-43f97f08fc10)
![RegistryEditor 10](https://github.com/AlduVG/NessusVA/assets/131760637/d0e21c23-5412-4c90-bf1f-5acef69097bf)
![RegistryEditorDWORD 11](https://github.com/AlduVG/NessusVA/assets/131760637/7214c926-4f14-4f6b-9e0d-f667802bcbd5)
![NessusScan 11](https://github.com/AlduVG/NessusVA/assets/131760637/260d6da6-16c9-456e-bb23-83fc34fd0803)
![NessusReport 12](https://github.com/AlduVG/NessusVA/assets/131760637/64324f1e-492f-46d1-a2f8-0455f1f08dfe)

## Vulnerabilities remediation.
Nessus also provides us with the options to remediate these vulnerabilities. In the scan we performed, there are 8 critical vulnerabilities to address.

![VARemediation-final](https://github.com/AlduVG/NessusVA/assets/131760637/1eabfa01-4ce6-46fc-8abd-a0e78c39d597)

### Upgrading Google Chrome.
In Google Chrome, we go to settings, select 'Help,' and choose 'About Google Chrome.' 

![GoogleChromeUpdate-2](https://github.com/AlduVG/NessusVA/assets/131760637/08a605ca-55bd-4ee5-ab0a-bb2aef91436a)

Next, we can update the browser to address the vulnerability found. It's also a good idea to keep Google updated as soon as an update is released to prevent future vulnerabilities.

![GoogleChromeUpdate](https://github.com/AlduVG/NessusVA/assets/131760637/46e25b83-a8fd-45a8-986f-f4bc8a913010)

### Upgrading Mozilla Firefox.

Remediating the vulnerability in Mozilla will be very similar to that in Google Chrome. For this, we go to the Mozilla options menu and select 'About Mozilla'.

![MozillaUpdate 24](https://github.com/AlduVG/NessusVA/assets/131760637/cb4946ca-3735-4039-a112-31d5c1d2b724)

The browser will update to the latest version.

![MozillaUpdate 25](https://github.com/AlduVG/NessusVA/assets/131760637/634835f7-8a7f-40d4-95f8-9cdee8f70945)

### Installing KB5031356.
To address the vulnerability related to KB5031356, we need to undo the changes we made earlier regarding uninstalling security updates in Windows. 

![NoWindowsUpdate 17](https://github.com/AlduVG/NessusVA/assets/131760637/c48159fc-8fd0-4108-a356-76744c6b9608)

![VAWindowsUpdate 18](https://github.com/AlduVG/NessusVA/assets/131760637/186900c6-6b33-4958-bd4b-7bbe55d4c728)

For this, we go to 'Settings,' resume system updates, and check for available updates to install. 

![InstallingKB5007186 14](https://github.com/AlduVG/NessusVA/assets/131760637/679c63b1-ae7b-4b5f-8cd2-c716aebd9a39)
![InstallingKB5007186 15](https://github.com/AlduVG/NessusVA/assets/131760637/f4008d3c-3e7c-44d5-962b-7cb64e2ec72b)

In my case, I had to install updates and restart several times until eventually there were no more updates to install.
![InstallingKB5007186 16](https://github.com/AlduVG/NessusVA/assets/131760637/19e1c3df-71dd-4f19-94da-c26c51a8adbe)


### Removing Log4j vulneravility.

To address the vulnerability related to Log4J, we simply need to delete all information related to the Minecraft server that we downloaded previously. It is necessary to empty the recycle bin so that we can mitigate this vulnerability.

![DeletingLog4jVul 13](https://github.com/AlduVG/NessusVA/assets/131760637/61720baa-f899-4d21-9c80-4f83337d8bd3)

### Upgrading 7-Zip, Snip & Sketch and Microsoft 3D.

To address the vulnerabilities related to 7-Zip, Snip & Sketch, and Microsoft 3D, we simply need to download the latest version of these software programs.

### Upgrading CURL to version 8.4.0.
To update the CURL vulnerability, follow these steps:

Verify your current CURL version by entering the following commands in CMD:

> curl --version

![CurlUpdate-20](https://github.com/AlduVG/NessusVA/assets/131760637/de53b671-7684-4e85-ad64-75315305f4c5)

> where curl

This ensures accurate identification of the existing version that requires updating. The "where" commands will indicate the location of the "curl.exe" file, usually is C:\Windows\System32\curl.exe.

Download the updated binaries from the official CURL website:
https://curl.se/windows/

After downloading, replace the existing "curl.exe" file in the system32 directory with the newly downloaded one. To do this, you first need to remove the outdated "curl.exe" file. Begin by claiming full ownership of the file (administrator privileges are required) and then proceed with the replacement. The steps are as follows: Right-click, select properties, navigate to security, go to advanced, and change the owner.

Execute another curl --version command to confirm that the updated version of CURL is now in place.

![CURLUPDATED](https://github.com/AlduVG/NessusVA/assets/131760637/65c29279-acd4-49f2-bee0-ce5ed5f25887)










