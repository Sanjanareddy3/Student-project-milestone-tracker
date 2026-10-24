# Task 1 test results — fill after running the prototype

**Important:** Do not mark tests as passed until you run the prototype and observe the result. The entries below are a recording template, not claims that tests have already passed.

Run `task-1/student_milestone_tracker.html` in a browser, click **Run 5 test scenarios**, and record the visible output. If a scenario is not implemented or the outcome differs from expectations, report that honestly.

| # | Scenario | Expected behavior | Actual observed result | Status |
|---|---|---|---|---|
| 1 | Normal request | Valid unique submission is accepted and status changes to Submitted. | Fill after running | Not run |
| 2 | Missing information | Submission is blocked and the missing field is identified. | Fill after running | Not run |
| 3 | Duplicate | Duplicate project/milestone/owner combination is detected; original record is preserved. | Fill after running | Not run |
| 4 | Unauthorized approval | Student role cannot approve; status remains unchanged. | Fill after running | Not run |
| 5 | Failed step / recovery | Empty submission is rejected; prior valid data is preserved where possible and a clear error is shown. | Fill after running | Not run |

## Run details

- Date/time run:
- Browser/version:
- Test runner output:
- Any failed or unexpected behavior:
- Corrective change made (if any):
- Retest result:

## Limitations

The prototype's role selector is a demonstration control, not real authentication. Local browser storage is not a tamper-proof audit system. A production implementation would need server-side authorization, durable storage, backups and error handling.
