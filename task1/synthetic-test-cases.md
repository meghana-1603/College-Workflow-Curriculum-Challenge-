# Task 1: Synthetic Test Cases
## Proposed Club Event Approval Status Tracker

**Purpose:** Define expected behaviour for a proposed tracker before any permitted pilot.

**Important:** These are hypothetical test cases. They have not been executed against a real tracker or university system.

| Test ID | Scenario | Input / action | Expected result | Recovery or control |
|---|---|---|---|---|
| TC01 | Normal status update | An authorized updater records a confirmed forwarding action and its date | The current status and last-updated date reflect the confirmed action | Retain the change history where supported |
| TC02 | Missing information | A user attempts to mark a submission complete without a required field | The entry is flagged as incomplete and is not represented as a complete submission | Ask the responsible user to provide the missing information |
| TC03 | Duplicate event | A user creates another entry with an existing event reference | The duplicate is detected or flagged for review | Check the existing entry before creating another record |
| TC04 | Unauthorized approval | A user without approval authority attempts to record an official decision | The action is rejected or escalated; the last confirmed official status remains unchanged | Refer the matter to an authorized person |
| TC05 | Failed update | An update cannot be saved because of an error or connectivity issue | The last confirmed status is preserved; the failed update is not presented as successful | Show the failure, allow retry, and retain the existing official process as a fallback |

## Test boundaries

- No test may create a real approval or alter a university record.
- Only authorized people may record official decisions.
- A forwarded proposal must not be treated as approved.
- If the tracker is stale or unavailable, users must follow the existing official process.
- Any future live test requires appropriate permission.
- Results must be recorded only after the tests are actually performed; expected outcomes are not evidence of successful execution.

## Acceptance criteria for a future permitted pilot

The proposed tracker should be considered for continued use only if:

1. Confirmed status updates can be distinguished from pending or unverified information.
2. Unauthorized users cannot record official decisions.
3. Failed updates do not overwrite the last confirmed status.
4. Duplicate and incomplete entries can be identified and corrected.
5. Maintenance effort and status accuracy can be measured.
6. The tracker does not replace or interfere with the university's official approval process.

If the tracker is unreliable, creates unacceptable access or privacy risks, or does not save measurable effort, it should be revised or abandoned.
