# Final Project Documentation.
by Group 7: Maraño, Mary France S., Pajenago, John Mark A., Quial, John Paul A., Vargas, Regine B.  

.    
##  Step-by-step documentation on how to do the following:
### 1. Prepare and Install Headless Raspbian OS in Raspberry Pi.
* **Step 1:** Download Raspbian OS. Head over to (https://www.raspberrypi.com/software/) and download the latest version of Raspbian OS (now called Raspberry Pi OS).
* **Step 2:** Insert your SD card into your computer and launch Raspberry Pi Imager. Select the "Choose OS" option and navigate to the downloaded Raspbian image file. Choose the SD card and click "Write." This will format the SD card and flash the Raspbian image onto it.
* **Step 3:** Enable SSH (Headless Setup). Create an empty file named ssh (without any extension) in the root directory of the microSD card. This enables SSH on the Raspberry Pi.
* **Step 4:** Configure Wi-Fi (Optional).
* **Step 5:** Boot your Raspberry Pi. Insert the SD card into your Raspberry Pi and connect it to a power source and an ethernet cable. The Pi will boot up automatically.

### 2. Connecting to Raspberry Pi via SSH using the terminal.
* **Step 1:** Find Raspberry Pi IP Address. Use a network scanning tool or check your router's connected devices to find the IP address assigned to your Raspberry Pi.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/25bbb021-d402-49af-963a-669f81ca1d20" width="50%">
* **Step 2:** Open the terminal on your computer. Connect to the Pi using SSH: Type the following command, replacing **<pi_ip>** with your Raspberry Pi's IP address: **ssh user@<pi_ip>**. Enter the default password (raspberry) when prompted.
  ![2](https://github.com/ginevargas/info_assurance/assets/145625291/5a7d292a-727b-4dc0-a785-e8e722934876)

* **Step 3:** Run the following command to update and upgrade package lists: **sudo apt update**, **sudo apt upgrade**
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/4b445379-8820-4c4a-a947-e22ca93c05eb" width="70%"> 
### 3. Deploying LAMP (Linux Apache MySQL PHP) Stack in raspberry Pi.
* **Step 1:**  Install LAMP stack. Install Apache, MySQL, and PHP using the following command:  
sudo apt install apache2.   
sudo apt install mariadb-server.  
sudo mysql_secure_installation.  
sudo apt install php libapache2-mod-php php-mysql.  
sudo apt-get install php*.  
sudo apt install phpmyadmin.  
* **Step 2:** Run the **sudo apt install apache2** on your terminal.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/0432b10c-1c92-4e3f-8bb2-15cb7ececa19" width="70%">.  
  If it ask "Do you want to continue?" type 'y' and enter.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/e6cbbd4f-adc9-48cb-8660-689029d3a9f1" width="50%">
* **Step 3:** After installing Apache, next run the **sudo apt install mariadb-server** on your terminal.
   <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/95d2066c-66af-4739-a5da-a78f2b89642c" width="50%">.  
   If it ask "Do you want to continue?" type 'y' and enter.  
   <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/271a00e7-129b-4523-8735-fcaf490b6277)" width="50%">
* **Step 4:** After installing the mariadb-server, next run **sudo mysql_secure_installation** on you terminal.
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/c76e19b4-e03e-4301-afdb-1f1cf4ebd2b9" width="70%">.  
  Enter your password for root.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/4da9c8e3-7dde-45a5-943f-9c2887b99e09" width="70%">.  
  type 'y' and enter.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/849148fd-e30f-467d-98ac-d472bca0ad49" width="50%">
* **Step 5:** Next, run and install **sudo apt install php libapache2-mod-php php-mysql** on your terminal.
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/29b377b5-62f0-49e0-b42d-f70cd77de590" width="50%">
* **Step 6:** Next, the last step is to run and install **sudo apt-get install php***, **sudo apt install phpmyadmin** on you terminal.
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/90fd215f-3722-409c-91db-3332e7384523" width="50%">
### 4. Enabling and controlling Raspberry Pi using VNC.
* **Step 1:** Installing RealVNC Server on Raspberry Pi: **sudo apt install realvnc-vnc-server**
* **Step 2:** Enabling VNC Server. Enter the command **sudo raspi-config** to your computer terminal.
* **Step 3:** Use the arrow keys to select Interfacing Options and press Enter.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/f15b59fc-f6a7-493c-a9f7-adb82fc9e9e2" width="50%">
* **Step 4:**  Use the arrow keys to select VNC and press Enter.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/322f4ad9-71ee-4db1-bee6-4273ee000bf7" width="50%">
* **Step 5:** You will be prompted to enable VNC Server. Select Yes and press Enter.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/b29e26f5-5015-44b3-9988-7c91c2a121b5" width="50%">  
* **Step 6:** Use the arrow keys to select Ok and then Finish, to return to the terminal.
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/8669592b-ad60-439a-8886-b1d4343db8bd" width="50%">
* **Step 7:** Download and install RealVNC Viewer on your computer.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/d291daaa-43d8-4569-92d1-06c0d593f494" width="50%">
* **Step 8:** Open VNC Viewer and enter the IP address of your Raspberry Pi. Log in with the Raspberry Pi credentials.
* **Step 9:**  Control Raspberry Pi through VNC: You can now use the VNC viewer to interact with the Raspberry Pi desktop as if you were physically connected to it. You can launch applications, configure settings, and manage your Raspberry Pi remotely.


.  
**BACHELOR OF SCIENCE IN COMPUTER SCIENCE**  
**CS 3A_CS 319_INFORMATION ASSURANCE AND SECURITY**
  
