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

Video walkthrough coming soon.
</details>
