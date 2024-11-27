<h1>DHCP</h1>
<p>DHCP (Dynamic Host Configuration Protocol) is a network protocol that automatically assigns IP addresses and other network configuration information to devices on a network.</p>
<h3>*Installing DHCP on Member Server</h3>
<p>1. To install DHCP on Member Server, do the following; .From the server manager-dashboard, go to Manage > Add roles and features</p>
<p align="center"><img src="https://i.imgur.com/BFw3fUz.png" height="50%" width="50%"/>
  
<p>2. On the before you begin screen, just click NEXT.</p>
<p align="center"><img src="https://i.imgur.com/gaMZiFi.png" height="50%" width="50%"/>

<p>3. On the Installation Type screen, make sure the Role-based or feature-based installation is selected, then click <b>NEXT.</b>.</p>
<p align="center"><img src="https://i.imgur.com/ZvY3YRt.png" height="50%" width="50%"/>

<p>4. On the Select destination server screen, make sure the select a server from the server pool is selected and select the server you are trying to install Adds from the server pool, then click NEXT.</p>
<p align="center"><img src="https://i.imgur.com/dd0OaUL.png" height="50%" width="50%"/>

<p>5. On the select server roles screen, search for DHCP and click on add features from the pop-up screen, then click NEXT.</p>
<p align="center"><img src="https://i.imgur.com/xKVg1jx.png" height="50%" width="50%"/>

<p>6. On the following page, just click NEXT</p>
<p align="center"><img src="https://i.imgur.com/bYESCSD.png" height="50%" width="50%"/>

<p>7. On confirm installation selections, just click on INSTALL and wait for the installation to complete.</p>
<p align="center"><img src="https://i.imgur.com/SMn0bfb.png" height="50%" width="50%"/>

<p>8. After the installation is complete, just click CLOSE</p>
<p align="center"><img src="https://i.imgur.com/8gYVfH9.png" height="50%" width="50%"/>

<br>

<h3>*Configuring DHCP</h3>
<p>1. From the installation progress screen, after the installation is complete, you are shown the option to click on “Complete DHCP configuration”</p>
<p align="center"><img src="https://i.imgur.com/QglwFBC.png" height="50%" width="50%"/>

<p>2. On the description page, click on NEXT</p>
<p align="center"><img src="https://i.imgur.com/UmTL1Z3.png" height="50%" width="50%"/>

<p>3. On the “Specify the credentials to be used to authorize this DHCP server in ADDS” page, click on specify in the ‘use alternate credentials” tab</p>
<p align="center"><img src="https://i.imgur.com/kKZfgku.png" height="50%" width="50%"/>

<p>4. You are then prompted to input the credentials to sign in to the domain, then click OK</p>
<p align="center"><img src="https://i.imgur.com/d2ZZ0eb.png" height="50%" width="50%"/>

<p>5. After the credentials have been recognized, click COMMIT</p>
<p align="center"><img src="https://i.imgur.com/S5KtudL.png" height="50%" width="50%"/>

<p>6. On the following page, click OK </p>
<p align="center"><img src="https://i.imgur.com/6Rn7W7A.png" height="50%" width="50%"/>
  
<p>7. On the Summary page, review your information, then click CLOSE</p>
<p align="center"><img src="https://i.imgur.com/iuaujla.png" height="50%" width="50%"/>

<br>

<h3>*Creating a DHCP Scope</h3>
<p>A DHCP scope is a defined range of IP addresses that a DHCP server can lease to clients within a particular network or subnet.</p>
<p>1. Open Server manager, go to Tools and select DHCP. Then on the DHCP manager screen, expand server and right-click on IPv4 and select New scope.</p>
<p align="center"><img src="https://i.imgur.com/E4bsWQl.png" height="50%" width="50%"/>

<p>2. New scope wizard is opened, just click NEXT</p>
<p align="center"><img src="https://i.imgur.com/kY06w8x.png" height="50%" width="50%"/>

<p>3. You are asked for the Scope name and the description, after that, click NEXT</p>
<p align="center"><img src="https://i.imgur.com/EC4FdsO.png" height="50%" width="50%"/>

<p>4. On the next page, you are asked to specify the IP Address range for the new scope, then click NEXT</p>
<p align="center"><img src="https://i.imgur.com/lOHGDiK.png" height="50%" width="50%"/>

<p>5. The “Add exclusion and delay page is for address you want to exclude from being distributed. You can exclude or decide to leave it, click NEXT</p>
<p align="center"><img src="https://i.imgur.com/YzjJjhU.png" height="50%" width="50%"/>

<p>6. The Lease duration page is next, leave it at 8 days and click NEXT</p>
<p align="center"><img src="https://i.imgur.com/BzOKBlW.png" height="50%" width="50%"/>

<p>7. Next, you are asked to configure DHCP option, select “No, I will configure these options later”, click NEXT</p>
<p align="center"><img src="https://i.imgur.com/uuAWAVI.png" height="50%" width="50%"/>

<p>8. On the completing the new scope wizard, just click FINISH</p>
<p align="center"><img src="https://i.imgur.com/mrRZXTM.png" height="50%" width="50%"/>

<p>9. <b>ACTIVATION</b> - To activate the DHCP scope, right on the scope and select Activate.</p>
<p align="center"><img src="https://i.imgur.com/xb2IpIf.png" height="50%" width="50%"/>

<br>

<h3>*Testing DHCP on a Client</h3>
<p>1.<b> On Windows 10 </b> - Go to Control Panel >Network and Internet > Network and Sharing Center, then click on Ethernet. On the Ethernet status screen, click on properties</p>
<p align="center"><img src="https://i.imgur.com/aOBWKCn.png" height="50%" width="50%"/>

<p>2. On the Ethernet status screen, click on properties</p>
<p align="center"><img src="https://i.imgur.com/aSYjtM2.png" height="50%" width="50%"/>

<p>3. On the Ethernet properties’ screen, select Ipv4 and click properties</p>
<p align="center"><img src="https://i.imgur.com/pwsQEh9.png" height="50%" width="50%"/>

<p>4. While on the IPv4 properties' screen, select Obtain an IP address automatically.</p>
<p align="center"><img src="https://i.imgur.com/tGNwnEV.png" height="50%" width="50%"/>

<p>5. On the computer, opened cmd and typed <b><i>"ipconfig"</i></b>. You will realize that the IP address has been changed to one of the ranges we configure in the new scope.</p>
<p align="center"><img src="https://i.imgur.com/uj0ET1u.png" height="50%" width="50%"/>

<p><b> On Windows 11</b> - I repeated the above steps for computer to obtain an IP address automatically, then opened cmd and typed i<b><i>"ipconfig"</i></b>. Amd it is evident that the IP address has been changed to one of the ranges we configure in the new scope</p>
<p align="center"><img src="https://i.imgur.com/WonCtJf.png" height="50%" width="50%"/>

<br>
