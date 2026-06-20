# Overtime Entry Feature

## Feature Description

Site managers should be able to record overtime worked by employees at the end of each day.

Fields:

- Worker
- Date
- Overtime Hours
- Reason
- Submitted By

Mobile support is required.

---

## Acceptance Criteria

### AC-01 Worker Selection

Given a site manager is logged in

When opening overtime entry

Then the manager can select a worker assigned to their site.

---

### AC-02 Date Entry

Given overtime is being recorded

When selecting a date

Then future dates must not be allowed.

---

### AC-03 Hours Validation

Given overtime hours are entered

When value is less than 0

Then validation error should appear.

When value exceeds allowed limit

Then submission should be blocked.

---

### AC-04 Reason Validation

Given overtime is submitted

When reason field is empty

Then system must display validation message.

---

### AC-05 Duplicate Prevention

Given overtime already exists for worker and date

When another record is submitted

Then system should prevent duplicate entry.

---

### AC-06 Mobile Support

Given manager uses mobile device

When accessing overtime page

Then all controls should remain usable.

---

## Edge Cases

1. Same worker entered twice.
2. Duplicate overtime for same day.
3. Internet disconnect during submission.
4. Worker no longer active.
5. Manager enters 0 hours.
6. Manager enters 24+ hours.
7. Multiple supervisors submit simultaneously.
8. Worker monthly overtime exceeds allowed limit.

---

## Questions For Product Manager

1. Maximum overtime allowed per day?
2. Maximum overtime allowed per month?
3. Can overtime be edited later?
4. Who approves overtime?
5. Should overtime affect payroll immediately?
6. Can managers submit offline?

---

## Launch Blockers

- Wrong payroll calculation
- Duplicate overtime records
- Data loss during submission
- Unauthorized access

## V2 Enhancements

- Bulk upload
- Offline mode
- GPS verification
- Approval workflow
