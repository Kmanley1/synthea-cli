# AI Change Log

This log records every automated task completed by Codex/GitHub Copilot or other AI agents for the **Synthea CLI** repository. Automations must append a new entry at the top of **Task Entries** using the template below.

---

## How to Use
1. **Automation** – After a task finishes, the automation script opens this file, inserts a new entry at the top of *Task Entries*, commits, and pushes the change.
2. **Manual fixes** – Developers may correct typos in past entries but **must never** reorder or delete historical items.
3. **Validation** – The CI pipeline fails if the file is missing required fields or the Markdown is malformed.

### Entry Template <!-- do not remove; used by validation script -->
```markdown
### Task Name: <short, imperative>
**Date:** YYYY-MM-DD
**Author:** <automation id or dev>
**Summary:** <1-2 sentence overview of what the task accomplished, referencing PR/commit if applicable>
**Acceptance Criteria:**
- [ ] Criterion 1
- [ ] Criterion 2
---
```

---

## Task Entries

<!-- New entries must be inserted directly below this line -->

### Task Name: Verify synthea run integration
**Date:** 2025-05-25
**Author:** Codex-Automation
**Summary:** Added integration test and README instructions (commit d3d8047).
**Acceptance Criteria:**
- [x] Test project runs `synthea run` and checks output
- [x] README explains how to run integration tests
---

### Task Name: Prefix implemented tasks with start timestamp
**Date:** 2025-05-25
**Author:** Codex-Automation
**Summary:** Updated automation to prepend UTC timestamps when moving task files, ensuring idempotency (commit 9661577).
**Acceptance Criteria:**
- [x] Timestamp prefix added on move
- [x] Context files remain in place
---

### Task Name: Move tasks to implemented after execution
**Date:** 2025-05-25
**Author:** Codex-Automation
**Summary:** Fixed missing context directories causing tasks to stay in `tasks/`; automation now creates them and moves completed tasks (commit e16a636).
**Acceptance Criteria:**
- [x] Tasks archived on success
- [x] Automation handles absent context folders
---


### Task Name: Sync automation docs with code
**Date:** 2025-05-25
**Author:** Codex-Automation
**Summary:** Updated codex-automation.md and archived task file, commit 1aa0e98.
**Acceptance Criteria:**
- [x] Documentation matches actual behaviour
- [x] Task file moved to implemented with timestamp
---

