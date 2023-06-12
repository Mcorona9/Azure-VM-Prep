
# Setting up Vulnerable VMs in Azure
<p align="center">
<img src="https://i.imgur.com/s9Ec1cp.png" alt="Traffic Examination"/>
</p>

<h1> </h1>
<br />




<h2>To initiate the Azure Honeynet project, the first step is to set up the virtual machines (VMs) that will be utilized. VMs serve as cloud-based computers and will establish the core infrastructure of our honeynet. The following steps outline the process in Microsoft Azure:</h2>






<p>
<img src="https://i.imgur.com/MQciqs4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
""
</p>
<br />

<p>
<img src="https://i.imgur.com/QqnCgFD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/njMCUxk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<img src="https://i.imgur.com/ANimQkA.png" alt="Disk Sanitization Steps"/>
</p>
<p>
"</p>
<br />

<p>
<img src="https://i.imgur.com/F7Cbt7P.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p> <b>
"Configuration of Inbound Security Rule for NSG:
To configure the inbound security rule for your Network Security Group (NSG), follow these steps:

Access the NSG: Open the Azure portal and use the search bar at the top to find and select "Network Security Groups." Locate and choose the NSG associated with your virtual machine.

Create a new inbound security rule: Within the NSG settings, navigate to the "Inbound security rules" section. Click on the "Add" button to initiate the creation of a new rule.

Rule configuration: You will be prompted to provide specific details for the new rule. Let's go through each parameter:

Source: Specify the source of incoming traffic. To allow traffic from any location, set it to "Any."

Source port ranges: Define the allowed ports on the source (the initiating computer). To permit all ports, you can set it to "*" or "Any."

Destination: Determine where the traffic is intended to go. Since we want the traffic to reach our VM, set it to "Any."

Destination port ranges: Specify the ports on the VM that are permitted to receive traffic. To open all ports, set it to "*" or "Any."

Priority: Setting priorities in NSGs is crucial as it determines the order in which rules are applied. Lower priority numbers take precedence over higher ones. For this lab, let's set the priority to 300 to ensure the effective functioning of the honeypot.

Action: Set the action to "Allow" to permit traffic that matches this rule to reach the VM.

By following these steps, you can configure the inbound security rule for your NSG effectively. </p>
<br />






