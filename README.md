SOLVEX

Smart Customer Support & Predictive SLA Management System

Tagline: Beyond Tickets. Predicting Problems.

Hackathon: AVISHKAR'26
Team Name: Hackhive
Project Name: SOLVEX

---

1. Project Overview

SOLVEX is a smart customer support and predictive SLA management platform designed to improve the way organizations handle customer complaints, support requests and service-related issues.

Traditional helpdesk systems mainly focus on recording and resolving tickets. SOLVEX aims to go beyond conventional ticket management by identifying potential problems, predicting SLA breaches, detecting similar incidents and helping support teams resolve issues efficiently.

The platform provides three dedicated workspaces:

- Customer Portal
- Agent Workspace
- Admin Control Center

All three workspaces are connected through a unified backend and database.

2. Problem Statement

Organizations receive a large number of customer complaints and service requests every day.

Traditional support systems face several challenges:

- Delayed ticket assignment.
- Difficulty identifying repeated or similar problems.
- SLA deadlines being missed.
- Uneven distribution of workload among support agents.
- Lack of regular communication with customers.
- Difficulty identifying common incidents.
- Repeated efforts to solve previously resolved problems.

These challenges reduce customer satisfaction and increase operational workload.

3. Proposed Solution

SOLVEX provides an integrated support management system that helps organizations manage tickets intelligently.

The system will:

1. Allow customers to submit and track support tickets.
2. Automatically categorize and prioritize incoming tickets.
3. Recommend suitable agents for ticket assignment.
4. Monitor SLA deadlines and identify possible breaches.
5. Detect similar tickets and potential common incidents.
6. Suggest solutions from previously resolved tickets.
7. Notify users about important ticket updates.
8. Provide administrators with real-time operational insights.

4. Main Objectives

- Improve customer support response time.
- Reduce SLA violations.
- Improve ticket assignment efficiency.
- Identify repeated issues.
- Improve agent workload distribution.
- Maintain transparent customer communication.
- Build a reusable knowledge base of resolved problems.

5. User Modules

A. Customer Portal

Customers can:

- Register and securely log in.
- Create support tickets.
- Select ticket categories and priorities.
- Upload relevant attachments.
- Track ticket status.
- View ticket progress and history.
- Communicate with assigned agents.
- Receive notifications.
- Confirm resolution.
- Submit customer satisfaction feedback.

B. Agent Workspace

Support agents can:

- Log in through a dedicated agent account.
- View assigned tickets.
- Access authorized unassigned tickets.
- Review ticket details.
- Reply to customers.
- Add private internal notes.
- Update ticket status.
- Monitor SLA countdowns.
- View similar incidents.
- Access previous resolution suggestions.
- Escalate tickets when required.

C. Admin Control Center

Administrators can:

- View all support tickets.
- Manage customers and agents.
- Create and manage agent accounts.
- Configure SLA policies.
- Assign and reassign tickets.
- Monitor agent workloads.
- View SLA performance.
- Manage incident groups.
- Analyze ticket trends.
- View system analytics and reports.

6. Innovative Features

1. SLA Rescue Radar

A proactive SLA monitoring feature that identifies tickets at risk of missing their deadlines.

It considers:

- Remaining SLA time.
- Ticket age.
- Ticket priority.
- Agent workload.
- Historical resolution duration, when sufficient data is available.

It generates risk levels and recommends actions such as escalation or reassignment.

2. Issue DNA

Identifies similar customer complaints and groups potential common incidents.

For example, if several customers report GPS tracking failures, SOLVEX can identify a possible shared incident rather than treating every complaint as completely unrelated.

3. Smart Problem Reproduction Assistant

Collects structured information about customer problems, including:

- What the customer tried.
- What actually happened.
- What was expected.
- Device or browser information.
- Relevant screenshots or attachments.

It helps agents understand and reproduce problems more easily.

4. Resolution Memory

Stores useful solutions from resolved tickets and recommends relevant previous solutions when similar problems appear.

5. Agent Fairness Meter

Helps distribute tickets fairly by considering:

- Current assigned tickets.
- Ticket priority.
- Ticket complexity.
- Agent workload.

It recommends suitable assignments to avoid overloading individual agents.

6. No-Silence Promise

Identifies tickets that have not received progress updates within the configured period and alerts responsible agents.

It encourages timely and transparent customer communication.

7. Ticket Journey Map

Provides customers with a visual representation of their ticket progress:

Submitted → Assigned → Investigating → In Progress → Resolved → Feedback.

7. Technology Stack

Component| Technology
Frontend| Next.js
UI Library| React
Programming Language| TypeScript
Styling| Tailwind CSS
Icons| Lucide React
Charts| Recharts
Backend| Node.js
Backend Framework| Express.js
Database| PostgreSQL
ORM| Prisma
Authentication| Secure session-based authentication
Password Security| bcrypt
Real-time Communication| Socket.IO
Validation| Zod
Containerization| Docker

8. System Architecture

SOLVEX follows a modular full-stack architecture.

Frontend Layer

- Customer Portal
- Agent Workspace
- Admin Control Center

Backend Layer

- Authentication and Authorization
- User Management
- Ticket Management
- Assignment Management
- SLA Management
- Notification Management
- Analytics and Reporting
- Innovative Feature Services

Database Layer

- PostgreSQL
- Prisma ORM

Real-time Layer

- Socket.IO for live notifications and ticket updates.

9. Database Design

The planned database includes the following main entities:

Entity| Description
User| Stores customer, agent and admin accounts
Ticket| Stores support ticket information
TicketMessage| Stores public conversations
InternalNote| Stores private agent notes
TicketAttachment| Stores ticket attachment information
TicketAssignment| Tracks ticket assignments
SLAPolicy| Stores SLA rules
SLARecord| Tracks SLA deadlines and performance
Notification| Stores user notifications
TicketFeedback| Stores customer feedback
TicketHistory| Tracks ticket activity
AgentSkill| Stores agent expertise
TicketIncidentGroup| Groups related incidents
ResolutionKnowledge| Stores previously resolved solutions

10. Security and Access Control

SOLVEX will implement role-based access control.

- Customers can access only their own tickets.
- Agents can access tickets assigned to them and other tickets explicitly authorized for their role.
- Administrators can manage the overall platform.
- Passwords will be securely hashed.
- Protected APIs will validate user permissions.
- Private internal notes will never be exposed through customer-facing APIs.
- Environment secrets will not be committed to GitHub.

11. Project Folder Structure

SOLVEX/
│
├── apps/
│   ├── web/
│   │   ├── app/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── lib/
│   │   └── public/
│   │
│   └── api/
│       ├── src/
│       │   ├── config/
│       │   ├── controllers/
│       │   ├── middleware/
│       │   ├── routes/
│       │   ├── services/
│       │   ├── sockets/
│       │   ├── utils/
│       │   └── server.ts
│       │
│       └── prisma/
│           ├── schema.prisma
│           └── seed.ts
│
├── docs/
├── docker-compose.yml
├── package.json
├── .env.example
├── .gitignore
└── README.md

12. Development Roadmap

The project will be developed in the following stages:

1. Project documentation and initial setup.
2. GitHub integration and monorepo configuration.
3. PostgreSQL database design and Prisma setup.
4. Frontend development.
5. Backend API development.
6. Authentication and role-based authorization.
7. Ticket management integration.
8. SLA Rescue Radar and innovative features.
9. Real-time notifications using Socket.IO.
10. Testing, optimization and deployment.

13. Expected Outcomes

SOLVEX aims to deliver:

- Faster and more organized customer support.
- Improved SLA monitoring.
- Better identification of repeated incidents.
- More balanced agent workload.
- Reduced repetitive troubleshooting.
- Improved customer communication.
- Better visibility into support operations.

14. Future Enhancements

Potential future enhancements include:

- Advanced machine-learning-based ticket classification.
- More sophisticated SLA breach prediction.
- Multilingual customer support.
- AI-assisted response suggestions.
- Voice-based ticket creation.
- Advanced incident analytics.

15. Conclusion

SOLVEX aims to transform traditional customer support from a reactive ticket-handling process into a proactive and intelligent support management system.

By combining ticket management, SLA monitoring, incident detection, workload balancing and resolution knowledge, SOLVEX aims to help organizations identify problems earlier and deliver better customer support.

SOLVEX — Beyond Tickets. Predicting Problems.

Developed by Team Hackhive | AVISHKAR'26