# Linux Project
<b>Objective</b> - Install VirtualBox on Windows. Download, Install, &amp; Configure Ubuntu Linux. 

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h1>Install VirtualBox on Windows:</h1>

<h2>Download VirtualBox</h2>

- <b>1. [Go to virtualbox.org](https://virtualbox.org)</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/2b1d986f-055e-429a-b4d3-635467639100)

- <b>2. Click giant button [Download VirtualBox "insert version number here" (ex: 7.0)]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d33598db-349e-4e11-bba7-9fb2cda84d9f)

- <b>3. Click on [Windows hosts]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/cd7856fa-1f43-4a46-a037-f73e38fa8fd3)

- <b>4. Once the download is finished, wait … DO NOT OPEN THE FILE AFTER DOWNLOADING.. the next step to verify the integrity of the file to make sure it's the correct one.</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/348880e6-dde2-4980-b533-be0b71679aeb)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Verify VirtualBox Integrity (Optional but Highly Recommended)</h2>

- <b>1. Open where your files are downloaded in file explorer to see if the file is there. If yes, then proceed to next step.</b>

- <b>2. In the address bar type "powershell" and a terminal should pop up in the folder where you have your downloaded file.</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d492a04b-e913-45a8-9285-e7260e0e3ad1)

- <b>3. In the terminal type "Get-FileHash", then the path, which by default is - C:\Users\(your_user_name)\Downloads.</b>
  - <i>(Note) If you can't find this then right click on your address bar and select "Copy Address".</i>
- <b>	After that, type, or copy and paste the ENTIRE file name including the ".exe". (EX: \VirtualBox-6.1.30-148432-Win.exe).
- Then after that type "-A SHA256".</b>
  - <i>The entire code should look something like this:</i>
  - `Get-FileHash C:\Users\wayne\Downloads\VirtualBox-6.1.30-148432-Win.exe -A SHA256`
  - ![Screenshot 2023-12-19 180311](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/b5a781ef-7714-4c37-a175-89b7633d82a9)

- <b>4. Press Enter and a Hash should pop up</b>
  - ![Screenshot 2023-12-19 180633](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/7153c0ea-482d-4ea6-a2da-fcae20f78f25)

- <b>5. Back on the downloads page of VirtualBox navigate to [SHA256 checksums] and click it. Leave the screen there until the next step.</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/36fc57c5-bc7c-4c18-82f5-ba7411cc80f7)

- <b>6. Place that screen with the SHA256 checksums and the PowerShell terminal side by side so you can compare the two.</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/293f485d-15f7-439a-8dca-0ed6e094b83d)

- <b>7. On the right hand side of the checksums, find the version of VirtualBox you have downloaded.
	- Then look at the string of letters and numbers next to it.
  - If it matches with the Hash in your PowerShell, then you are finished with the verification. If not, then you may have a manipulated file and should not open it.

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Download Ubuntu</h2>

- <b>1. [Go to ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d84d4b30-4976-4347-8110-fdc25c3f3d55)

- <b>2. Scroll down and click on the button with the highest version. EX: [Download 23.10]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/604ec342-7702-45ef-b0c0-979dc95c1f2b)

- <b>3. Wait for download to complete and move on to next step.
  -  ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/4f247bd8-acf6-4806-bd0b-2e63fe91299a)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Install VirtualBox</h2>

<h3>Page Name - Welcome to the Oracle VM VirtualBox "insert version number here" Setup Wizard</h3>

- <b>1. Action - Click [Next]</b>
  - <i>(Note) Click next to proceed with the setup. Otherwise, click cancel.</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/dd37ef3c-528e-468b-9baf-8439d88741b7)

<h3>Page Name - Custom Setup</h3>

- <b>2. Action - Click [Next]</b>
  - <i>(Note) Install all features of VB by just clicking next. Leave the "Location" alone unless you have no space on the default drive.
  - Click "Browse" if there is no space on the default drive and find another with more space.</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/bfe1e3b4-8497-4eb4-b35e-fae16174b3ee)

<h3>Page Name - Warning: Network Interfaces</h3>

- <b>3. Action - Click [Yes]</b>
  - <i>(Note) Temporary disconnect from the network</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d7871992-5307-49f9-83df-197a4f215a87)

<h3>Page Name - Missing Dependencies Python Core / win32api</h3>

- <b>4. Action - Click [Yes]</b>
  - <i>(Note) Installs missing dependencies</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/5a34b345-ef4f-4bcf-a669-cdd9641d8ffe)

<h3>Page Name - Ready to Install</h3>

- <b>5. Action - Click [Install]</b>
  - <i>(Note) Proceed with installation</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/7a127b27-1a05-46ba-9df8-6a3f50f6b297)
 
<h3>Page Name - Oracle VM VirtualBox "insert version name here" installation is complete.</h3>

- <b>6. Action - Click [Finish]</b>
  - <i>(Note) Leave checkbox for "Start Oracle VM VirtualBox after installation" checked to start up VirtualBox after clicking "Finish"</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/1df231dd-62de-4b60-8e9e-906eda1ed3fa)
 
<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Download VirtualBox Extension Pack (Optional)</h2>

- <b>1. Head back to the VirtualBox downloads page [virtualbox.org/wiki/Downloads]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/8e8544e3-8949-4167-8f46-5ccf8a8a96db)
 
- <b>2. Locate the header that says "VirtualBox (version number) Oracle VM VirtualBox Extension Pack" and click [All supported platforms]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/7e69654d-b876-4c36-b3eb-064de4c26c97)
 
- <b>3. Once the download is finished, click the file in your browser to run the "Setup Wizard"</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/f42fb355-ec67-4c83-8134-3e08d5ec3e51)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Install VirtualBox Extension Pack (Optional)</h2>

- <b>1. Action - Click [Install]
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/32b25bbc-5dc0-482d-b3e8-887f93e01cc3)
 
- <b>2. Action - Scroll down and Click [I Agree]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/e8598fe3-6a82-452b-b4d5-2bc808327dcf)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h2>Install Ubuntu</h2>

- <b>1. In VirtualBox click [New] in the Machine Tab</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/30a82427-f42f-4872-a21c-563a0c891847)
 
- <b>2. Create the VM
  - a) In "Name", type Ubuntu.
  - b) Leave "Folder" alone.
  - c) In "ISO Image" click the drop down menu and choose "Other…"
  - d) Find your Ubuntu ISO and click on it and then click [Open]</b>
  - ![Screenshot 2023-12-19 211718](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/78639fb6-7d36-4174-af33-58c6748214c1)

- <b>3. Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/fbd64944-c360-4213-9bc8-905ff9a6c2f8)

- <b>4. Unattended Guest Setup
  - a) Choose a username, hostname (device name) and password
  - b) Leave "Domain Name" alone
  - c) Click check box for "Guest Additions"
  - d) Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/4295bda6-3601-4aa4-a3b6-dfab7fef3680)
 
- <b>5. Allocate Memory and CPU
  - a) Give about 4,096 Megabytes (4.096 Gigabytes) and at least 4 CPUs
  - b) Enable EFI
  - c) Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/ddf9873e-8f41-4d2a-bc07-f8563deb74e6)
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/6d4d37a4-ee7d-4736-8370-eab1bb9f3245)
 
- <b>6. Choose Hard Disk Space and then click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d1a19a0d-7f31-4c79-bea5-54f934c109d4)

- <b>7. Review and Click [Finish]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/885d30fd-3b66-4c9e-9cbc-4790e8ce433f)

- <b>8. Wait for a few processes to run and then it should open up a new window and bring you to this screen (BIOS/EFI) then click [Enter] on "Try or Install Ubuntu":</b>
  - <i>(Note) If it gives you an error before the EFI screen and asks to mount a DVD again then just choose the same Ubuntu ISO and click next</i>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/cb069dac-0588-4112-8e50-9c3311deadb8)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->


<h1>Ubuntu Setup</h1>

<h2>Setup Pages</h2>

- <b>1. You should land on this screen. Choose your language and click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/25683594-becd-4fef-a7e9-43486f83be11)

- <b>2. Select Install Ubuntu and Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/4be39357-4a0c-43f1-81b5-22126c7d8c70)
 
- <b>3. Choose Keyboard Layout and Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/79af9ea6-542b-4527-a074-dbec0eb3ce5a)

- <b>4. Choose a network connection type and Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/b91360ae-93d2-49ad-a0a8-157955f0d41a)
 
- <b>5. Click the update if available</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/fb9d55fa-6683-4a7a-a271-4bffef7fd3ce)
 
- <b>6. Restart the Installer</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/29b52f49-0254-44e7-a7ca-e2fe2b219589)
 
- <b>7. Click [Next] until you reach this screen:
  - a) Default installation to reduce your attack surface
  - b) Install the drivers and support
  - c) Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/b72b7400-30a7-4def-a073-4933783138b8)

- <b>8. Choose manual partitioning and Click [Next]</b>
  - ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/d999fbea-aa16-4906-bde8-733c95f0d150)

<!---------------------------------------------------------------------- SECTION BREAK ---------------------------------------------------------------------->

<h2>Define Multiple Partitions</h2>

<i>(Note) Will be using Ext4 instead of more secure/under development Btrfs for stability/simplicity but suggest learning how to set it up.</i>

<h3>1. Separate /boot</h3>

- <b>Select Free Space, then click the "+" sign.</b>
	- ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/050db9b3-d37b-4cb7-b251-c7c0ea149a77)
- <b>a) Size: 500 MB
- b) Used as: Ext4
- c) Mount Point: /boot
- d) Click [OK]</b>
	- ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/231587fe-451c-4d93-acce-651c54049631)
- <b>Result:</b>
	- ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/fbadacbe-e7e5-496b-a58c-68db6f772afc)
  - <i>(Note) /boot/efi is automatically created and that is normal.</i>

- <b>Notes:
- Priority - [LOW]
- Significance:</b> <i>Separating /boot helps in keeping the kernel and bootloader files isolated.
- This is useful in situations where the root file system is encrypted, as the bootloader can access the /boot partition without encryption.</i>

<!-------------------------------------- SMALL BREAK -------------------------------------->


<h3>2. Separate /swap</h3>

- <b>Select Free Space, then click the "+" sign.
- Size: Amount of Ram you chose (4GB)
- Used as: Swap
- Mount Point: N/A
- Click [OK]</b>
	- ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/6a6d57a3-c24a-4a9b-b4e2-3ac5497052a3)
- <b>Result:</b>
	- ![image](https://github.com/AngelMcArthur/Linux-Project/assets/55830075/64ab8733-cb8e-428f-8e51-7c12faa3387c)

- <b>Notes:
- Priority - [LOW]
- Significance:</b> <i>Swap is a special area on the disk that the system uses as extra memory. 
- A good rule of thumb is to make the swap partition the same size as your RAM, or 1.5 times that amount if you have less than 4GB of RAM.</i>

<!-------------------------------------- SMALL BREAK -------------------------------------->

