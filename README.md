## Cyber Security Task 4 : Windows Firewall Task (on windows) :

## i] Objective :

Configure and test basic firewall rules to allow or block traffic on Windows using Windows Defender Firewall.

# Steps Performed :
  
- Opened Windows Defender Firewall/
- Accessed through Control Panel and navigated to "Advanced Settings"
- Listed Current Inbound Rules.
- Reviewed existing rules under “Inbound Rules.”
- Created a Rule to Block Inbound Traffic on Port 23 (Telnet)
- New rule: Type = Port, Protocol = TCP, Port = 23, Action = Block, Applied to all profiles.
- Named as “Block Telnet port 23.”
- Tested the Block Rule

# Screenshots :

## Block Telnet Port 23
<img width="1919" height="445" alt="Image" src="https://github.com/user-attachments/assets/293b6471-fa3a-4239-a091-1edfd48f1f85" />


## Python Commands
<img width="891" height="37" alt="Image" src="https://github.com/user-attachments/assets/1df3ec3d-dab1-4caa-983d-51ba591ed1a9" />


<img width="389" height="37" alt="Image" src="https://github.com/user-attachments/assets/8b1c3bb0-a8e0-43ce-b1bb-2348ae75c3fe" />


## SSH Port 22
<img width="1919" height="505" alt="Image" src="https://github.com/user-attachments/assets/637e3670-05eb-4486-80c0-f884381485cf" />

# Troubleshooting :

- Double-checked the rule, ensured it was enabled, checked for conflicting allow rules, verified firewall status, and attempted a system restart.
- Added Rule to Allow SSH (Port 22)
- New rule: Type = Port, Protocol = TCP, Port = 22, Action = Allow, All profiles.
- Named as “Allow SSH port 22.”
- Restored Firewall State
- Disabled or deleted the block rule for port 23.

# Summary =  How Firewall Filters Traffic :

Configured firewall rules act as filters at the OS boundary, controlling which network connections are allowed or denied based on protocol type, port, or application. By blocking Telnet (port 23), potential remote attacks using an insecure protocol are prevented. By allowing SSH (port 22), secure remote management is enabled. These actions strengthen security by exposing only trusted services and reducing attack surface.







