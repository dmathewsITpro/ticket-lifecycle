<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>🗂️ Ticket Lifecycle Stages Detailed</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

### 1. 🎫 Intake (Ticket Creation by End Users)
- End User Portal: `http://localhost/osTicket`
- Created sample tickets representing real-world scenarios:
  - **Critical Outage:** Mobile/Online Banking system down
  - **Software Request:** Adobe upgrade request from Accounting
  - **Hardware Issue:** CFO’s laptop won’t power on
- Each ticket is submitted through the user portal and appears in the agent dashboard for triage.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

2. 👨‍💻 Assignment and Communication (Admin/Agent Actions)
- Admin/Analyst Panel: `http://localhost/osTicket/scp/login.php`
- Deleted the "Maintenance" department and promoted **SysAdmins** to a **Top-Level Department**
- Assigned appropriate **Departments** and **SLA plans** to each ticket:
  - **Ticket 1:** Assigned to `Online Banking`, `Sev-A SLA (1 hour)`
  - **Ticket 2 & 3:** Assigned to `Support`, `Sev-B SLA (4 hours)`
- Observed ticket metadata:
  - **Priority**
  - **Department**
  - **SLA**
  - **Assigned Agent**
- Verified visibility and access permissions (e.g., `john` could not view a ticket assigned to another department without explicit access)
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

3. 🔧 Working the Issue (Ticket Processing)
- Tickets were actively worked and completed by the assigned agents:
  - `john` handled **Support** tickets (Adobe upgrade & CFO laptop)
  - `jane` handled the escalated **SysAdmins** ticket
- Adjusted ticket properties as required, escalated where appropriate.
- Verified visibility restrictions for escalated tickets (required Admin panel access to grant view permissions)
- Reinforced the concept of **ticket ownership, escalation, and limited modification rights** across departments.
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

4. ✅ Resolution (Ticket Closure and Final Notes)
- All tickets were marked as resolved after simulated troubleshooting steps.
- Demonstrated:
  - Ticket resolution process
  - Role-based access control
  - Final ticket status update
- Discussed how osTicket typically sends **automated email notifications** to users on ticket updates, allowing user-agent communication outside the portal.
<br />

🧠 Real-World Application Notes

> In real IT environments, ticket intake can occur via:
- Phone calls
- Walk-ups
- Chat apps (Slack, Teams)
- Email
- Web forms

🎯 **Best Practice:** Create a ticket for *every* issue handled—even ad-hoc requests—to ensure accurate metrics, accountability, and traceability.

## 💼 Skills Demonstrated

- ITIL-aligned ticket lifecycle management
- Realistic end-user simulation and agent response
- Role-based permission troubleshooting
- Ticket escalation and departmental visibility control
- Understanding of metrics and audit trails

## 🔁 Practice & Technical Skill Building

> Repeating this lab builds technical intuition and mastery of support workflows.  
> Encouraged continued practice to reinforce:
- Ticket handling speed and accuracy
- Familiarity with Admin and Agent panels
- Use of the email communication feature
- Efficient user-agent interaction

📌 **Note:** This lab simulates real-world IT support work and reinforces critical technical skills in service management environments.
