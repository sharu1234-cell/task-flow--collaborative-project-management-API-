# TaskFlow – Collaborative Project Management API

## Project Overview
TaskFlow is a RESTful API for a collaborative project management platform that enables teams to create projects, manage tasks, track progress, and facilitate team communication with real-time updates.

## Tech Stack
- **Runtime**: Node.js v20+
- **Framework**: Express.js
- **Database**: PostgreSQL with Drizzle ORM
- **Real-time**: WebSocket (ws)
- **Frontend**: React + TypeScript + Tailwind CSS

## Features
- Project & Team Management
- Task Management with Kanban board
- Real-time WebSocket updates
- Analytics dashboard

## Installation

```bash
npm install
npm run db:push
npm run dev
```

## API Endpoints

### Authentication
- POST /api/auth/register
- POST /api/auth/login

### Projects
- GET /api/projects
- POST /api/projects
- GET /api/projects/:id
- PUT /api/projects/:id
- DELETE /api/projects/:id

### Tasks
- GET /api/tasks
- POST /api/tasks
- PUT /api/tasks/:id
- DELETE /api/tasks/:id

### Teams
- GET /api/teams
- POST /api/teams
- DELETE /api/teams/:id

### Comments
- GET /api/tasks/:taskId/comments
- POST /api/tasks/:taskId/comments

### Attachments
- GET /api/tasks/:taskId/attachments
- POST /api/tasks/:taskId/attachments
- GET /api/attachments/:id
- DELETE /api/attachments/:id

## WebSocket
Connect to ws://localhost:5000/ws for real-time updates.

## License
MIT
