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

*Video walkthrough coming soon.*

</details>
