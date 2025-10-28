<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket Installation</h1>
<p align="center">How To Install OsTicket.</p><br />


<h2 align="center">Video Demonstration</h2>

<p align="center"><a href="https://youtu.be/qozYHcSI2mg"><b>OsTicket Installation</b></a></p>

<h2 align="center">Environments and Technologies Used</h2>

<p align="center">Microsoft Azure</p>
<p align="center">Remote Desktop</p>
<p align="center">Internet Information Services (IIS)</p>

<h2 align="center">Operating Systems Used </h2>

<p align="center">Windows 10</p>

<h2 align="center">List of Prerequisites</h2>

<p align="center">Create A Virtual Machine In Azure.</p>
<p align="center"><a href="https://docs.osticket.com/en/latest/"><b>Download The Prerequesites</b></a>.</p>

<h2 align="center">Installation Steps</h2>

<p align="center">
<img src="https://i.imgur.com/tQOv9cq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Search For The Control Panel; Click <b>Uninstall A Program</b>, Then Click <b>Turn Windows Features On Or Off</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/r3QyPhn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Install <b>PHP Manager For IIS</b> and <b>The Rewrite Module</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/Slc6xID.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
In The Folder, <b>This PC</b>, Add A New Folder Titled <b>PHP</b> To Create The Directory.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/HXnAhLy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Extract The Necessary <b>php...</b> Folder To The PHP Directory.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/xyzd8c7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
<img src="https://i.imgur.com/Y6cNOnX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
1. Open IIS, Double-Click PHP Manager From The Top Level.
</p>
<p align="center">
2. Click <b>Register New PHP Version</b>.
</p>
<p align="center">
3. Type In "<b>C:\php-cgi.exe</b>".
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/iYJwuZN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Install MySQL And Choose The <b>Typical</b> Option With <b>Standard Configuration</b>. 
  <h3 align = "center"><b>Do Not Forget The Password You Set Here</b></h3>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/1ZYRPjG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Install The <b>VC Redistributable</b>.
</p>
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/qyk4gkJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Rename File, <b>ost-sampleconfig.php</b>, To <b>ost-config.php</b>
</p>
<p align="center">
<img src="https://i.imgur.com/MQpRcMm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Right Click <b>ost-config.php</b>.</p><p align="center"> In <b>Properties</b>, Under The <b>Security</b> Tab, Set <b>Inheritance</b> To <b>Full Control</b> For <b>Everyone</b>.
</p>
<p align="center"><sub><em>~We Will Remove Full Control Later On~</em></sub></p>
<br />

<p align="center">
<img src="https://i.imgur.com/AilrtxV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/pUWUIfx_d.webp?maxwidth=760&fidelity=grand" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KUbgDDL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vn3dDV6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p align="center">
1. In IIS, Open: <b>osticket</b> > <b>Sites</b> > <b>Default Web Site</b> > <b>osTicket</b> And Double-Click <b>PHP Manager</b>.
</p>
<p align="center">
2. Under <b>PHP Extensions</b>, Click: <b>Enable Or Disable An Extension</b>.
</p>
<p align="center">
3. Enable <b>php_imap.dll</b>, <b>php_intl.dll</b>, And <b>php_opcache.dll</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/QwHiT11.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
After Clicking Continue, Fill In The Textboxes Under <b>System Settings</b> And <b>Admin User</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/4kqnz8r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Install <b>HeidiSQL</b>
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/KjItS1y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Click <b>New</b>, To Create A New Session. Recall The Username And Password From MySQL. Click <b>Open</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/y5e6ByH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
A New Window Of File, <b>Unnamed</b> Will Open. Right-Click <b>Unnamed</b>, Select <b>Create New</b>, Select <b>Database</b>. 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/hOYtoLM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
When The Small Window Opens, Type "<b>osTicket</b>" In "Name:"
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/oQzUMT1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Finish <b>Database Settings</b>. The Information For <b>Name</b> Is "osTicket". Recall The Username And Password You Set In <b>MySQL</b>.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/0oCEUCw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
Change Inheritance Of Everyone To <b>Read</b> Only.
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/ONP8zld.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
<b>Delete C:\inetpub\wwwroot\osTicket\setup</b>
</p>
