Sprintly — README (Planning Doc for project )
What is this?


A multi-user, Jira-inspired project & task management platform. One person can create a workspace, invite/manage team members, create projects, and track tasks through a drag-and-drop Kanban board — with an analytics dashboard showing team progress.

Built specifically as a portfolio project to demonstrate React + REST API + full-stack skills for frontend/full-stack internship applications (Bright Money and similar FinTech/startup roles).

Tech Stack
Frontend: React (functional components, hooks), react-beautiful-dnd or @dnd-kit for drag-and-drop, Axios for API calls, Recharts/Chart.js for dashboard
Backend: Laravel (REST API), JWT/Sanctum for authentication
Database: MySQL
Styling: CSS3 / Tailwind (mobile-first, responsive)
Core Features to Build
1. Authentication & Users
Signup/Login (JWT via Laravel Sanctum)
Roles: Admin (creates workspace/projects) vs Member (assigned to tasks)
2. Workspaces & Projects
User creates a "Workspace"
Workspace has multiple "Projects"
Each project has its own Kanban board
3. Kanban Board (core React piece)
Columns: To Do / In Progress / Done (customizable later)
Drag-and-drop tasks between columns
Add/Edit/Delete task (title, description, assignee, due date, priority)
4. Team Collaboration
Invite members to workspace (simple email-based invite or just add-by-username for MVP)
Assign tasks to specific members
5. Analytics Dashboard
Task completion % per project
Workload distribution (tasks per member)
Simple charts using Recharts — bar/pie chart is enough, no need for literal Power BI embed
6. Responsive Design
Mobile-first layout
Board view collapses to stacked/scrollable view on small screens
Suggested Build Order (2–3 Days)

Day 1 — Backend Foundation

Laravel setup, migrations: users, workspaces, projects, tasks, workspace_members
Auth API (register/login/JWT)
CRUD API for projects and tasks

Day 2 — Frontend Core

React app setup, routing (login → dashboard → project board)
Kanban board UI + drag-and-drop
Connect to Laravel API (Axios) for tasks CRUD

Day 3 — Dashboard + Polish

Analytics dashboard page (Recharts)
Responsive styling pass
README with screenshots/GIF
Deploy (Vercel for frontend, Railway/Render for backend) if time allows
What NOT to over-engineer (keep MVP scope)
Skip real email invites — just add members by username/ID for now
Skip literal Power BI integration — native Recharts dashboard is enough, call it "analytics dashboard" not "Power BI dashboard"
Skip notifications/real-time sockets — not needed to prove the core skills this JD asks for
Skip custom column creation — fixed 3 columns (To Do/In Progress/Done) is fine for MVP
Resume Bullet (once built)
Sprintly – Multi-User Project & Task Management Platform (2026)
React, Laravel, MySQL, REST APIs
- Built a Jira-inspired multi-user task management platform with role-based access control for teams and project boards.
- Developed a drag-and-drop Kanban interface using React hooks and component-level state management.
- Engineered a Laravel REST API with JWT authentication, supporting multi-tenant workspaces and team collaboration.
- Designed analytics dashboards visualizing task completion and workload distribution.
- Implemented a fully responsive, mobile-first UI for cross-device usability.
