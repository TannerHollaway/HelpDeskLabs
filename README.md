# HelpDeskLabs

A collection of hands-on IT helpdesk labs completed through ServiceDesk Simulator. 
Each entry includes a written breakdown of the scenario, tools used, and resolution process.

---

<details>
<summary>00 — Tool Familiarization | ServiceDesk Simulator</summary>

Before responding to any tickets, I spent time exploring the ServiceDesk Simulator 
environment to understand the tools available to me. In a real helpdesk role, knowing 
where to find information and how to navigate your environment is just as important as 
knowing how to solve the problem.

## Dashboard
The central hub for navigating the entire environment. Provides access to all sections 
including devices, documentation, analytics, and remote tools.

## Devices Section
Lists all endpoints and workstations in the simulated network, organized by user and 
department (Finance, Sales, HR, Engineering). Used to identify affected systems when 
working a ticket.

## Device Details Panel
Displays per-device information including usernames, departments, IP addresses, and 
assigned systems. Essential for verifying scope during an incident.

## Network Topology Map
A visual representation of the simulated network including routers, firewalls, switches, 
endpoints, and the ISP connection. Used to understand traffic flow and identify where 
a network issue may originate.

- **Router Node** — Handles traffic routing between internal networks and external connections
- **Firewall Node** — Filters and protects internal traffic
- **Switch Nodes** — Distribute traffic to department systems
- **Endpoint/Workstation Nodes** — Represent user machines connected to the network
- **ISP Connection Node** — Represents the simulated internet entry point

## Remote Desktop Tool
Allows remote access into any workstation on the network. Used to directly troubleshoot 
and resolve issues on end-user machines without physical access.

## Documentation Station
The central knowledge base for the environment. In a real helpdesk role, this is where 
you go before making changes — to verify configurations, follow SOPs, and avoid guessing.

- **Email Exchange Documentation** — Exchange server config, SMTP relay settings, ActiveSync, and OWA
- **Password & Security Documentation** — Password policies and security procedures
- **Network & Connectivity Documentation** — Network configuration and connectivity details
- **Server Documentation** — Server setup and operational data
- **Standard Procedures (SOPs)** — Internal workflows for common IT tasks
- **Software & Licensing Documentation** — Installed software and license tracking
- **Hardware & Assets Documentation** — Hardware inventory records
- **Contacts & Escalation Documentation** — Escalation paths and key contacts
- **Credentials & Access Documentation** — System login credentials and access info

## Exchange Server Configuration
Detailed view of the Exchange mail server including protocols, ports, OS version, SMTP 
relay settings, ActiveSync configuration, and OWA access. Referenced when troubleshooting 
email-related tickets.

## Analytics Section
Provides metrics and monitoring data for the simulated environment. Useful for identifying 
trends or recurring issues across the network.

## Search Function
Allows quick searching across all documentation, SOPs, and credential records. Saves time 
when working a ticket under pressure.

---

[Video of me quickly going through the documents](https://www.youtube.com/watch?v=Lgfva49Im_E)

</details>
<details>
<summary>01 — Email Server Degraded | ServiceDesk Simulator</summary>
A ticket came in reporting that no one in the building had email access. Users were experiencing failed or delayed email delivery with Outlook showing a "Disconnected" status. The goal was to identify the root cause, resolve it, and confirm restoration with the affected user.
Tools Used

Ticket Dashboard
Documentation Station (Exchange Server Configuration)
Server Room
Internal Messaging

Process
1. Reviewed the Ticket
Opened the active incident from the ticket queue and read through the issue details. The ticket indicated degraded email server performance affecting multiple users.
2. Referenced Documentation
Opened the Documentation Station and navigated to the Email/Exchange section. Reviewed the Exchange Server configuration document to understand the mail infrastructure before taking any action.
3. Communicated with the User
Opened the internal messaging panel and made contact with the affected user to gather more detail and set expectations.

Technician: Hello, this is Dakota and I'll be helping you out today.

User: Hey Dakota, thanks for helping! I'm still having trouble with my email. It says "Disconnected," and I can't send or receive anything.

Technician: And from my understanding others are also having this issue?

User: Yeah, that's right! Everyone seems to be having the same problem. It's pretty frustrating since I've got some deadlines coming up.

Technician: Okay, please give me one moment while I check into this for you.

User: Sure thing, take your time! Thanks for looking into it.

4. Identified and Resolved the Issue
Opened the Server Room management interface and located the Exchange/email infrastructure. Restarted the Exchange email server from the Server Room interface and confirmed the action through the system prompt.
5. Confirmed Resolution
Returned to the ticket and followed up with the user to verify email was restored.

Technician: Thank you so much for waiting. Could you please confirm if your issues has been solved?
User: Oh, it's all working again, really appreciate the quick fix! Thank you!
Technician: Of course.

6. Closed the Ticket
Selected the resolution action on the ticket dashboard and confirmed closure. Ticket status updated to "Solution Complete."
Outcome
Email service was restored for all affected users. The issue was resolved by restarting the Exchange email server from the Server Room interface. User confirmed full functionality before the ticket was closed.

[Video Walkthrough](https://youtu.be/GNrkLXhD00o)
</details>

<details>
<summary>02 — Suspicious Promotion Request | ServiceDesk Simulator</summary>

A ticket came in from a user claiming they had been promoted and needed to be added to 
the Management group immediately. The request appeared pre-justified with references to 
HR approval, VP sign-off, and business urgency. Despite this, the ticket raised several 
red flags before any action was taken.

## Tools Used
- Ticket Dashboard
- Documentation Station
- External Consultation (Claude)
- Hint System

## Why It Was Suspicious

At first glance the ticket looked routine, but several details stood out:

- **The requester submitted their own promotion ticket** — legitimate promotions are typically initiated by HR or a manager, not the employee themselves
- **Multiple authority claims with no verification path** — the ticket referenced HR approval, an official email, and VP sign-off, but none of it was attached or verifiable through the system
- **Urgency pressure** — phrases like "effective immediately" and "team waiting on approvals" are classic social engineering tactics used to rush technicians into skipping verification steps
- **High privilege request** — adding someone to a Management group grants access to budget reports, purchase approvals, and team management tools — not something to act on without a clear process

## Process

**1. Reviewed the Ticket**
Opened the ticket and immediately noted the unusual framing. The request was self-reported by the employee claiming the promotion, not submitted through HR or a manager.

**2. Checked Documentation**
Opened the Documentation Station and searched for a promotion or group access change policy. No documentation existed for this process, which removed any SOP to follow.

**3. Consulted an External Source**
Pasted the ticket contents to Claude and asked whether the request was legitimate. The response flagged it as suspicious based on the self-reported nature of the request, unverifiable approval claims, and urgency language.

**4. Used the Hint System**
With no policy to reference and a strong suspicion the request was not legitimate, the hint system was consulted. The hint indicated to complete the ticket as written.

**5. Closed the Ticket**
Completed the ticket per the simulator's intended resolution.

## Takeaway
In a real environment, this ticket would not have been actioned without direct confirmation from HR or the requester's manager through a verified channel — not based on claims made within the ticket itself. Tickets that self-justify with urgency and authority references are a common vector for privilege escalation through social engineering. The correct real-world response would be to pause, escalate, and verify before making any group membership changes.

---

*Video walkthrough coming soon.*

</details>
