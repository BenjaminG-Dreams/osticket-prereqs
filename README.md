<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Tech Used</h2>

- Microsoft Azure
- Remote Desktop
- Internet Information Services
- osTicket
- HeidiSQL

<h2>Operating Systems </h2>

- Windows 10</b> (21H2)

<h2>Steps</h2>

- Remote Desktop Connection into your Windows 10 Virtual Machine
- Install / Enable Internet Information Services in Windows WITH CGI
- Download and install PHP Manager for Internet Information Services
- Download and install the Rewrite Module
- Create the directory C:\PHP
- Download PHP 7.3.8 and unzip the contents into C:\PHP
- Download and install VC_redist.x86.exe
- Download and install MySQL 5.5.62
- Open IIS as an Admin and register PHP from within IIS
- Install osTicket v1.15.8
- Download and install HeidiSQL
- Continue setting up osTicket in the browser

<h2>Installation Steps</h2>

![Screenshot 2025-01-30 185248](https://github.com/user-attachments/assets/2ffaa948-e71e-4e6c-b605-d0ffb09b1ee5)
![Screenshot 2025-01-30 185412](https://github.com/user-attachments/assets/d01a8992-a4fd-4d6d-a5fc-91b3b2a3a645)
![Screenshot 2025-01-30 185519](https://github.com/user-attachments/assets/8e455152-abbc-4e38-9238-a1f9528871bd)

<p>
First, we will be connecting to our VM through Remote Desktop Connnection. To do this, go to the VM on the Azure Portal > Copy Public IP Address > Connect with RDC.
</p>
<br />

![Screenshot 2025-01-30 185823](https://github.com/user-attachments/assets/ec1c1cd6-6f6e-4c8f-b22e-37f48f31282d)

![Screenshot 2025-01-30 185910](https://github.com/user-attachments/assets/05191aff-fe91-45dd-8e94-adaef0df6b0c)

![Screenshot 2025-01-30 190012](https://github.com/user-attachments/assets/9ba6293a-28e4-4c76-9b09-82a6db6b6313)

<p>
Paste the link into the browser inside of your VM.

- https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD
</p>
<br />

![Screenshot 2025-01-30 190222](https://github.com/user-attachments/assets/35cc2db9-2787-4880-b138-586cc7c37a17)

![Screenshot 2025-01-30 190345](https://github.com/user-attachments/assets/8af099d4-dd35-44a6-887c-1f3afc11c1bd)

<p>
Go to the Programs section in Control Panel and click on "Turn Windows features on or off".
</p>
<br />

![Screenshot 2025-01-30 190752](https://github.com/user-attachments/assets/0f1b7822-5228-45f8-8b4c-dedd21e49802)

<p>
Next, install and enable IIS in Windows WITH CGI. Check every box shown in the visual step and hit OK to install.
</p>
<br />

![Screenshot 2025-01-30 191133](https://github.com/user-attachments/assets/e5901fd8-278a-48e2-bb1c-79c98b670504)

<p>
After you install IIS, open a new browser and type into the search bar "127.0.0.1". The IIS page should pop up but if you do not see it; you will need to go back to control panel to make sure CGI is checked.
</p>
<br />

![Screenshot 2025-01-30 191330](https://github.com/user-attachments/assets/a58c9da7-92e1-4895-bf26-99f9d3508081)

![Screenshot 2025-01-30 191520](https://github.com/user-attachments/assets/afe0ab6c-a9e7-4fca-9548-aa2bf3ba836b)

![Screenshot 2025-01-30 191617](https://github.com/user-attachments/assets/0f084613-b55c-443b-ba40-db32893dedee)

<p>
Install PHPManagerForIIS_V1.5.0.msi from the install folders.
</p>
<br />

![Screenshot 2025-01-30 191746](https://github.com/user-attachments/assets/a5eb2213-4fe6-499c-9884-f481dab78e39)

![Screenshot 2025-01-30 191903](https://github.com/user-attachments/assets/3fec4a03-867c-4cac-87a4-1cecf30a95db)



<p>
Install rewrite_amd64_en-US.msi from the install folders.
</p>
<br />


![Screenshot 2025-01-30 192458](https://github.com/user-attachments/assets/27aa41d7-07d0-4bad-b3ce-8a6f44c40e7c)

<p>
Next, create a new directory in your C drive called PHP or C:\PHP.
</p>
<br />

![Screenshot 2025-01-30 192618](https://github.com/user-attachments/assets/eb88e5c9-a379-4b6e-8090-f389183193ba)

![Screenshot 2025-01-30 193129](https://github.com/user-attachments/assets/2bf9a56f-3d80-449e-b54f-54d237453544)

![Screenshot 2025-01-30 193221](https://github.com/user-attachments/assets/b10c50c6-2bff-4af1-b9ae-03c37c99f8e5)

![Screenshot 2025-01-30 193349](https://github.com/user-attachments/assets/06994022-fb0d-4065-83ca-a6b6dab93324)

![Screenshot 2025-01-30 193520](https://github.com/user-attachments/assets/29e58481-cf16-4866-a801-479a922a691b)

<p>
Now, download and install php-7.3.8-nts-Win32-VC15-x86.zip and then extract all the contents into C:\PHP.
</p>
<br />

![Screenshot 2025-01-30 193727](https://github.com/user-attachments/assets/9b7e2453-59bf-4f0b-a3d1-aae1dc39c351)

![Screenshot 2025-01-30 193836](https://github.com/user-attachments/assets/d7e80181-784d-4639-a01e-233e0dc319c6)


<p>
Download and install VC_redist.x86.exe.
</p>
<br />

![Screenshot 2025-01-30 194132](https://github.com/user-attachments/assets/5fef6072-6961-4ee3-b27a-73ccb3ada37f)

![Screenshot 2025-01-30 194222](https://github.com/user-attachments/assets/a8fa1924-6a0d-48b9-9c76-fb5774f8b358)

![Screenshot 2025-01-30 194634](https://github.com/user-attachments/assets/f8db430a-458c-48b7-a96e-ea7cb5e09bcd)

![Screenshot 2025-01-30 194711](https://github.com/user-attachments/assets/483473fb-06ac-4ffb-9daa-937728423c37)

![Screenshot 2025-01-30 195117](https://github.com/user-attachments/assets/f8baf812-5c3e-4d2f-a93d-eb9e9ede8418)

![Screenshot 2025-01-30 195148](https://github.com/user-attachments/assets/cda33e4b-00d8-4bc1-8b48-a859e0ef172f)

<p>
Download and install mysql-5.5.62-win32.msi
- Typical Setup > Launch Wizard > Standard Configuration > Next > Set the Username and password to "root" > Execute
</p>
<br />

![Screenshot 2025-01-30 195413](https://github.com/user-attachments/assets/4715c654-a96f-4909-9229-0dbfef75993c)

<p>
Search for IIS in the search bar and open it as administrator.
</p>
<br />

![Screenshot 2025-01-30 195708](https://github.com/user-attachments/assets/1f0a00b1-e74a-4d09-b6d8-30113c217512)

![Screenshot 2025-01-30 200000](https://github.com/user-attachments/assets/85af8c0e-76b8-4764-bd3d-768c54eaa868)

<p>
After opening IIS Manager as admin, click on "PHP Manager" icon > click on "Register new PHP version" > Browse files > C:\PHP > open "php-cgi"
</p>
<br />

![Screenshot 2025-01-30 200154](https://github.com/user-attachments/assets/535042f5-7e4e-4ba5-a439-be104ce5799b)

<p>
Stop the IIS server.
</p>
<br />

![Screenshot 2025-01-30 200303](https://github.com/user-attachments/assets/5fa0515d-a12f-49f4-8d67-c69860d6dcf9)

<p>
Start the IIS server.
</p>
<br />


![Screenshot 2025-01-30 200516](https://github.com/user-attachments/assets/c2067945-a662-49b9-acf7-207e0483f553)

![Screenshot 2025-01-30 200545](https://github.com/user-attachments/assets/268034c2-9d76-4927-86b9-41208c7e1bf0)

<p>
Now, download the file osTicket-v1.15.8 from the install files. After it finishes downloading, open two file explorer windows and navigate to the osTicket-v1.15.8.zip folder and "inetpup".
</p>
<br />

![Screenshot 2025-01-30 201458](https://github.com/user-attachments/assets/62b39976-718c-4ea5-bd25-9e14b79f4150)

![Screenshot 2025-01-30 201759](https://github.com/user-attachments/assets/9407b687-6658-4639-a7a7-7b89dd3a0b13)


<p>
In the inetpup folder, go to "wwwroot" and transfer the "upload" folder in from the osTicket zip. After it finishes, rename the "upload" folder to "osTicket". 
</p>
<br />

![Screenshot 2025-01-30 200154](https://github.com/user-attachments/assets/cfef5da9-6ae5-4c16-8ebe-28e52fbf4f45)

<p>
Stop the IIS server.
</p>
<br />

![Screenshot 2025-01-30 202028](https://github.com/user-attachments/assets/c146461c-d2e3-456e-97d6-7286e46cee50)

<p>
Restart IIS as admin and expand VM1 on the left menus > Sites > Default Web Sites > Click osTicket. Click on "Browse *.80 which will open web browser that will open a osTicket installer.
</p>
<br />

![Screenshot 2025-01-30 202303](https://github.com/user-attachments/assets/c261770e-54b7-4ca2-b267-de109a1604aa)

![Screenshot 2025-01-30 202322](https://github.com/user-attachments/assets/468d47b6-22b2-4860-9a40-725d4c1d182a)

<p>
Head back to IIS Manager and into osTicket again. Click on the "PHP Manager" icon and then at the bottom click "Enable or disable an extension".
</p>
<br />

![Screenshot 2025-01-30 202550](https://github.com/user-attachments/assets/08b01bf9-f236-49fa-8f1b-9437ce91e8a1)

<p>
Enable "php_imap.dll", "php_intl.dll", and "php_opcache.dll" by right clicking and hitting enable. And Refresh the web browser that has the osTicket installer and observe the changes. It should look like the screenshot above.
</p>
<br />

![Screenshot 2025-01-30 203317](https://github.com/user-attachments/assets/57638e1a-355c-4fcf-beb4-2c10bb3f9763)

<p>
Open up file explorer and navigate back to osTicket inside of inetpub. Click on include and locate "ost-sampleconfig.php" at the bottom of the list.And then rename the file from "ost-sampleconfig.php" to "ost-config.php"
</p>
<br />

![Screenshot 2025-01-30 203658](https://github.com/user-attachments/assets/07edd4e2-f897-40f7-af4e-91cd9d5e9287)

<p>
Now, click on that files Properties > Security > Advanced > Disable Inheritance > Remove all.
</p>
<br />

![Screenshot 2025-01-30 203936](https://github.com/user-attachments/assets/59ab9cf9-7bf3-43a4-822a-102c0313eb99)

<p>
Afterwards, click Add > Select a principle > type "everyone" in the object box > Check name > Press Ok.
</p>
<br />

![Screenshot 2025-01-30 204059](https://github.com/user-attachments/assets/68e6e736-3ef9-433f-b7c5-472fd1482ae6)

![Screenshot 2025-01-30 204146](https://github.com/user-attachments/assets/c9e6a221-c9c3-4330-8cd9-11b5f7440f62)

<p>
Check the box for "full control" > press OK > Apply and then OK until the properties window closes.
</p>
<br />

![Screenshot 2025-01-30 204232](https://github.com/user-attachments/assets/f65b47ef-85db-4fdf-8e5f-d7df579199af)

<p>
Head back to the osTicket installer and press "Continue".
</p>
<br />

![Screenshot 2025-01-30 204658](https://github.com/user-attachments/assets/a44f9b91-25ee-40b0-bf6e-966ee4e04302)

![Screenshot 2025-01-30 204802](https://github.com/user-attachments/assets/327c952d-5eb7-42ec-a709-68c8352c6166)

![Screenshot 2025-01-30 204830](https://github.com/user-attachments/assets/963d7aac-e854-4728-9da3-01f8fefd2356)

![Screenshot 2025-01-30 204909](https://github.com/user-attachments/assets/6367c373-5b50-4c65-bb21-713758609e7c)

![Screenshot 2025-01-30 205023](https://github.com/user-attachments/assets/6f231bdb-7858-4e94-b69e-630ce9a340ab)


<p>
Next, download HeidiSQL from the drive folder which contains a word doc with a link to the downloader. Open the installer and click continue all the way through. Once it has installed you will click the "New" button at the bottom of the window > the username should already be set to "root" and type the password that we created "Password1" > press open.
</p>
<br />

![Screenshot 2025-01-30 205126](https://github.com/user-attachments/assets/fe15680d-ed17-41d5-872b-9f235c8c653c)

![Screenshot 2025-01-30 205152](https://github.com/user-attachments/assets/b196b2a1-43b6-485f-a7f8-454c38af7ebb)


<p>
Inside of HeidiSQL, right click "Unnamed" > Create new > Database > Name it "osTicket"> Click OK.
</p>
<br />

![Screenshot 2025-01-30 205347](https://github.com/user-attachments/assets/2803c625-2802-42a2-b04a-75d471706211)

<p>
Name your Helpdesk to your liking and a random email. This tutorial will be using the name "Helpdesk" and the email "john@helpdesk.com". You will continue the form by making your own Admin user credentials. I used a random email and created a password; be sure to write these down if you are forgetful Then, head to Database settings the the username and password should be "root" and "root". The hostname should also be "osTicket".
</p>
<br />

<p>
And if you want to clean up some of the extra stuff in the tutorial, we'll browse back into C:\inetpub > wwwroot > osTicket > delete the "setup" folder.
</p>
<br />

<h1>Stay Tuned for osTicket: Post-Installation Configuration!</h1>
