
<body>
  <h1>azureSentinelLab</h1>

  <h2>Goal</h2>
  <p>The goal of this project is to develop hands-on experience in Cloud Security, specifically focusing on Azure Virtual Machines and Azure Sentinel.</p>

  <h2>Description</h2>

  <h3>Context</h3>
  <p>In this project, we've set up a live virtual machine acting as a honeypot to visualize RDP (Remote Desktop Protocol) brute force attempts on a map using Azure Sentinel. This allows us to monitor and analyze RDP attacks from various locations around the world.</p>

  <h3>Methodology</h3>
  <p>To achieve this, we utilized a PowerShell script responsible for:</p>
  <ul>
    <li>Parsing Windows Event Log information for failed RDP attacks.</li>
    <li>Utilizing a third-party API to translate IP addresses from Event Logs to the geographic locations of attackers.</li>
  </ul>
  

![Capture d’écran du 2024-05-06 21-58-11](https://github.com/gkounga/azureSentinelLab/assets/99138607/99b9e66a-9832-49ed-b899-184d11ce1600)

 
  <h2>Components</h2>

  <h3>Languages Used</h3>
  <ul>
    <li>PowerShell: Used to extract RDP failed logon logs from the Windows Event Viewer.</li>
  </ul>

  <h3>Utilities Used</h3>
  <ul>
    <li>ipgeolocation.io: Utilized for IP Address to Geolocation API.</li>

![Design sans titre(4)](https://github.com/gkounga/azureSentinelLab/assets/99138607/ff6e8c31-70be-47d7-bd20-d18266a26b75)

    
  </ul>
  
  <h3> Custom Script displaying RDP attacks </h3>

![GetImage(2)](https://github.com/gkounga/azureSentinelLab/assets/99138607/041d29d0-8c26-4a28-aecc-5124dc67b23a)

  <h3> World map of incoming attacks after 24 hours</h3>

 ![GetImage(3)](https://github.com/gkounga/azureSentinelLab/assets/99138607/8c6eb235-0c5a-48fa-b07c-3bb662dc481b)

<p><em>Custom logs including geodata were used to generate this map.</em></p>

</body>

