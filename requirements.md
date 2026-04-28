# Enterprise Initiative & Action Item Tracker

**System Requirements and End-to-End Flow Document**

## 1. Purpose & Vision

### 1.1 Purpose

The Tracker is intended to serve as a single source of truth for tracking strategic initiatives, action items, ownership, status, and next steps across EY Caribbean AI-related workstreams, replacing fragmented updates across emails, meetings, and ad-hoc documents.

### 1.2 Strategic Vision (as articulated by Anil Persad)

The Tracker is not a passive reporting artifact. It is a management and execution tool that:

- Centralizes visibility across initiatives
- Enables leadership to drive strategy, not chase updates
- Embeds accountability and progress measurement
- Supports prioritization across strategic pillars
- Enables continuity between meetings

## 2. Business Objectives

| Objective           | Description                                                       |
| ------------------- | ----------------------------------------------------------------- |
| Centralization      | All initiatives, actions, and ownership visible in one place      |
| Accountability      | Clear owners and next steps for every tracked item                |
| Continuity          | Tracker updates persist across meetings and reporting cycles      |
| Strategic Alignment | Items mapped to strategic pillars and priorities                  |
| Decision Enablement | Leadership can assess progress, blockers, and focus areas quickly |

## 3. Scope

### 3.1 In Scope

- AI initiatives
- GTM activities
- Capability-building workstreams
- Client pilots (e.g., COJ, StarApple)
- Internal tooling and automation initiatives
- Action items from AI Taskforce meetings

### 3.2 Out of Scope

- Task-level execution tooling (e.g., Jira replacement)
- Time tracking or financial accounting
- HR performance evaluation

## 4. Key Users & Roles

| Role                               | Responsibilities                           |
| ---------------------------------- | ------------------------------------------ |
| Leadership (Anil, Justin, Matthew) | Direction, prioritization, decision-making |
| Tracker Steward                    | Maintains tracker integrity and updates    |
| Initiative Owners                  | Update status and next steps               |
| Contributors                       | Provide inputs to owners                   |
| View-Only Stakeholders             | Consume reports and summaries              |

## 5. Core Data Model (Logical)

Each Tracker Record represents one initiative or major action item.

### 5.1 Mandatory Fields

| Field            | Description                                          |
| ---------------- | ---------------------------------------------------- |
| Initiative ID    | Unique identifier                                    |
| Initiative Name  | Clear, concise title                                 |
| Strategic Pillar | GTM, Capability, Engineering, Value Office, etc.     |
| Description      | What the initiative is                               |
| Owner            | Accountable individual                               |
| Sponsors         | Senior stakeholders                                  |
| Status           | Not Started, In Progress, Blocked, Complete, Removed |
| Priority         | High, Medium, Low                                    |
| Next Steps       | Immediate actions                                    |
| Dependencies     | Upstream/downstream items                            |
| Notes / Context  | Decision history and rationale                       |
| Last Updated     | Timestamp                                            |
| Update Owner     | Person who last updated                              |

## 6. System Flow Overview (High Level)

Meeting Discussion
-> New / Updated Action Identified
-> Tracker Updated
-> Owner Accountability Established
-> Progress Tracked Over Time
-> PDF / Report Generated
-> Distributed Ahead of Next Meeting

## 7. Detailed System Flows

### 7.1 Flow 1: Capturing New Items

**Trigger:**

- AI Taskforce meeting discussion
- Leadership request
- Emerging initiative or decision

**Steps:**

1. Action or initiative is discussed and agreed
2. Tracker Steward creates a new record
3. Owner and sponsor are assigned
4. Status set to Not Started
5. Next steps captured verbatim
6. Item becomes visible to all stakeholders

**Outcome:** Item is officially tracked and cannot be lost between meetings.

### 7.2 Flow 2: Updating Existing Items

**Trigger:**

- Owner progress
- Blocker identified
- Decision made

**Steps:**

1. Owner provides update to Steward or updates directly
2. Status updated (e.g., In Progress -> Blocked)
3. Notes updated with rationale
4. Dependencies adjusted if required
5. Last Updated timestamp refreshed

**Outcome:** Leadership has real-time clarity on progress and issues.

### 7.3 Flow 3: Meeting Preparation

**Trigger:** Upcoming AI Taskforce meeting

**Steps:**

1. Tracker filtered to active items
2. Items grouped by strategic pillar
3. Blocked and high-priority items highlighted
4. PDF export generated
5. Report shared ahead of meeting

**Outcome:** Meetings focus on decisions, not status collection.

### 7.4 Flow 4: In-Meeting Usage

**Trigger:** Live meeting discussion

**Steps:**

1. Tracker report used as agenda
2. Items reviewed sequentially
3. Decisions captured directly into tracker
4. Ownership changes recorded in real time
5. New items logged immediately

**Outcome:** Tracker remains authoritative and current.

### 7.5 Flow 5: Post-Meeting Continuity

**Trigger:** Meeting close

**Steps:**

1. Tracker finalized with agreed updates
2. PDF snapshot archived
3. Tracker becomes baseline for next session

**Outcome:** No regression or loss of institutional memory.

## 8. Reporting & Outputs

### 8.1 Standard Outputs

- PDF tracker report
- Executive summary view
- Blockers and risks view
- Pillar-based rollups

## 9. Governance & Controls

| Control              | Purpose                 |
| -------------------- | ----------------------- |
| Steward role         | Prevents data drift     |
| Mandatory fields     | Enforces consistency    |
| Status definitions   | Avoids ambiguity        |
| Archived snapshots   | Audit trail             |
| Owner accountability | Prevents orphaned items |

## 10. Non-Functional Requirements (Recommended)

Design recommendation (not explicitly prescribed in sources):

- Role-based access
- Version history
- Filter and sort by pillar, owner, priority
- Export to PDF
- Lightweight, low-friction UI

## 11. Success Metrics

| Metric                  | Definition                     |
| ----------------------- | ------------------------------ |
| Update completeness     | % of items with current status |
| Blocker visibility      | Time to surface blockers       |
| Meeting efficiency      | Reduced time spent on status   |
| Decision follow-through | Actions closed vs created      |

Aligned to leadership intent expressed by Anil Persad.

## 12. Summary

This Tracker is fundamentally a strategy execution mechanism, not a spreadsheet. Its value lies in:

- Visibility
- Discipline
- Continuity
- Leadership enablement

As stated by Anil Persad, the objective is to see everything in one place and move the team from operational noise to strategic focus.
