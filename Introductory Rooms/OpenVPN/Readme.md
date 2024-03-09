<h1 align="center">
  
![image](https://github.com/konboot/TryHackMe/assets/53315283/4e49ee58-b847-4775-b0ad-223da62cb39d)
<br>OpenVPN
</h1>


<p align="center">OpenVPN is a virtual private network (VPN) system that implements techniques to create secure point-to-point or site-to-site connections in routed or bridged configurations and remote access facilities. It implements both client and server applications.</p>

<h2 align="center">A guide to connecting to our network using OpenVPN.</h2>
<p align="center">1. To connect to OpenVPN on Windows, you will need to use the OpenVPN connect software provided on their website. </p>
<p align="center">Download the OpenVPN GUI application with this link https://openvpn.net/community-downloads/ select the most recent release and download the version that is supported on your machine (x64, x32, ARM).<br>
  
![image](https://github.com/konboot/TryHackMe/assets/53315283/15c01baf-751c-40a6-b842-e2c180d30aaf)
</p>

<p align="center">2. After installing the OpenVPN setup wizard, run through the steps. If OpenVPN does not automatically start afterwards, run the OpenVPN executable. Ensure you are running it as an administrator.<br>
  
 &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; ![Screenshot 2024-03-09 172928](https://github.com/konboot/TryHackMe/assets/53315283/20ecb1b7-8c1b-4f7a-9e3a-f94c39672416)
<br></p>

<p align="center">3. Scroll to the top of the page and download your configuration found in the Machines tab.<br>

  ![image](https://github.com/konboot/TryHackMe/assets/53315283/77030e42-0054-4634-90e3-7d9297625fcd)
<br>

<p align="center">4. If your region does not appear on the list, select the one closest to you.<br>
  
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; ![image](https://github.com/konboot/TryHackMe/assets/53315283/a784d9f9-b00d-4abe-abf5-dc803e8ea5e9)
<br>

<p align="center">5. In the bottom right of your screen, on the task bar, press the click the icon that looks like an up arrow (^). There should be an icon within the new window that looks like a monitor with a plug, right-click. This is where you will manage your OpenVPN connections.<br>

<p align="center">6. Next hover over Import, select Import file and navigate to your OpenVPN profile.<br>
  
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  ![Screenshot 2024-03-09 174932](https://github.com/konboot/TryHackMe/assets/53315283/1ac18504-2277-467c-88b1-c4ddf0c55ece)
<br>

<p align="center">7. Finally, right-click on the OpenVPN icon again, select Connect and wait for it to notify you that you have been connected successfully.<br>
  
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;![Screenshot 2024-03-09 175042](https://github.com/konboot/TryHackMe/assets/53315283/1158adcd-e6a9-482f-acd9-98e03213a00d)

<br>

 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;![image](https://github.com/konboot/TryHackMe/assets/53315283/668eb76a-f368-4650-958b-b707adb8ddd8)</p></center>

<b>NOTE:</b> <p>If you are unable to connect to our network through the VPN, you can deploy a Kali-based AttackBox machine and control it in your browser. The AttackBox button is available in the room you are in and located on the top-right side.  You can then access all TryHackMe machines through that machine. Free users can deploy the machine for 1 hour a day, subscribers have unlimited access.

![image](https://github.com/konboot/TryHackMe/assets/53315283/542721c6-74f8-4de4-9afe-4a2d3e29c770)


An in-browser window will then appear, wait for your machine to load, and you will be able to access machines through the Kali Linux machine without being connected to a VPN.</p>




