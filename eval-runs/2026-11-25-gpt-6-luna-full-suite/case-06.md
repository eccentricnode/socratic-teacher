Model: openai-codex/gpt-6-luna
Pi: 1.6.0
Extensions: disabled
Auto skill discovery: disabled; only Socratic Teacher explicitly loaded
Context files: disabled
Tools: read,bash,write,edit (write enabled)
Each scenario: fresh temporary workspace/session; case 9 is a two-turn dialogue in one fresh session
Case 8A: actual ASU plan plus synthetic eval-only Topic 1-complete progress fixture; case 8B: actual plan only
UTC: 2026-11-25T02:43:33.575914+00:00

Prompt: I want to learn networking so I can troubleshoot my home network. I’m a beginner and don’t have source material. Help me make a learning plan.
Exit code(s): [0]
Unexpected workspace files: []

Exit: 0
# Learning Plan: Home Networking Troubleshooting

**Source:** AI-generated curriculum  
**Goal:** Build enough understanding to diagnose common home-network problems, isolate where they occur, and choose safe next steps.  
**Concepts:** 7  
**Assumed knowledge:** No networking experience. I’ll assume you can use a computer or phone and access your home router’s settings if needed. The plan uses practical examples and free built-in tools; no special equipment is required.

## Concept Sequence

### 1. How a home network fits together
**Core idea:** Your devices connect through Wi‑Fi or Ethernet to a router, which usually connects to a modem or internet gateway and then to your internet provider.  
**Why it matters:** Knowing the path helps narrow down where a connection problem starts.  
**Exit criteria:**
- **Explain:** Describe the route from a device to an internet service.
- **Apply:** Given a simple network diagram, identify the likely section to investigate when one device or all devices lose internet.
- **Tradeoffs:** Compare Wi‑Fi and Ethernet for reliability and convenience.
- **Connect:** Relate each piece of equipment to the connection path.

### 2. Local connections, IP addresses, and DHCP
**Depends on:** Concept 1  
**Core idea:** Devices need local network addresses; routers commonly assign those addresses automatically using DHCP.  
**Why it matters:** Addressing problems can prevent a device from communicating even when Wi‑Fi appears connected.  
**Exit criteria:**
- **Explain:** Describe what a local IP address is and what DHCP does.
- **Apply:** Use a device’s network settings to identify its IP address and default gateway.
- **Tradeoffs:** Explain why automatic addressing is convenient, and when a manually assigned address might be useful or risky.
- **Connect:** Explain how a device’s address helps it communicate through the router.

### 3. Wi‑Fi basics and signal problems
**Depends on:** Concept 1  
**Core idea:** Wi‑Fi is a radio connection whose performance depends on signal strength, distance, obstacles, interference, and settings.  
**Why it matters:** A weak or unstable wireless link can look like an internet outage.  
**Exit criteria:**
- **Explain:** Identify several factors that can weaken or disrupt Wi‑Fi.
- **Apply:** Propose a safe test to distinguish a Wi‑Fi problem from a broader internet problem.
- **Tradeoffs:** Compare moving the router, changing Wi‑Fi settings, and adding equipment.
- **Connect:** Relate Wi‑Fi quality to the device’s local connection, before considering the internet provider.

### 4. DNS and finding services by name
**Depends on:** Concept 2  
**Core idea:** DNS translates human-readable names, such as website addresses, into IP addresses computers can use.  
**Why it matters:** Some problems affect name lookup while other network communication still works.  
**Exit criteria:**
- **Explain:** Describe DNS’s role without confusing it with Wi‑Fi or internet access itself.
- **Apply:** Interpret a simple scenario where a site fails by name but other connectivity appears available.
- **Tradeoffs:** Explain why changing DNS settings may help in some cases but is not a universal fix.
- **Connect:** Relate DNS lookup to a device’s IP connectivity.

### 5. A step-by-step troubleshooting method
**Depends on:** Concepts 1–4  
**Core idea:** Check symptoms, compare devices, and test one layer at a time, starting with the simplest and safest checks.  
**Why it matters:** A consistent process avoids guesswork and unnecessary resets or purchases.  
**Exit criteria:**
- **Explain:** Describe why changing one thing at a time makes troubleshooting clearer.
- **Apply:** Work through a case where one device cannot connect but others can.
- **Tradeoffs:** Decide when to keep investigating locally versus contact the internet provider.
- **Connect:** Use the connection path, addressing, Wi‑Fi, and DNS concepts to justify a test order.

### 6. Basic network tools and interpreting results
**Depends on:** Concepts 2, 4, and 5  
**Core idea:** Built-in settings and tools can reveal whether a device has an address, can reach the router, and can reach other destinations.  
**Why it matters:** Evidence helps locate the failure instead of relying on a vague “internet is down” symptom.  
**Exit criteria:**
- **Explain:** Describe what a connectivity test can and cannot tell you.
- **Apply:** Choose an appropriate built-in check for a given symptom and interpret a simple result.
- **Tradeoffs:** Compare quick, low-risk checks with more advanced tools that may need extra care.
- **Connect:** Relate test results to the network layers and path from earlier concepts.

### 7. Router settings, safe changes, and escalation
**Depends on:** Concepts 1–6  
**Core idea:** Router settings affect the whole home network, so changes should be deliberate, reversible, and documented.  
**Why it matters:** Safe handling prevents a troubleshooting attempt from creating a larger outage or weakening security.  
**Exit criteria:**
- **Explain:** Identify why router changes can affect multiple devices.
- **Apply:** Make a safe troubleshooting plan that records the current state and includes a way to undo a change.
- **Tradeoffs:** Decide when a router restart, settings change, or provider support is the sensible next step.
- **Connect:** Use evidence from earlier checks to explain what information to give a support technician.

## Gaps

- Advanced router configuration, VLANs, port forwarding, and firewall rules.
- Mesh-network design and detailed Wi‑Fi channel planning.
- Packet capture and enterprise networking.
- These can be added later if your troubleshooting needs grow.

Please review the plan and either approve it or request changes. If you approve, which exact folder should hold the plan and progress files? I won’t create either file until you approve the plan and specify the destination.
