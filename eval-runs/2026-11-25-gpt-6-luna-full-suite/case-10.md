Model: openai-codex/gpt-6-luna
Pi: 1.6.0
Extensions: disabled
Auto skill discovery: disabled; only Socratic Teacher explicitly loaded
Context files: disabled
Tools: read,bash,write,edit (write enabled)
Each scenario: fresh temporary workspace/session; case 9 is a two-turn dialogue in one fresh session
Case 8A: actual ASU plan plus synthetic eval-only Topic 1-complete progress fixture; case 8B: actual plan only
UTC: 2026-11-25T02:43:33.575914+00:00

Prompt: Create a learning plan for networking. My goal is to troubleshoot my home network; I’m a beginner and have no source material.
Exit code(s): [0]
Unexpected workspace files: []

Exit: 0
# Learning Plan: Home Network Troubleshooting

**Source:** AI-generated curriculum  
**Goal:** Troubleshoot common home network problems, such as devices failing to connect, slow or unreliable Wi‑Fi, and loss of internet access.  
**Concepts:** 7  
**Assumed knowledge:** Beginner; no networking knowledge or source material assumed. I’ve assumed a practical, hands-on learning style and no special time constraints.

## Concept Sequence

### 1. How a home network fits together
**Core idea:** Devices communicate through a local network, typically using a router and Wi‑Fi access point, while the router connects that network to the internet through a modem or gateway.  
**Why it matters:** Knowing the basic layout helps narrow down where a problem might be.

**Exit criteria:**
- **Explain:** Describe how a device’s traffic reaches a website through a home network.
- **Apply:** Sketch a simple home setup and identify the router, internet connection, and connected devices.
- **Tradeoffs:** Explain why a combined modem-router is convenient and what can make it harder to troubleshoot.
- **Connect:** Relate the network’s layout to where you would look if one device loses internet access.

### 2. The connection path: Wi‑Fi, Ethernet, and local connectivity
**Depends on:** Concept 1  
**Core idea:** A device can connect to the home network over Wi‑Fi or Ethernet; being connected to the local network is different from having internet access.  
**Why it matters:** This separates wireless or local-network faults from problems farther upstream.

**Exit criteria:**
- **Explain:** Distinguish a Wi‑Fi connection, a local network connection, and an internet connection.
- **Apply:** Given that one wired device works but one wireless device does not, identify what the evidence suggests.
- **Tradeoffs:** Compare Wi‑Fi and Ethernet for reliability, convenience, and troubleshooting.
- **Connect:** Use the connection path from Concept 1 to pinpoint where a failure could occur.

### 3. IP addresses and DHCP
**Depends on:** Concept 2  
**Core idea:** Devices need network addresses to communicate; home routers commonly assign those addresses automatically using DHCP.  
**Why it matters:** Addressing problems can prevent a device from communicating even when it appears connected to Wi‑Fi.

**Exit criteria:**
- **Explain:** Describe the purpose of an IP address and what DHCP does.
- **Apply:** Interpret basic device network details—such as its IP address and gateway—to spot a likely address-assignment problem.
- **Tradeoffs:** Explain why automatic addressing is easier to manage than manually assigning addresses, and when manual settings can cause trouble.
- **Connect:** Relate a device’s address and gateway to its ability to reach the router and the internet.

### 4. DNS and reaching websites
**Depends on:** Concept 3  
**Core idea:** DNS translates website names into addresses that devices can use to connect.  
**Why it matters:** A device may have internet connectivity but still fail to open websites if name lookup is failing.

**Exit criteria:**
- **Explain:** Describe the difference between reaching an address and looking up a website name.
- **Apply:** Reason through a case where some internet-connected apps work but websites do not.
- **Tradeoffs:** Explain why changing DNS settings might help in some cases but shouldn’t be the first fix for every outage.
- **Connect:** Trace how a device’s IP configuration and DNS work together when opening a website.

### 5. Wi‑Fi signal, interference, and placement
**Depends on:** Concept 2  
**Core idea:** Wi‑Fi performance depends on signal strength, distance, obstacles, interference, and the router’s radio settings.  
**Why it matters:** Slow or unreliable Wi‑Fi often has a local, physical cause rather than an internet-provider issue.

**Exit criteria:**
- **Explain:** Describe how distance and obstacles can affect a Wi‑Fi connection.
- **Apply:** Propose a simple test to distinguish a coverage problem from a broader internet problem.
- **Tradeoffs:** Explain the practical tradeoffs of router placement, using different Wi‑Fi bands, and adding an extender.
- **Connect:** Use the difference between local connectivity and internet access (Concept 2) to interpret a weak-signal symptom.

### 6. A systematic troubleshooting method
**Depends on:** Concepts 1–5  
**Core idea:** Troubleshooting works best when you define the symptom, compare affected devices, test one layer at a time, and change one thing at a time.  
**Why it matters:** A repeatable method helps avoid random resets and makes it easier to identify the real cause.

**Exit criteria:**
- **Explain:** Describe a step-by-step approach that moves from the affected device toward the internet connection.
- **Apply:** Given a realistic outage, choose tests in a sensible order and say what each result would tell you.
- **Tradeoffs:** Explain when rebooting equipment is a reasonable test and why repeated reboots or multiple simultaneous changes can obscure the cause.
- **Connect:** Use IP, DNS, Wi‑Fi, and network-layout clues from earlier concepts to narrow a fault.

### 7. Common fixes, safe changes, and when to escalate
**Depends on:** Concept 6  
**Core idea:** Some problems are safe to fix at home; others require careful configuration or help from the router manufacturer or internet provider.  
**Why it matters:** Good troubleshooting includes knowing how to recover from a change and when not to make one.

**Exit criteria:**
- **Explain:** Identify the difference between restarting equipment and resetting it to factory defaults.
- **Apply:** Create a safe action plan for a recurring home-network problem, including what information to collect before contacting support.
- **Tradeoffs:** Explain the risks of changing router settings versus leaving them alone, and when escalation is preferable.
- **Connect:** Use the troubleshooting results from Concept 6 to decide whether the likely fault is in the home network or beyond it.

## Gaps
- Advanced router configuration, VLANs, firewall rules, and port forwarding.
- Network monitoring tools and packet analysis.
- Mesh-system design and detailed Wi‑Fi channel planning.

Would you review and approve this plan, or request changes—and which exact folder should hold the plan and progress files?
