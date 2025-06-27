<h1>How to Create a VM and Connect Through RDP on MacOS</h1>
This tutorial outlines the creation of a Virtual Machine in Azure and how to access it via Remote Desktop.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop

<h2>Operating Systems Used </h2>

- MacOS
- Windows 10 (22H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Log into Azure
- Create a Virtual Machine
- Connect to Virtual Machine via Remote Desktop

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="1422" alt="image" src="https://github.com/user-attachments/assets/00ec09e6-c923-4725-a125-5a93200a2350" />

</p>
<p>
When you log into Azure search "Virtual Machines". Click it, then press create.
</p>
<br />

<p>
<img width="1061" alt="image" src="https://github.com/user-attachments/assets/c57a3eb7-957e-4293-81ca-74b5d90cceb7" />

</p>
<p>
We didn't create a resource group, but we can create a new one right now. First Initial of your first and last name, followed by Network activities with a "-" between each word. You can name the virtual machine "windows-vm". The region doesn't necessarily matter. West or East US 2 is fine. The availability zone isn't important either, but I would choose the same image. Windows 10 pro, version 22H2 x64 Gen 2.
</p>
<br />

<p>
<img width="1061" alt="image" src="https://github.com/user-attachments/assets/98f7105e-cb17-4076-a9ee-e8947bbb58c4" />

</p>
<p>
You can choose any size. I chose one with 2vcpus (typically the more vcpus = better concurrency). Choose your preferred username and password. Don't forget to agree to licensing at the very bottom of the page in the left corner. Once completed, select next until you're on the networking page.
  
</p>

<img width="1061" alt="image" src="https://github.com/user-attachments/assets/6e15c632-730d-4b04-a03c-5d8b9e4e25de">

<br />
</p>
<p>
I chose to change the name of the virtual network. This is optional. I did the first initial of my first and last name followed by "-vnet". For our purposes, we can skip straight to review and create. A validation will pass and then you will select create again. 
</p>
<br />

<p>

<img width="1428" alt="image" src="https://github.com/user-attachments/assets/cb2b16fa-7caa-4fef-bf90-b4d04e4d0447" />

</p>
<p>
Once to VM is created, search virtual machines again. The new VM we created will appear. Click on it, then copy the IP address.
</p>
<br />

<p>
<img width="1158" alt="image" src="https://github.com/user-attachments/assets/2347bcc3-826b-447c-83cb-94c1373311bb" />

</p>
<p>
Open remote desk top. Hit the + in the top right corner and then selct "Add PC". Under PC name, paste the IP address we copied from the virtual machine. Friendly name is optional, but I named mine "windows-vm". After this is complete press add.
</p>
<br /><p>
<img width="1158" alt="image" src="https://github.com/user-attachments/assets/432d4535-9dfb-4f6c-88f5-d464bdcdb9cf" />

</p>
<p>
Double click the VM once it's added. Insert the username and password that we created earlier for the VM. Then select continue.
</p>
<br />

<img width="1080" alt="image" src="https://github.com/user-attachments/assets/1b1e0ee9-4c8a-49c2-b514-dde7c853d547" />

</p>
<p>
Congratulations! You've successfully connected to the VM via remote desktop!
</p>
<br />
