# Task 1: Investigating and Improving a College Workflow
## A Study of the Club Event Approval Process at ICFAI University Hyderabad

**Prepared by:** Meghana Dasari  
**Evidence log prepared:** 21 October 2026  
**Scope:** Investigation and proposed improvement; no live system implemented

## 1. Executive Summary

This report examines the club event approval process at ICFAI University Hyderabad, based on my experience as a Game Development Club student leader. The aim is to identify whether clearer status visibility could reduce uncertainty and repeated follow-up while preserving the university’s existing approval authority.

The process involves event planning, communication with the club mentor, preliminary discussion with the Student Affairs Dean, submission of event and budget forms, signatures, forwarding to the Director, and final approval before the event takes place.

Waiting for approvals and making budget or form corrections are practical difficulties I have encountered. I propose a simple status tracker as a possible improvement. It would record confirmed stages and updates; it would not replace any official approval, change decision-making authority, or guarantee faster decisions.

The investigation is limited. It uses two past event examples, with submission dates checked against proposal files and approval dates recalled from memory. Follow-up counts, time spent on rework, annual event volume, and potential savings have not been measured reliably. Therefore, the proposal should be evaluated through a small, permission-based pilot before any decision to adopt it.

## 2. Scope and Current Workflow

### 2.1 Workflow observed through personal experience

The current process, as I understand and have experienced it, is:

1. The club head plans an event with club members.
2. The club head informs the club mentor.
3. A preliminary discussion takes place with the Student Affairs Dean to check whether the event is acceptable.
4. The event proposal and budget forms are submitted to the Dean.
5. The club mentor and Dean sign the forms.
6. The Dean forwards the proposal to the Director.
7. The event is conducted after approval is received.

The proposal should generally be submitted about one week before the planned event. Both physical and digital submission methods have been used.

### 2.2 Scope boundaries

This investigation focuses on the visibility of a proposal’s status and the effort involved in following up. It does not assess individual staff performance, challenge the approval hierarchy, or assume that every delay is avoidable.

The proposed tracker would document only confirmed information and would not treat a submission, signature, or forwarding action as final approval.

## 3. Investigation Method and Confirmed Findings

The report is based on personal experience, two event proposal files, and permission requested from the club mentor to discuss the general workflow. Permission was granted, but a complete formal interview record or independently verified process-time dataset is not available. The report therefore does not present the permission discussion as a completed formal interview.

The two event examples are used to describe the process, not to establish a university-wide average.

| Finding | Evidence status |
|---|---|
| The two proposal submission dates | Checked against the available proposal files |
| Final approval dates for the two examples | Recalled from memory; not independently verified |
| The approval stages described in Section 2 | Based on personal experience |
| Waiting and budget/form corrections as difficulties | Based on personal experience |
| Typical approval time of about one week | Personal estimate, not measured across a representative sample |
| Follow-up frequency and time spent | Not reliably recorded; excluded from confirmed findings |
| Annual proposal volume and potential savings | Estimates only; require measurement |

## 4. Dated Evidence Log Summary

### Event example A: E-Sports Tournament 2026

- Submission date: 11 February 2026, checked against the proposal file.
- Final approval date: 23 February 2026, recalled from memory.
- Elapsed calendar time between these dates: 12 days.
- Corrections: No corrections recalled.
- Main observation: The process included a wait for Director approval.
- Effect on registration or event delivery: No significant quantified impact is available.

### Event example B: Campus Master League 2026

- Submission date: 17 July 2026, checked against the proposal file.
- Final approval date: 23 July 2026, recalled from memory.
- Elapsed calendar time between these dates: 6 days.
- Corrections: No corrections recalled.
- Main observation: The process was completed within the recalled period.
- Effect on registration or event delivery: No significant quantified impact is available.

These dates describe two individual cases only. Since the approval dates are recalled rather than documented, the elapsed periods should be treated as approximate. They do not establish the average approval time for all college events.

## 5. Operational Problem and Scale of Effort

The main improvement opportunity is **status visibility**, rather than assuming that approval itself can be accelerated by software.

When the current stage or latest confirmed update is unclear, a club representative may need to ask for information again. A tracker could make the latest recorded status easier to check and could reduce avoidable status enquiries if authorized users maintain it.

Budget or form corrections may still be necessary. A tracker cannot remove the need to correct incomplete or inaccurate information, and it cannot control when an authorized person reviews or approves a proposal.

The current evidence is insufficient to calculate the actual time lost to follow-ups or corrections. No follow-up visit counts or time totals are claimed in this report.

For planning purposes only, the annual proposal volume has previously been estimated at approximately 4–6 events, but this has not been verified against an annual register. This estimate must not be treated as a measured workload figure.

## 6. Proposed Improved Workflow

### 6.1 Proposed tracker

A basic spreadsheet with restricted editing access could record:

- Event reference or title
- Proposal submission date
- Current confirmed status
- Date of the latest update
- Date forwarded to the Director, only when confirmed
- Whether a correction has been requested
- Official decision and decision date, once confirmed
- Updating role
- Change history or update notes

The tracker should store only information needed to manage the workflow. It should not contain unnecessary personal information, private contact details, signatures, or confidential documents.

### 6.2 Suggested status values

1. Preparing Forms
2. Submitted
3. Awaiting Required Signatures
4. Forwarded to Director
5. Pending Director Approval
6. Correction Required
7. Approved
8. Not Approved

Only an authorized person should record an official decision. A status such as “Forwarded to Director” must not be displayed as “Approved.”

### 6.3 Proposed process

1. The club representative prepares and submits the required forms using the existing process.
2. An authorized person records the submission and its confirmed status in the tracker.
3. When a signature, forwarding action, correction request, or decision is confirmed, an authorized updater records the change and date.
4. Club representatives check the tracker before making another status enquiry.
5. If the status is stale, unclear, or unavailable, the tracker directs the user to follow the existing official process.
6. The tracker is reviewed after a permitted pilot to decide whether it saves effort and remains accurate.

### 6.4 Why a simple solution is preferable

A spreadsheet is a suitable first proposal because the workflow is small and rule-based. A complex application or AI system is not justified by the current evidence. The first objective is to test whether a simple, maintained status record is useful.

## 7. Synthetic Test Cases

The following are hypothetical tests for the proposed tracker, not tests conducted on a real university system.

| Test | Scenario | Expected result |
|---|---|---|
| 1. Normal update | An authorized updater records a confirmed forwarding action | Status and update date are recorded accurately |
| 2. Missing information | A required submission field is missing | The entry is flagged as incomplete; it is not represented as a complete submission |
| 3. Duplicate entry | The same event reference is entered twice | The duplicate is flagged for review rather than creating conflicting records |
| 4. Unauthorized approval | An unauthorized user attempts to record an approval | The action is rejected or escalated; the official status remains unchanged |
| 5. Failed update | A status update cannot be saved | The last confirmed status is preserved, the failure is indicated, and the user can retry or use the existing process |

These tests describe expected behaviour only. They do not demonstrate that a tracker has been built, deployed, or validated.

## 8. Estimated Net Time Savings

A reliable savings figure cannot be calculated from the available evidence. Follow-up visit counts, actual duration, correction effort, tracker maintenance, and support requirements were not measured.

A future pilot could record:

- Time spent on status enquiries before the tracker
- Time spent checking the tracker and following up afterward
- Time required to enter and maintain updates
- Number of stale or incorrect status entries
- Time spent correcting forms, separately from status enquiries

The relevant calculation would be:

**Net time saved = follow-up time avoided − setup effort − maintenance effort − support and review effort.**

If a future pilot assumes that some follow-up effort can be avoided, that assumption must be labelled and compared against measured results. No percentage reduction or net savings is claimed in this report.

## 9. Risks, Unknowns, and Abandonment Criteria

| Risk or unknown | Mitigation or decision rule |
|---|---|
| Outdated status | Show the last update date and flag stale entries |
| Incorrect approval status | Allow only authorized roles to record official decisions |
| Additional administrative effort | Keep fields minimal and measure upkeep time |
| Privacy or access concerns | Obtain permission and restrict access to appropriate users |
| False confidence in the tracker | State clearly that the official approval process remains authoritative |
| Small evidence sample | Gather more examples before making broad claims |
| Unmeasured follow-up and correction effort | Record actual time during a permitted pilot |
| No improvement in decision speed | Evaluate status visibility separately from approval turnaround |

The tracker should be revised or abandoned if it is unreliable, creates unacceptable privacy or access risks, or requires as much or more effort to maintain than the effort it demonstrably saves. Any pilot would require appropriate permission and agreement from the responsible people.

## 10. Permission, Privacy, and Fieldwork Boundaries

The work is limited to my own experience and general workflow information that I am permitted to discuss. The permission received to discuss the general process does not automatically authorize access to internal records, implementation, or a live pilot.

No private student information, staff names, signatures, confidential forms, or internal records should be uploaded to a public repository. The synthetic tests use hypothetical scenarios. Any future collection of timestamps or pilot measurements would require permission and should use only the minimum information needed.

The proposed tracker is a recommendation, not a system currently in use. No deployment, live integration, or measured outcome is claimed.

## Conclusion

The club event approval workflow has multiple legitimate review and authorization stages. The improvement opportunity identified here is to make confirmed status information easier to check, while preserving the existing decision-making process.

A simple tracker may be worth testing, but the present evidence is not sufficient to claim that it will reduce approval time or produce a specific amount of savings. The next responsible step would be to obtain permission for a small pilot, measure the effort and accuracy, and continue only if the results justify the additional work.

This report presents a limited, experience-based investigation and a testable proposal, not a claim that the university’s existing process is defective.
