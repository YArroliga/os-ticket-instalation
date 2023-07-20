# os-ticket-instalation
Installing Os ticket in an Azure VM
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine
- Remote Desktop
- Internet Information Services (IIS)
- PhP manager for IIS

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a Virtual Machine on Azure 
- Install ISS and PHP manager 
- Install OsTicket

<h2>Installation Steps</h2>

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/8c09594e-1e34-4de8-855b-960e637e75c5) 

<p>
On Azure, open a Virtual Machine using Windows 10 as an operating system
<br />

  ![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/de3e2ae9-52fc-4bf1-a81f-64bbcef4981d)


Open Remote Desktop and remote into the VM
<p>
  
![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/a7a6c91e-c10f-4a84-9e84-c90e9f0b1519) 

In windows under Programs > Turn Windows features on or off > Install ISS

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/7989b573-272a-4571-bb9a-7dfee70950c8)

Install PhP manager for ISS 

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/94204e00-c99a-4342-a660-9e3fc5287e51)

Download PhP, in this case it came in a compressed file that was extracted to a premade folder in the C drive.
</p>
<p>

<br /> ![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/66991048-ed34-4c1d-a933-3846438e49a4)

Open IIS as an administrator by right clicking from the Start menu.

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/83438101-cd1a-47af-be27-096dbc84b024)

In IIS open PhP manager and register the new PhP version that was installed in the premade folder

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/af6a9c04-efe6-4570-a5e8-4a56f4a25667)

Install MySQL

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/66806daa-58be-4ae7-adf4-2720e2716364)

MySQL sets up a Password that gets used later during OsTicket installation  


<p>

  ![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/af7ba319-9926-43fa-8991-47d6179ebd28)

Restart the server

  ![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/a512908b-92f7-4aa1-9a1a-8f157f4791df)

Download OsTicket and in the downloads folder open the OsTicket folder to drag the uploads folder into  Windows C: > inetpub > wwwroot folder, then rename the uploads folder to OsTicket

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/7391ce37-f8bf-4537-ba3e-308356497c8a)

OsTicket is installed but it's not fully functioning. We still need to enable some protocols. 

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/72f8d8f5-a1e0-472a-a615-baba3e4ff917)


In IIS under PHP manager > Enable or disable an extension 
Enable: PHP IMAP Extension and Intl Extension

![image](https://github.com/YArroliga/os-ticket-instalation/assets/139689160/a8e7941a-0d02-42dd-8fa8-fbac14a694b8)

Finish the installation process of the program by filling out the information 


</p>
<br />
