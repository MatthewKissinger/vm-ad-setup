<p align="center">
  <img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Microsoft Azure Tutorial</h1>
<h2>Creating a Domain Controller and Client Virtual Machines for Active Directory Deployment</h2>
<p>This tutorial outlines the prerequisites and the creation of a Domain Controller and Client Virtual Machines in the cloud computing platform Microsoft Azure.</p> 
<p>We will first create a Domain Controller VM (named DC-1) with the windows server OS, then create a Client VM (named Client-1).</p>  
Once both Virtual Machines are up and running we will ensure that they are connected via ICMPv4. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- ICMPv4
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10
- Windows Server 2022

<h2>List of Prerequisites</h2>

- Microsoft Azure Account (Free version of $200 credits available)
- Personal Computer running Windows 10 or 11
- Basic understanding of ping command
- Basic understanding of Windows File Explorer
  
<h2>Create the Domain Controller Virtual Machine</h2>

<p>1) From the Microsoft Azure Homepage click on the Virtual Machines Icon [See Below]</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/baddce6d-515a-45d2-88ee-490466fd3a6a)

<p>2) Now that you're in the Virtual Machines Section Click on the Create Button [See Below]</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/d50995ee-a7e0-4ed7-8959-f6012e3599da)

<p> And select Azure Virtual Machine</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/3ec70234-22ae-4da4-99ca-5f9ce4c595f4)

<p>3) Have the Resource Group auto-created by the form</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/04eec0c7-329a-491a-a110-0338cf9f84da)

<p>4) Name the virtual machine DC-1 (for Domain Controller 1) and select a region near you (ex: US West 2)</p>

<p>For Image select Windows Server 2022</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/769f35b8-fdbf-461e-ac89-e1a74a714826)

<p>For Size, select at least 2vcpu. Going over this may be costly, especially if you are using the free $200 credits for learning purposes. Example below: ** You may need to look at all sizes and filter and then go back to the creation screen if using a free account **</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/622c818e-1b21-412a-bce4-4abe57dc379e)

<p>5) Set up a username and password and WRITE THIS INFO DOWN!  It will be needed to access the virtual machine via Remote Desktop Connection in the next Tutorial. </p>

<p>Also, write down the Resource Group and Vnet (Virtual Network) that were created for DC-1 </p>

<p>5) Set the Domain Controller's NIC (Network Interface Card) Private IP Address to static</p>

<p>Navigate to the Virtual Machines page by clicing on the VM icon again. </p>

<p>From here click on DC-1 </p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/d5e72456-2784-4d92-aa4e-1752a4427029)

<p>then, Network Settings under the Networking dropdown menu</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/0354a965-06c6-43a3-b055-44ba4c1aafe2)

<p>then, click on the Network interface / IP configuraion card (your NIC name may be different)</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/69e1abf8-b2a1-4ca7-966d-7f8f4e5beb59)

<p>In Ip configurations</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/803936c3-52c3-4508-8708-dd48f60a8757)

<p>click on the name ipconfig 1</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/d4f063b8-dc3a-4796-a245-ea82a7b81a8d)

<p>Change the Private IP address settings Allocation from Dynamic to Static</p>

![image](https://github.com/MatthewKissinger/vm-ad-setup/assets/48774883/fe50b8d3-d3f2-43d5-8fcf-b274813a1404)






















<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
