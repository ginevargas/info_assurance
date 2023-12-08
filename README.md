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
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/25bbb021-d402-49af-963a-669f81ca1d20" width="500">
* **Step 2:** Open the terminal on your computer. Connect to the Pi using SSH: Type the following command, replacing **<pi_ip>** with your Raspberry Pi's IP address: **ssh user@<pi_ip>**. Enter the default password (raspberry) when prompted.
  ![2](https://github.com/ginevargas/info_assurance/assets/145625291/5a7d292a-727b-4dc0-a785-e8e722934876)

* **Step 3:** Run the following command to update and upgrade package lists: **sudo apt update**, **sudo apt upgrade**
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/4b445379-8820-4c4a-a947-e22ca93c05eb" width="70%">

* **Step 4:** 
* **Step 5:**
* 
### 3. Deploying LAMP (Linux Apache MySQL PHP) Stack in raspberry Pi.
* **Step 1:**  Install LAMP stack. Install Apache, MySQL, and PHP using the following command:  
sudo apt install apache2.   
sudo apt install mariadb-server.  
sudo mysql_secure_installation.  
sudo apt install php libapache2-mod-php php-mysql.  
sudo apt-get install php*.  
sudo apt install phpmyadmin.  
* **Step 2:** Run the **sudo apt install apache2** in your terminal.  
  <img src= "https://github.com/ginevargas/info_assurance/assets/145625291/0432b10c-1c92-4e3f-8bb2-15cb7ececa19" width="70%">

* **Step 3:**
* **Step 4:**
* **Step 5:**
* 
### 4. Enabling and controlling Raspberry Pi using VNC.
* **Step 1:**
* **Step 2:**
* **Step 3:**
* **Step 4:**
* **Step 5:**
* 

