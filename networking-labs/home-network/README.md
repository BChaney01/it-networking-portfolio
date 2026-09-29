Home Network Connectivity & DNS Troubleshooting Lab
Objective
The goal of this lab was to investigate my Mac's network configuration and test connectivity between my computer, my local router, and the Internet.
Environment
Device: MacBook Air
Operating System: macOS
Shell: Zsh
Tools used: ipconfig, route, ping, nslookup
Network Information
My Mac's private IP address was:
10.0.0.162

My default gateway was:

10.0.0.1

My subnet mask was:

255.255.255.0

This corresponds to a /24 network.

Network:

10.0.0.0/24

Broadcast address:

10.0.0.255

Connectivity Test 1 — Default Gateway
I tested connectivity between my Mac and the default gateway using:
ping -c 4 10.0.0.1

Result
Packets transmitted: 4
Packets received: 4
Packet loss: 0%
Average round-trip time: 11.425 ms
Conclusion
My Mac successfully communicated with the local router.
Connectivity Test 2 — Internet
I tested Internet connectivity using Google's public DNS server:
ping -c 4 8.8.8.8

Result
Packets transmitted: 4
Packets received: 4
Packet loss: 0%
Average round-trip time: 24.294 ms
Conclusion
My Mac successfully reached a destination outside the local network.
DNS Test
I tested DNS name resolution using:
nslookup google.com

The lookup returned multiple IP addresses for google.com.
Conclusion
DNS name resolution was functioning successfully.
Troubleshooting Methodology
I followed a basic troubleshooting process:
Identify the computer's IP address.
Identify the default gateway.
Test connectivity to the gateway.
Test connectivity to an Internet destination.
Test DNS resolution.
What I Learned
Through this lab, I practiced:
Identifying a private IP address.
Identifying a default gateway.
Understanding subnet masks and /24 networks.
Using ping to test connectivity.
Understanding packet loss and round-trip time.
Using nslookup to test DNS.
Documenting network troubleshooting steps and results.
