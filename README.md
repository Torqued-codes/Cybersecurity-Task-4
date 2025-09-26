Cyber Security Internship: Windows Firewall Task :

Task 4: Setup and Use a Firewall on Windows :

i] Objective :

Configure and test basic firewall rules to allow or block traffic on Windows using Windows Defender Firewall.

Steps Performed :
  
- Opened Windows Defender Firewall/
- Accessed through Control Panel and navigated to "Advanced Settings"
- Listed Current Inbound Rules.
- Reviewed existing rules under “Inbound Rules.”
- Created a Rule to Block Inbound Traffic on Port 23 (Telnet)
- New rule: Type = Port, Protocol = TCP, Port = 23, Action = Block, Applied to all profiles.
- Named as “Block Telnet port 23.”
- Tested the Block Rule

Used Python command for connectivity test:

python -m http.server 23

And

python -c "import socket; s=socket.socket(); print(s.connect_ex(('localhost', 23)))"
Connection was still possible, indicating further troubleshooting was needed.

Troubleshooting :

- Double-checked the rule, ensured it was enabled, checked for conflicting allow rules, verified firewall status, and attempted a system restart.
- Added Rule to Allow SSH (Port 22)
- New rule: Type = Port, Protocol = TCP, Port = 22, Action = Allow, All profiles.
- Named as “Allow SSH port 22.”
- Restored Firewall State
- Disabled or deleted the block rule for port 23.

Summary =  How Firewall Filters Traffic :

Configured firewall rules act as filters at the OS boundary, controlling which network connections are allowed or denied based on protocol type, port, or application. By blocking Telnet (port 23), potential remote attacks using an insecure protocol are prevented. By allowing SSH (port 22), secure remote management is enabled. These actions strengthen security by exposing only trusted services and reducing attack surface.







