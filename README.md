<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install / Enable IIS in Windows
- Install web platform installer
- Install My SQL
- install c++ redistributable
- Item 5 configure permissions install OS ticket

<h2>Installation Steps</h2>


<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/3a4e5fb1-01a2-4286-b86d-94b3266437f4" height="80%" width="80%" alt="ISS Installation"/>
</p>
<p>
  -1) Go to Apps & Features under setting
 - 2) select Programs an Features
 - 3) Select Turn Windows features on or off
-  4)navigate to Internet Information Services>World Wide Web Services
  -5) Under Application Development Features make sure CGI is selected
  6)under Common HTTP Features make sure every folder is checked.
</p>
<br />
![PHP Folder creation]()
![PHP Folder extraction]()

<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/7009c703-0867-4bb1-ac09-70ad7967f965" height="80%" width="80%" alt="Resources"/>
</p>
<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/93abbf3e-a2e2-4719-aea0-29d8863368d2" height="80%" width="80%" alt="Resources"/>
</p>
<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/7009c703-0867-4bb1-ac09-70ad7967f965" height="80%" width="80%" alt="Resources"/>
</p>
<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/9a0de007-c096-4f88-ab15-c386101f035d" height="80%" width="80%" alt="Resources"/>
</p>
<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/b1273125-d8fd-4070-a538-e700eba7e72b" height="80%" width="80%" alt="Resources"/>
</p>
<p>
Download PHP Files and other resources.
  1) Install PHP Manager and Rewrite Module
  2) Create a PHP folder in C://
  3) Extract PHP files into the newly created folder 
  4) Register PHP from within IIS, then restart
</p>
<br />

<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/ae64ea4a-5697-44fd-80b5-97aedf35cbc4" height="80%" width="80%" alt="MySQL Download and c++ redistributable"/>
</p>
<p>
Install C++ Redistributable, then MySQL. After MySQL is finished installing go through the setup Wizard
</p>
<br />
![osTicket Download](https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/fd11e8c1-69e0-4946-b4a1-846300cef69c)
![osTicket setup](https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/e3c26782-5dc4-4f60-8d66-883784ddd46f)
![Browse to 80](https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/e49d22b9-101f-404d-b3f5-a715feaa6e55)
![enable extensions](https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/a6cf64ef-9965-40c7-b46e-268bd2e611ee)
![Rename and assign permissions](https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/382e03ec-4d2f-4814-94ce-ee01561b3b0c)


<p>
<img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/fd11e8c1-69e0-4946-b4a1-846300cef69c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/e3c26782-5dc4-4f60-8d66-883784ddd46f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/e49d22b9-101f-404d-b3f5-a715feaa6e55" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/a6cf64ef-9965-40c7-b46e-268bd2e611ee" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://github.com/JZumbuehl/osticket-prereqs/assets/159186024/382e03ec-4d2f-4814-94ce-ee01561b3b0c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and Install osTicket
  1) Extract osTicket and copy the upload file
  2) Navigate to C:/inetpub/wwwroot and paste the Upload folder there. then rename the upload folder to osTicket
  3) Within IIS, on the left-hand side, navigate to Sites, and click on Browse *:80 (http) on the right-hand side
  4) Back on the IIS window, from sites go to >default website > osTicket, click on the PHP icon, then click on enable or disable an extension. 
  5) On the PHP extensions page enable php_imap.dll, php_intl.dll, and php_opcache.dll.
  6) Refresh IIS, and check the webpage that was opened to view the changes. 
  7) Go to C:/inetpub/wwwroot/osTicket/include, locate the ost-sampleconfig.php file, and rename it to ost-config.php. 
  8) Open the properties of the folder, go to security, and open up permissions. Remove all of the current permissions, and add a new permission for Everyone, and give it full access. 
  
</p>
<br />
