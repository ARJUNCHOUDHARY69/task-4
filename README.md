Interview Questions:
Outcome: Basic firewall management skills and understanding of network traffic filtering.

1. What is a firewall?
A firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It acts as a barrier between a trusted internal network and untrusted external networks, like the internet.

2. Difference between stateful and stateless firewall?

Feature           | Stateless Firewall                     | Stateful Firewall
------------------|-----------------------------------------|-------------------------------
Traffic Tracking  | Does not track connection state         | Tracks the state of connections
Rules             | Each packet is evaluated independently  | Decisions based on traffic context
Performance       | Generally faster                        | Slightly slower, more resource use
Use Case          | Simple filtering                        | Complex enterprise filtering

3. What are inbound and outbound rules?
- Inbound rules control traffic coming into a network or device from external sources.
- Outbound rules control traffic leaving a network or device to external destinations.

4. How does UFW simplify firewall management?
UFW (Uncomplicated Firewall) is a frontend for iptables that simplifies firewall configuration on Linux systems. It provides:
- Easy commands (e.g., `ufw allow 22`)
- Default policies
- Simple syntax for adding/removing rules
- Status checking with `ufw status`

5. Why block port 23 (Telnet)?
- Telnet transmits data, including passwords, unencrypted.
- Vulnerable to sniffing and interception.
- Replaced by SSH (port 22) for secure remote access.
- Blocking reduces risk of unauthorized access.

6. What are common firewall mistakes?
- Too permissive rules
- Lack of regular rule auditing or updates
- Misconfigured or open unnecessary ports
- No logging or monitoring
- Not using a "deny by default" policy
- Ignoring outbound traffic rules

7. How does a firewall improve network security?
- Blocks unauthorized access
- Filters malicious or suspicious traffic
- Enforces access control policies
- Logs traffic for anomaly detection
- Limits exposure of internal systems

8. What is NAT in firewalls?
NAT (Network Address Translation) allows multiple devices on a private network to share a single public IP address. In firewalls:
- SNAT (Source NAT): Used for outbound traffic; hides internal IPs.
- DNAT (Destination NAT): Used for port forwarding; redirects traffic to internal devices.
- Provides security by masking internal network details.
