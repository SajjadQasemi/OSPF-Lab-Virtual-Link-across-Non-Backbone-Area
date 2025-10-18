# OSPF-Lab-Virtual-Link-across-Non-Backbone-Area
A hands-on lab demonstrating OSPF backbone reachability using a virtual link. Step-by-step topology, practical Cisco IOS config examples, verification commands, and troubleshooting tips — perfect for network engineers, students preparing for CCNA/CCNP, or anyone learning OSPF design
🚀 Highlights
Clear multi-area OSPF topology with Area 0, Area 2, NSSA (Area 3), and a non-backbone Area (Area 10) connected via a virtual link.
Complete configuration examples for router interfaces and OSPF process (virtual link creation).
Verification commands and troubleshooting tips.
Accompanying step-by-step video tutorial on YouTube.(computer scienceکمپیوتر ساینس)

🛠️ Prerequisites
Basic familiarity with Cisco IOS (or similar vendor) CLI.
Packet Tracer / GNS3 / EVE-NG for lab deployment (recommended).
Routers with OSPF support.

🔍 Verification & Useful Commands
show ip ospf neighbor
show ip ospf virtual-links
show ip ospf
show ip route (confirm routes from the remote area are in the RIB)
debug ip ospf adj (use carefully in lab only)

🛑 Troubleshooting Tips
Virtual links require OSPF adjacency across the transit area — the transit area must be configured on intermediate routers and not be a stub.
Ensure router IDs are unique.
Use show ip ospf database to confirm LSAs and the virtual link’s LSAs.
If adjacency won’t form, check MTU mismatches, hello/dead timers, and authentication mismatch.
🎥 Video Tutorial

A full, narrated step-by-step walkthrough is available on YouTube — (https://www.youtube.com/channel/UCAvnuCGBgYjizY3lCZ7Brrw?sub_confirmation=1). The video shows topology setup, full config on each router, verification and troubleshooting.


⭐ If you like this lab
Star this repo ⭐
Follow me for more networking labs and step-by-step tutorials
Watch and subscribe to the YouTube walkthrough (link in this repo)

License
Feel free to reuse these configs and topology for study. If you publish derivative content, a short attribution is appreciated.
Enjoy the lab — and let me know if you want additional variants (e.g., with authentication, LSA filtering, or OSPF summarization)!![pic](https://github.com/user-attachments/assets/8d59b23f-79a7-435b-b7ad-5f6614f3329c)
