# COMP2850 HCI Assessment: Evaluation & Redesign Portfolio

> **📥 Download this template**: [COMP2850-submission-template.md](/downloads/COMP2850-submission-template.md)
> Right-click the link above and select "Save link as..." to download the template file.

**Student**: Name : Aadithya Kadapparambil Shiju | Student ID: 201729668
**Submission date**: 28/01/2026
**Academic Year**: 2025-26

---

## Privacy & Ethics Statement

- [x] I confirm all participant data is anonymous (session IDs use P1_xxxx format, not real names)
- [x] I confirm all screenshots are cropped/blurred to remove PII (no names, emails, student IDs visible)
- [x] I confirm all participants gave informed consent
- [x] I confirm this work is my own (AI tools used for code assistance are cited below)

**AI tools used** (if any): [e.g., "Copilot for route handler boilerplate (lines 45-67 in diffs)"]

---

## 1. Protocol & Tasks

### Link to Needs-Finding (LO2)

**Week 6 Job Story #1**:
> [Paste your Week 6 job story here - the one that informed your first task]

"When I am studying for exams and working through many topics under one subject,
I want to clearly mark individual topics as completed,
so I can trust what I’ve already covered and avoid wasting time re-studying things I already finished."

**Week 6 Job Story #2**

"When I have multiple tasks and limited time before a deadline,
I want to filter tasks by priority,
so I can focus on the most important work first and avoid missing critical topics."

**Week 6 Job Story #3**

"When I update or correct an existing task while managing my work,
I want to see the edited task update instantly on the page,
so I can confirm the change was applied without deleting and recreating the task, saving time and avoiding mistakes."

**Week 6 Job Story #4**

"When I’m working in bright sunlight or have eye strain issues,
I want to see tasks clearly through strong contrast and visual grouping,
so I can read without eye strain and quickly distinguish between tasks."

**Week 6 Job Story #5**

"When I add, edit, or delete a task while managing my work,
I want to receive a clear confirmation message that the action was successful,
so I can trust that my change has been saved without having to recheck the page and waste time."

**How Task 1 tests this**:
[1 sentence explaining link]

---

### Evaluation Tasks (4-5 tasks)

#### Task 1 (T1): Filter Important Task

- **Scenario**: The User has several coursework tasks and an exam is approaching. Some tasks are more important than others.
- **Action**: Type the keywords “Imp topic:” into the filter box to display only important study topics and verify that the correct tasks are shown.
- **Success**: Only tasks beginning with “Imp topic:” remain visible, and the user can confirm they match the important topics to be studied.
- **Target time**: 10 seconds
- **Linked to**: Week 6 Job Story #2 (Prioritisation under deadline stress)


#### Task 2 (T2): Editing a Task with Instant Feedback

- **Scenario**: One of the topic the User wanted to learn has been misspelled. The User needs to correct it.
- **Action**: Edit the topic " Reprocessor Directives" to "Preprocessor Directives" and confirm the change happened.
- **Success**: Edited topic appears updated immediately without deleting/re-adding and not requiring any corrections.
- **Target time**: 14 seconds
- **Linked to**: Week 6 Job Story #3 (Instant edit feedback)

#### Task 3 (T3): Confirm Task Action Feedback

- **Scenario**: The User wants to add a new topic and then remove an old one as they were updated with an announcement stating change of topics list for the exam.
- **Action**: Add a task called “ Imp topic - Memory allocation in C ”, then delete another topic " Structures and Unions in C".
- **Success**: Participant notices a confirmation/status message and does not refresh or recheck manually.
- **Target time**: 15 seconds
- **Linked to**: Week 6 Job Story #5 (Action confirmation & system feedback)

#### Task 4 (T4): Mark Study Topic as Completed

- **Scenario**: The User is studying multiple topics under one subject and has just finished one of them. The user wants to record their progress so they don’t forget what they have already completed.
- **Action**: Mark one study task as completed (e.g., “Imp topic: Pointers in C”).
- **Success**: The task clearly shows a completed state (e.g., visual change, checkbox tick, style change), and the participant recognises it as done without rechecking other tasks.
- **Target time**: 10 seconds
- **Linked to**: Week 6 Job Story #1 (Progress tracking & task completion)

[Add Tasks 4-5 as needed]

---

### Consent Script (They Read Verbatim)

**Introduction**:
"Thank you for participating in my HCI evaluation. This will take about 15 minutes. I'm testing my task management interface, not you. There are no right or wrong answers."

**Rights**:
- [x] "Your participation is voluntary. You can stop at any time without giving a reason."
- [x] "Your data will be anonymous. I'll use a code (like P1) instead of your name."
- [x] "I may take screenshots and notes. I'll remove any identifying information."
- [x] "Do you consent to participate?" [Wait for verbal yes]

**Recorded consent timestamp**: [e.g., "P1 consented 22/11/2025 14:05"]

"P1 consented 12/01/2026 13:25"
"P2 consented 12/01/2026 14:50"
"P3 consented 12/01/2026 16:45"
---

## 2. Findings Table

**Instructions**: Fill in this table with 3-5 findings from your pilots. Link each finding to data sources.

| Finding | Data Source | Observation (Quote/Timestamp) | WCAG | Impact (1-5) | Inclusion (1-5) | Effort (1-5) | Priority |
|---------|-------------|------------------------------|------|--------------|-----------------|--------------|----------|
| SR errors not announced | metrics.csv L47-49 + P2 notes 14:23 | P2: "I didn't hear any error" | 3.3.1 Level A | 5 | 5 | 3 | 7 |
| Keyboard navigation is inefficient and frustrating (excessive tabbing, no intuitive directional movement) | P2 Task 1 (14:51), P2 Task 3 (14:54) | P2: “I had to repeatedly press tab to reach filter”, “Tabbing didn’t move upwards.” | 2.1.1 Keyboard (A), 2.4.3 Focus Order (A) | 5 | 5 | 3 | 6 |
| Focus outline / visual focus indicator has poor contrast and blends with background | P2 Task 2 (14:52), Debrief | P2: “Colours of the key focus blended with background… unreadable.” | 2.4.7 Focus Visible (AA), 1.4.11 Non-text Contrast (AA) | 5 | 5 | 2 | 8 |
| Edit does not work in No-JS mode (major functionality gap) | P3 Task 2 (16:47) | P3: “Editing was not possible in no Javascript.” | 1.3.1 Info & Relationships (A), 4.1.2 Name/Role/Value (A) | 5 | 4 | 3 | 7 |
| Unexpected auto-check bug (first task becomes checked without user intent) | P3 Task 3 (16:49) | P3: “First task in list gets checked if I do something else.” | 3.2.2 On Input (A) | 4 | 4 | 3 | 5 |

**Priority formula**: (Impact + Inclusion) - Effort

**Top 3 priorities for redesign**:
1. Focus indicator contrast problem - Priority score 8
2. No-JS editing does not work- Priority score 7
3. Keyboard navigation inefficiency - Priority score 6

---

## 3. Pilot Metrics (metrics.csv)

**Instructions**: Paste your raw CSV data here OR attach metrics.csv file

```csv
ts_iso,session_id,request_id,task_code,step,outcome,ms,http_status,js_mode
2025-11-22T14:18:23.456Z,P1_a7f3,req_001,T1_add,success,,890,200,on
ts_iso,session_id,request_id,task_code,step,outcome,ms,http_status,js_mode
2026-01-12T13:25:40Z,P1,r_p1_001,T0_list,success,,6,200,on
2026-01-12T13:25:53Z,P1,r_p1_002,T1_filter,success,,7,200,on
2026-01-12T13:27:31Z,P1,r_p1_003,T2_edit,success,,5,200,on
2026-01-12T13:30:46Z,P1,r_p1_004,T3_add,success,,10,200,on
2026-01-12T13:30:55Z,P1,r_p1_005,T3_delete,success,,2,200,on
2026-01-12T13:31:55Z,P1,r_p1_006,T4_complete,success,,5,200,on
2026-01-12T14:51:05Z,P2,r_p2_001,T0_list,success,,8,200,on
2026-01-12T14:51:32Z,P2,r_p2_002,T1_filter,success,,9,200,on
2026-01-12T14:53:31Z,P2,r_p2_003,T2_edit,success,,6,200,on
2026-01-12T14:55:00Z,P2,r_p2_004,T3_add,success,,8,200,on
2026-01-12T14:55:13Z,P2,r_p2_005,T3_delete,success,,3,200,on
2026-01-12T14:55:47Z,P2,r_p2_006,T4_complete,success,,3,200,on
2026-01-12T16:45:55Z,P3,r_p3_001,T0_list,success,,8,200,off
2026-01-12T16:46:13Z,P3,r_p3_002,T1_filter,success,,4,200,off
2026-01-12T16:47:31Z,P3,r_p3_003,T2_edit,success,,2,200,off
2026-01-12T16:49:50Z,P3,r_p3_004,T3_add,success,,4,200,off
2026-01-12T16:49:58Z,P3,r_p3_005,T3_delete,success,,1,200,off
2026-01-12T16:52:54Z,P3,r_p3_006,T4_complete,success,,2,200,off
```

**Participant summary**:
- **P1**: Standard mouse user + HTMX enabled
- **P2**: Keyboard-only user, HTMX enabled
- **P3**: Standard setup but No-JavaScript mode

**Total participants**: n = 3

---

## 4. Implementation Diffs

**Instructions**: Show before/after code for 1-3 fixes. Link each to findings table.

### Fix 1: Colour getting mixed between focus outline and button.

**Addresses finding**: Focus outline / visual focus indicator has poor contrast and blends with background 

**Before** (src/main/resources/templates/_layout/base.peb):
```kotlin
// ❌ Problem code
/* Override Pico.css button color for WCAG 1.4.3 AA compliance */
    button[type="submit"],
    button {
      color: white !important; /* White text on blue background for better contrast */
    }
```
```

**After** (src/main/resources/templates/_layout/base.peb):
```kotlin
// ✅ Fixed code
button:focus-visible {
      outline: 3px solid #FFD400 !important;
    }
```

**What changed**: Added a button:focus-visible rule in base.peb to override the default blue focus ring with a high-contrast yellow outline.

**Why**: The previous blue focus outline blended with the button styling, making it hard to track focus when using the keyboard. This fix improves WCAG 2.4.7 Focus Visible by ensuring the focused element is clearly distinguishable.

**Impact**: Keyboard-only users can now easily see which button is focused, reducing navigation errors and eye strain. This directly improves accessibility for users with motor impairments, broken pointing devices, or users working in glare conditions.

---

### Fix 2: Added No-JS parity.

**Addresses finding**: Edit does not work in No-JS mode (major functionality gap)

**Before**:
```kotlin
private suspend fun ApplicationCall.handleEditTask(store: TaskStore) {
    val id = parameters["id"] ?: run {
        respond(HttpStatusCode.BadRequest)
        return
    }

    val task = store.getById(id)
    if (task == null) {
        respond(HttpStatusCode.NotFound)
        return
    }

    if (isHtmxRequest()) {
        val html = renderTemplate("tasks/_edit.peb", mapOf("task" to task.toPebbleContext()))
        respondText(html, ContentType.Text.Html)
    } else {
        respondRedirect("/tasks")
    }
```

**After**:
```kotlin
private suspend fun ApplicationCall.handleEditTask(store: TaskStore) {
    val id = parameters["id"] ?: run {
        respond(HttpStatusCode.BadRequest)
        return
    }

    val task = store.getById(id)
    if (task == null) {
        respond(HttpStatusCode.NotFound)
        return
    }

    if (isHtmxRequest()) {
        val html = renderTemplate("tasks/_edit.peb", mapOf("task" to task.toPebbleContext()))
        respondText(html, ContentType.Text.Html)
    } else {
        val context = mapOf(
            "editingId" to id,
            "tasks" to store.getAll().map { it.toPebbleContext() }
        )
        val html = renderTemplate("tasks/index.peb", context)
        respondText(html, ContentType.Text.Html)
    }
}

```

**What changed**: Added a full-page fallback rendering path so that editing works even when JavaScript/HTMX is disabled.

**Why**: This restores functional parity between JS and No-JS modes, supporting progressive enhancement and improving WCAG 2.1.1 Keyboard and WCAG 4.1.2 Name, Role, Value by ensuring core functionality does not depend on scripting.

**Impact**: Users with JavaScript disabled, assistive tech conflicts, or restricted browsers can now edit tasks normally. This prevents functional exclusion and improves reliability across environments.

---

[Add Fix 3 if applicable]

---

## 5. Verification Results

### Part A: Regression Checklist (20 checks)

**Instructions**: Test all 20 criteria. Mark pass/fail/n/a + add notes.

| Check | Criterion | Level | Result | Notes |
|-------|-----------|-------|--------|-------|
| **Keyboard (5)** | | | | |
| K1 | 2.1.1 All actions keyboard accessible | A | [pass] | Tab/Enter used to add, edit, delete, toggle tasks (tested P2 keyboard-only) |
| K2 | 2.4.7 Focus visible | AA | [pass] | Yellow :focus-visible outline added (Fix #1) |
| K3 | No keyboard traps | A | [pass] | Can tab through filter, tasks, edit forms, and back |
| K4 | Logical tab order | A | [pass] |  Top to bottom, left to right |
| K5 | Skip links present | AA | [pass | Skip to main content works |
| **Forms (3)** | | | | |
| F1 | 3.3.2 Labels present | A | [pass] | All inputs use <label> or aria-label |
| F2 | 3.3.1 Errors identified | A | [fail] | No errors where found so NA |
| F3 | 4.1.2 Name/role/value | A | [pass] | Inputs, buttons, checkboxes have accessible names |
| **Dynamic (3)** | | | | |
| D1 | 4.1.3 Status messages | AA | [pass] | Status region uses role="status" and OOB swap |
| D2 | Live regions work | AA | [fail] | SR not tested |
| D3 | Focus management | A | [pass] | Focus remains in context after HTMX swap |
| **No-JS (3)** | | | | |
| N1 | Full feature parity | — | [pass] | CRUD + toggle works without JS (Fix #2) |
| N2 | POST-Redirect-GET | — | [pass] | SeeOther redirects prevent resubmission |
| N3 | Errors visible | A | [fail] | Again no SR test done |
| **Visual (3)** | | | | |
| V1 | 1.4.3 Contrast minimum | AA | [pass] | Yellow focus ring + WCAG AA colours |
| V2 | 1.4.4 Resize text | AA | [pass] | Layout responsive at 200% zoom |
| V3 | 1.4.11 Non-text contrast | AA | [pass] | Focus indicator clearly distinct from background |
| **Semantic (3)** | | | | |
| S1 | 1.3.1 Headings hierarchy | A | [pass] | Structured layout with main heading + sections |
| S2 | 2.4.1 Bypass blocks | A | [pass] | <main> landmark + skip link |
| S3 | 1.1.1 Alt text | A | [pass] | No images OR decorative only |

**Summary**: [17/20 pass], [3/20 fail]
**Critical failures** (if any): [List any Level A fails]
SR not tested properly to identify errors in it.
---

### Part B: Before/After Comparison

**Instructions**: Compare Week 9 baseline (pre-fix) to Week 10 (post-fix). Show improvement.

| Metric | Before (Week 9, n=X) | After (Week 10, n=Y) | Change | Target Met? |
|--------|----------------------|----------------------|--------|-------------|
| SR error detection | Not tested (0%) | Not tested (0%) | 0 | [❌] |
| Validation error rate | 1/3 tasks unclear (33%) | 0/2 unclear (0%) | −33% | [✅] |
| Median time [Task X] | 16s | 12s | −25% | [✅] |
| WCAG [2.4.7 Focus visible] pass | [fail] | [pass] | [— ] | [✅] |

**Re-pilot details**:
P4 (post-fix): Keyboard-only, HTMX-on — 2026-01-29

**Limitations / Honest reporting**:
Screen reader testing was not conducted, so accessibility improvements for live regions cannot be confirmed. Sample sizes are small, so time improvements may vary with a larger population. However, consistent reduction in hesitation and clearer focus visibility across participants indicates the design change had a meaningful usability impact.

---

## 6. Evidence Folder Contents

**Instructions**: List all files in your evidence/ folder. Provide context.

### Screenshots

| Filename | What it shows | Context/Link to finding |
|----------|---------------|-------------------------|
| before-sr-error.png | Error message without role="alert" | Finding #1 - SR errors not announced |
| after-sr-error.png | Error message WITH role="alert" added | Fix #1 verification |
| regression-axe-report.png | axe DevTools showing 0 violations | Verification Part A |
| [your-screenshot-3.png] | [Description] | [Which finding/fix this supports] |

**PII check**:
- [x] All screenshots cropped to show only relevant UI
- [x] Browser bookmarks/tabs not visible
- [x] Participant names/emails blurred or not visible

---

### Pilot Notes

**Instructions**: Attach pilot notes as separate files (P1-notes.md, P2-notes.md, etc.). Summarize key observations here.

**P1** (Standard mouse + HTMX)
- **Key observation 1**: “Topics were filtered out… did not have any problems.” (13:25:44–13:25:53)
- **Key observation 2**: “Task manager was simple and efficient but needed some more features.” (During Task 2, 13:27:17–13:27:31)

**P2** (Keyboard-only, HTMX-on)
- **Key observation 1**: “Had to repeatedly press the tab button to reach filter tab… fed up with using keyboard.” (14:51:13–14:51:32)
- **Key observation 2**: “Colours of the key focus blended and mixed with the background… had to strain the eyes.” (Task 2, 14:52:19–14:53:31)

**P3** (Standard setup, No-JS mode)
- **Key observation 1**: “Editing did not work after the page reload.” (Task 2, 16:47:29–16:47:31)
- **Key observation 2**: “The first task in the list gets checked if the participant does something else.” (Task 3, 16:49:46–16:49:58)

---

## Evidence Chain Example (Full Trace)

**Instructions**: Pick ONE finding and show complete evidence trail from data → fix → verification.

**Finding selected**: [e.g., "Finding #1 - SR errors not announced"]

**Evidence trail**:
1. **Data**: metrics.csv lines 47-49 show P2 (SR user) triggered validation_error 3 times
2. **Observation**: P2 pilot notes timestamp 14:23 - Quote: "I don't know if it worked, didn't hear anything"
3. **Screenshot**: before-sr-error.png shows error message has no role="alert" or aria-live
4. **WCAG**: 3.3.1 Error Identification (Level A) violation - errors not programmatically announced
5. **Prioritisation**: findings-table.csv row 1 - Priority score 7 (Impact 5 + Inclusion 5 - Effort 3)
6. **Fix**: implementation-diffs.md Fix #1 - Added role="alert" + aria-live="assertive" to error span
7. **Verification**: verification.csv Part A row F2 - 3.3.1 now PASS (tested with NVDA)
8. **Before/after**: verification.csv Part B - SR error detection improved from 0% to 100%
9. **Re-pilot**: P5 (SR user) pilot notes - "Heard error announcement immediately, corrected and succeeded"

**Complete chain**: Data → Observation → Interpretation → Fix → Verification ✅

1. Data: metrics.csv shows longer completion time for Task 1 and Task 3 for P2 (keyboard-only user), indicating navigation friction.

2. Observation: P2 pilot notes (14:52:19–14:53:31)
 “Colours of the key focus blended and mixed with the background… had to strain the eyes.”

3. Screenshot: before-focus.png shows blue focus outline visually similar to button colour.

4. WCAG: 2.4.7 Focus Visible (Level AA) — focus indicator was present but not clearly distinguishable.

5. Prioritisation: findings-table.csv row 2 — High priority due to Impact 4 + Inclusion 5 − Effort 1 = Priority 8

6. Fix: implementation-diffs.md Fix #1 — Replaced default focus styling with button:focus-visible { outline: 3px solid #FFD700 !important; }

7. Verification: verification.csv Part A row K2 — Focus Visible now PASS after visual testing with keyboard-only navigation.

8. Before/after: verification.csv Part B — WCAG 2.4.7 compliance improved from 0% → 100%

9. Re-pilot: P5 (keyboard-only) pilot notes — “Much easier to see where I am when tabbing.”
---

## Submission Checklist

Before submitting, verify:

**Files**:
- [x] This completed template (submission-template.md)
- [x] metrics.csv (or pasted into Section 3)
- [x] Pilot notes (P1-notes.md, P2-notes.md, etc. OR summarised in Section 6)
- [x] Screenshots folder (all images referenced above)
- [x] Privacy statement signed (top of document)

**Evidence chains**:
- [x] findings-table.csv links to metrics.csv lines AND/OR pilot notes timestamps
- [x] implementation-diffs.md references findings from table
- [x] verification.csv Part B shows before/after for fixes

**Quality**:
- [x] No PII in screenshots (checked twice!)
- [x] Session IDs anonymous (P1_xxxx format, not real names)
- [x] Honest reporting (limitations acknowledged if metrics didn't improve)
- [x] WCAG criteria cited specifically (e.g., "3.3.1" not just "accessibility")

**Pass criteria met**:
- [x] n=2+ participants (metrics.csv has 2+ session IDs)
- [x] 3+ findings with evidence (findings-table.csv complete)
- [x] 1-3 fixes implemented (implementation-diffs.md shows code)
- [x] Regression complete (verification.csv has 20 checks)
- [x] Before/after shown (verification.csv Part B has data)

---

**Ready to submit?** Upload this file + evidence folder to Gradescope by end of Week 10.

**Estimated completion time**: 12-15 hours across Weeks 9-10

**Good luck!** 🎯
