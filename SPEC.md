# Agent Collaboration Kanban Dashboard

## Project Overview
- **Project Name:** Agent Collaboration Dashboard
- **Purpose:** Visualize and track all agent conversations and tasks in real-time
- **Target Users:** Ishambik (business owner) - to monitor agent collaboration

---

## Core Features

### 1. Agent Cards
- Display all agents: Seonino, WordPressino, Devlopino, Writino
- Show agent status (active/idle)
- Link to agent workspace/logs
- Show current model being used

### 2. Conversation Viewer
- Real-time display of agent-to-agent messages
- Show who is talking to whom
- Timestamp for each message
- Message preview

### 3. Kanban Task Board
Three columns:
- **New** - Newly assigned tasks
- **Processing** - Tasks currently being worked on
- **Done** - Completed tasks

Task cards include:
- Task title
- Assigned agent
- Created timestamp
- Priority indicator

### 4. Broadcast Feature
- Ability to broadcast new tasks to all agents
- Task form with: title, description, assignee, priority
- Real-time updates across dashboard

---

## Technical Stack
- **Frontend:** Single HTML file with embedded CSS/JS
- **Styling:** Modern, clean design (dark mode)
- **Data:** LocalStorage for persistence (demo) / WebSocket ready (future)
- **Icons:** Emoji-based for simplicity

---

## UI Layout

```
┌─────────────────────────────────────────────────────────────┐
│  🤖 Agent Collaboration Dashboard                    [Logo] │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐    │
│  │ Seonino   │ │WordPress │ │Devlopino │ │ Writino  │    │
│  │ 🟢 Active │ │ 🟢 Active│ │ 🟡 Idle  │ │ 🔴 Offline│    │
│  │ GLM-4.7   │ │ Qwen3.5  │ │ MiniMax  │ │ Claude   │    │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘    │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│  💬 Recent Conversations                                    │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────────────────────┐│
│  │ Seonino → WordPressino: "Here's the blog post..."     ││
│  │ Devlopino → Seonino: "Schema verified!"               ││
│  │ WordPressino → Devlopino: "Homepage updated"           ││
│  └─────────────────────────────────────────────────────────┘│
├─────────────────────────────────────────────────────────────┤
│  📋 Kanban Board                        [+ New Task]      │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐           │
│  │    NEW      │ │ PROCESSING  │ │    DONE     │           │
│  │─────────────│ │─────────────│ │─────────────│           │
│  │ ☐ Task 1    │ │ ◐ Task 2   │ │ ✓ Task 3   │           │
│  │ ☐ Task 4    │ │ ◐ Task 5   │ │ ✓ Task 6   │           │
│  │             │ │             │ │             │           │
│  └─────────────┘ └─────────────┘ └─────────────┘           │
└─────────────────────────────────────────────────────────────┘
```

---

## File Structure
```
/data/openclaw-workspace/projects/agent-dashboard/
├── index.html          # Main dashboard (single file)
├── SPEC.md             # This specification
└── README.md           # Usage instructions
```

---

## Acceptance Criteria

1. ✅ Dashboard loads with all 4 agent cards
2. ✅ Agent status displayed (active/idle/offline)
3. ✅ Conversations section shows message history
4. ✅ Kanban board has 3 columns (New, Processing, Done)
5. ✅ Tasks can be created via "New Task" button
6. ✅ Tasks can be dragged between columns
7. ✅ Tasks show: title, agent, timestamp
8. ✅ Responsive design (works on mobile)
9. ✅ Clean, modern dark theme

---

## GitHub Push

When complete, push to:
- **Repository:** https://github.com/discountkeys/agent-dashboard
- **Branch:** main
- **Files:** index.html, README.md

---

**Status:** Ready to build  
**Assigned to:** Devlopino (technical), WordPressino (UI/UX)  
**Deadline:** Today
