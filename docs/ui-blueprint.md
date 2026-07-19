# SprintSync UI Blueprint

## Purpose

This document defines the UI structure and navigation for SprintSync Version 1.

The goal is not to build a flashy product. The goal is to build a clean enterprise-style UI that is simple, consistent, and enough to support backend learning.

---

# UI Principles

- Keep the UI simple and professional.
- Follow a consistent design system.
- Prefer reusable components over page-specific components.
- Avoid unnecessary screens and features.
- Make every screen support backend learning.
- Keep navigation shallow and intuitive.
- Maintain consistency across forms, tables, dialogs, and layouts.

---

# Design Stack

- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- TanStack Query
- TanStack Table
- React Hook Form
- Zod
- Lucide React

---

# Application Layout

```
+------------------------------------------------------+
| Header (Search • Notifications • User Menu)         |
+----------------------+-------------------------------+
| Sidebar              |                               |
|                      |        Main Content           |
| Dashboard            |                               |
| Projects             |                               |
| Tasks                |                               |
| Users                |                               |
| Profile              |                               |
| Settings             |                               |
|                      |                               |
+----------------------+-------------------------------+
```

---

# Sidebar Navigation

## Main Navigation

- Dashboard
- Projects
- Tasks
- Users
- Profile

## Secondary

- Settings (minimal)

---

# Screen Inventory

## Public Screens

- Login
- Forgot Password
- Reset Password

---

## Private Screens

- Dashboard
- Projects List
- Project Details
- Tasks List
- Task Details
- Users List
- User Details
- Profile
- Settings

---

## Dialogs / Modals

- Create Project
- Edit Project
- Create Task
- Edit Task
- Create User
- Edit User
- Assign User
- Change Status
- Delete Confirmation

---

# Screen Details

## Login

- Email / Username
- Password
- Login button
- Forgot password link
- Validation
- Error handling

---

## Dashboard

Contains:

- Summary cards
- Recent Tasks
- Recent Projects
- Basic status overview

No heavy analytics in Version 1.

---

## Projects

Features:

- Table
- Search
- Sorting
- Status Filter
- Create Project
- Edit Project
- Delete Project

Selecting a project opens:

### Project Details

Tabs:

- Overview
- Members
- Tasks
- Activity

---

## Tasks

Features:

- Table
- Search
- Sorting
- Pagination
- Filters
- Create Task
- Edit Task

Selecting a task opens:

### Task Details

Tabs:

- Details
- Comments
- Attachments
- Activity

---

## Users

Features:

- User table
- Search
- Filter by role
- Create User
- Edit User

Selecting a user opens:

### User Details

- Profile
- Assigned Projects
- Assigned Tasks

---

## Profile

- View profile
- Edit profile
- Change password

---

## Settings

Minimal preferences only.

No complex administration screens.

---

# Reusable Components

Layout

- AppLayout
- Sidebar
- Header
- PageContainer
- PageHeader

Tables

- DataTable
- Pagination
- SearchInput
- FilterBar

Forms

- FormField
- TextInput
- SelectInput
- TextArea
- DatePicker

Dialogs

- ModalDialog
- ConfirmDialog

Feedback

- LoadingSkeleton
- EmptyState
- ErrorState
- Toast

Misc

- StatusBadge
- PriorityBadge
- Avatar
- AvatarGroup
- Tabs
- Breadcrumb

---

# Table Standard

Every table should support:

- Search
- Sorting
- Pagination
- Row Actions
- Loading State
- Empty State

Tables:

- Projects
- Tasks
- Users

---

# Form Standard

Every form should contain:

- Label
- Input
- Validation
- Error Message
- Submit
- Cancel
- Loading State

Used by:

- Login
- Project
- Task
- User
- Profile

---

# Navigation Principles

The user should reach any important screen in no more than three clicks.

Example:

Dashboard

↓

Projects

↓

Project Details

↓

Task Details

Avoid deep navigation hierarchies.

---

# Version 1 Exclusions

The following are intentionally excluded to keep the application focused on backend learning:

- Chat
- Calendar
- Kanban Board
- Gantt Chart
- Reports Module
- Audit Log Page
- Notification Center Page
- AI Features
- Real-time Collaboration
- Micro Frontend Architecture

---

# UI Goal

SprintSync should look like a real internal enterprise application.

The interface should be:

- Clean
- Minimal
- Professional
- Easy to navigate
- Consistent

The UI exists to support learning enterprise React and Spring Boot—not to maximize visual complexity.