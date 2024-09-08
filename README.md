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


  <img src="https://github.com/user-attachments/assets/d48781f7-c8fc-44d2-bec0-7d687ae01a95                                                                                                                                                                                   
                                                              l" height="80%" width="80%" />  
  <img src="" height="80%" width="80%" />
    <img src="" height="80%" width="80%" />
      <img src="" height="80%" width="80%" />
        <img src="" height="80%" width="80%" />
