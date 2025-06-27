# TASK-4: Setup and use a firewall on Windows/Linux


1) Task Overview
This task is part of a cybersecurity internship focused on practical network security configurations. The goal was to understand how to configure firewall rules on a Windows operating system and block specific traffic based on port-level filtering.

2) Objective
- Configure basic firewall rules using **Windows Defender Firewall**.
- Block **inbound traffic on port 23 (Telnet)** on Windows.
- Verify firewall behavior by attempting a connection test.
- Gain hands-on experience with GUI-based firewall rule creation and validation.

3) Tools Used
- Windows 10
- Windows Defender Firewall with Advanced Security
- Command Prompt (Telnet Test)

4) Steps Performed
 a. **Opened the Windows Firewall with Advanced Security**  
   Accessed via Run → `wf.msc`.
 b. **Viewed existing Inbound Rules**  
   Inspected current rules to understand the default configuration.
 c. **Created a New Inbound Rule**
   - Protocol: TCP  
   - Port: 23 (Telnet)  
   - Action: **Block the connection**  
   - Profile: All (Domain, Private, Public)  
   - Named as: `Telnet-Port-23-Block`
 d. **Tested using Telnet Command**
   - Used the command: `telnet 127.0.0.1 23`  
   - Result: **Connection failed**, confirming the block rule worked.
 e. **Verified the Rule**
   - Confirmed the custom block rule was active under inbound rules.

6) Screenshots

- Firewall Overview: ![Win 10- 1](https://github.com/user-attachments/assets/fe7376e5-b431-4215-9f51-d04713df265a) 
- Inbound Rules View: ![Win 10- 2](https://github.com/user-attachments/assets/74b4a0da-8b35-485b-8a8f-c312553fd051) 
- New Rule Setup: ![Win 10- 3](https://github.com/user-attachments/assets/2b5d2122-7741-415d-ba47-85b4a33a0c93) 
- Telnet Block Test: ![Win 10- result](https://github.com/user-attachments/assets/5399d62a-17df-49b8-b412-03c1c3487ec0)  
- Rule Confirmation: ![Win 10- telnet block](https://github.com/user-attachments/assets/c70fda70-95ec-4e2d-87bb-28aac0bf9926) 

7) Key Findings

- A custom firewall rule can effectively block targeted network traffic using port numbers.
- Windows Defender Firewall provides a user-friendly GUI to define security policies.
- Telnet is often blocked in secure environments due to its unencrypted nature.
- Real-time testing (e.g., Telnet) is a good way to confirm firewall effectiveness.

8) Key Concepts Learned

- Inbound vs Outbound Rules: Directional control of traffic based on origin/destination.
- Port-Based Filtering: Specific traffic can be blocked by defining port rules.
- Protocol Awareness: TCP/UDP protocols must be specified when configuring rules.
- GUI Firewall Management: Understanding how to navigate and configure firewall rules using Windows Defender.
- Telnet as a Security Risk: Why Telnet is disabled/blocked in modern networks.


