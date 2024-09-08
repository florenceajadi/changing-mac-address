<h4>Changing Mac Address</h4>
<p>MAC Address is a unique identifier assigned to devices like computers or phones that connect to a network. It helps in identifying and communicating with devices on the same local network.</p>


<img src="https://github.com/user-attachments/assets/814dafc7-b923-4bc6-89b9-736ccef6d3cd" height="80%" width="80%" />
<p> I was able to run ifconfig on Kali Linux to show details on my devices like IP addresses, MAC address, and other network info. I picked up: </p>
<p>eth0: The first Ethernet network interface (wired connection).</p>
<p>lo: The loopback interface, used for internal network communication within your device (IP 127.0.0.1).</p>
<p>vmnet2 & vmnet8: Virtual network interfaces created by virtualization software (e.g., VMware) for virtual machines.</p>
<p>wlan0: The first wireless network interface (Wi-Fi connection).</p>
<br />
_________________________________________________________________________________________________________________________________________


  <img src="https://github.com/user-attachments/assets/e8c5cfa2-9b66-4293-9c44-89604e805547" height="80%" width="80%" />

<p> ifconfig wlan0 down command disables the wireless network interface (wlan0), immediately disconnecting it from any Wi-Fi network.</p>
  
   <p>Using ifconfig wlan0 hw ether 00:11:22:33:44:55 command to change the MAC address of the wireless interface (wlan0) to 00:11:22:33:44:55.</p>

   <p>ifconfig wlan0 up command re-connects the wireless network interface (wlan0), allowing it to connect to Wi-Fi networks again.</p>

<br />
_________________________________________________________________________________________________________________________________________


  <img src="https://github.com/user-attachments/assets/d6653df6-6a1f-49c3-bd08-591e66dd5f94" height="80%" width="80%" />
  <p>Using the ifconfig to see the new changes made to wlan0.</p>

  <br />
_________________________________________________________________________________________________________________________________________


  <img src="https://github.com/user-attachments/assets/a0347a09-8680-4a1d-bf39-23565695e3a4" height="80%" width="80%" />
  <p>iwconfig is a Linux command used to display and modify the settings of wireless network interfaces, like changing the Wi-Fi network (SSID), frequency, or encryption settings.</p>
    <img src="https://github.com/user-attachments/assets/0cadd16f-98fd-40eb-b428-33cec0f71577" height="80%" width="80%" />
    <p> ifconfig wlan0 down command disables the wireless network interface (wlan0), immediately disconnecting it from any Wi-Fi network</p>
    <p>airmon-ng check kill stops any background processes (like network managers) that could interfere with putting your wireless network interface into monitor mode, which is used for tasks like packet capturing and wireless network analysis.</p>
      <p>wpa_supplicant is responsible for managing Wi-Fi connections. It handles authentication and ensures your device stays connected to the network. By killing wpa_supplicant, your device's ability to manage and connect to Wi-Fi networks is temporarily disabled, allowing the interface to be used in monitor mode for activities like network scanning or packet capturing.</p>
      <img src="https://github.com/user-attachments/assets/2b0e6cdd-9f4a-4658-aeba-b5be8dcb06f2" height="80%" width="80%" />
      <p>iwconfig wlan0 mode monitor puts the wireless interface (wlan0) into monitor mode, which allows it to capture all wireless traffic, not just traffic directed to or from my device. </p>
      
