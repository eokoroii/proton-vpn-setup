<h1>Proton VPN Setup &amp; IP Address Testing</h1>

<h2>Project Summary</h2>
<p>
  In this lab, I used Proton VPN on a Windows VM to explore how connecting via 
  different VPN servers changes my public IP and potentially impacts region-based website content. 
  I tested multiple server locations and confirmed each assigned IP address through 
  <em>whatismyipaddress.com</em>.
</p>

<ul>
  <li><strong>Focus Areas:</strong>
    <ul>
      <li>Public IP identification</li>
      <li>VPN installation &amp; account setup</li>
      <li>Testing website differences when changing IP/country</li>
    </ul>
  </li>
  <li><strong>Tools &amp; Services:</strong>
    <ul>
      <li>Azure Windows VM or local Windows machine</li>
      <li>Proton VPN client</li>
      <li>Web browser checks (Google, Disney, etc.)</li>
    </ul>
  </li>
</ul>

<hr />

<h2>Steps & Screenshots</h2>
<ol>
  <li>
    <strong>Check Baseline Public IP</strong><br />
    I navigated to <a href="https://www.whatismyipaddress.com" target="_blank">whatismyipaddress.com</a> 
    to note my current public IP. This gave me a baseline to compare once the VPN was activated.
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/FjHfcWZ.png" alt="Baseline IP check" width="600" />
      <br />
      <em>Figure VPN.1 – Initial public IP before VPN use.</em>
    </p>
  </li>
  <br />

  <li>
    <strong>Create Proton Account &amp; Download Client</strong><br />
    I signed up for a Proton VPN account at <a href="https://protonvpn.com" target="_blank">protonvpn.com</a> 
    (free tier for this demo) and downloaded the Windows client installer.
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/l4T1TjO.png" alt="ProtonVPN site" width="600" />
      <br />
      <em>Figure VPN.2 – Proton VPN official website.</em>
    </p>
  </li>
  <br />

  <li>
    <strong>Install &amp; Launch Proton VPN</strong><br />
    After running the installer on my VM, I logged in with my newly created account. 
    The dashboard displays available servers around the world.
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/R7ehCke.png" alt="Proton VPN installation" width="600" />
      <img src="https://i.imgur.com/gFVKkQT.png" alt="Proton VPN installation" width="600" />
      <br />
      <em>Figure VPN.3 – Proton VPN client post-installation.</em>
    </p>
  </li>
  <br />

  <li>
    <strong>Websites Before VPN</strong><br />
    I visited <code>google.com</code> and <code>disney.com</code> to note any region-specific content. 
    This helps detect changes once I connect to a VPN server in a different location.
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/wDt3Gl3.png" alt="Google pre-VPN" width="600" />
      <br />
      <em>Figure VPN.4 – Google’s page prior to VPN usage.</em>
      <br /><br />
      <img src="https://i.imgur.com/NOluxy6.png" alt="Disney pre-VPN" width="600" />
      <br />
      <em>Figure VPN.5 – Disney’s site looks standard without VPN changes.</em>
    </p>
  </li>
  <br />

  <li>
    <strong>Connect to Proton VPN &amp; Recheck IP</strong><br />
    I picked a server in another country and clicked <em>Connect</em>. 
    Returning to <em>whatismyipaddress.com</em> now showed a new public IP, 
    often in the assigned server’s location.
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/k01wEiw.png" alt="Proton VPN connected" width="600" />
      <br />
      <em>Figure VPN.6 – Confirming connection to a foreign server.</em>
      <br /><br />
      <img src="https://i.imgur.com/tFo0EcY.png" alt="New IP from VPN" width="600" />
      <br />
      <em>Figure VPN.7 – My public IP now shows the VPN’s location.</em>
    </p>
  </li>
  <br />

  <li>
    <strong>Websites After VPN</strong><br />
    Finally, with the VPN active, I reloaded <code>google.com</code> and <code>disney.com</code>. 
    Depending on the server location, I occasionally saw content in another language or different 
    region-based services. This highlights how easily the VPN changes your perceived location. 
    <br /><br />
    <p align="center">
      <img src="https://i.imgur.com/Ijz8vyx.png" alt="Disney after VPN" width="600" />
      <img src="https://i.imgur.com/cvpiAqe.png" alt="Google after VPN" width="600" />
      <br />
      <em>Figure VPN.8 – Google potentially serving a localized site.</em>
    </p>
  </li>
  <br />
</ol>

<hr />

<h2>Conclusion</h2>
<p>
  By using Proton VPN, I illustrated how connecting to different servers changes 
  your external IP address and can influence localized content on websites. 
  This lab underscores VPN benefits (e.g., privacy, bypassing regional restrictions) 
  and the importance of understanding how public IP location can affect your browsing experience.
</p>
