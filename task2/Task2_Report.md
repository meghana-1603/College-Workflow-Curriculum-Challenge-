# Task 2 — Curriculum Audit and Redesign for 2030

**Student proposal, not an official ICFAI syllabus revision**

**Student:** Meghana Dasari  
**Campus/programme:** ICFAI University Hyderabad, ICFAITech School  
**Degree/branch:** B.Tech in Data Science & Artificial Intelligence  
**Admission batch:** 2023–2027  
**Curriculum version**: Course names and credits are based on my academic record. The proposed changes should be checked against the official curriculum and regulations applicable to the 2023–2027 batch before implementation.
**Evidence access date:** 22 October 2026. URLs and source-status notes are recorded in `../sources/references.md`.

## Executive summary

This proposal preserves mathematics, programming, algorithms, databases, operating systems, networks, machine learning and other foundational subjects while recommending more assessed practice in software testing, data engineering, cloud delivery, generative-AI evaluation and responsible AI.

The proposal uses an **overall academic baseline of 166 credits**. The listed Semester I–VIII course totals add up to **163 credits**; IP201 — Internship-I contributes another **3 academic credits**, giving 166 credits overall. Internship-I is part of the academic programme, not an additional component outside it. This remains a planning baseline pending verification against the official curriculum applicable to the 2023–2027 batch.

## 1. Starting point and confidence

The student-record map in `curriculum-map.md` is the working baseline. Semesters I–VI total 132 listed course credits/units. Semester VII has 16 listed credits, including Professional Ethics (3) and Computer Vision (provisionally 3). Semester VIII internship is reported as 15 credits. Thus, Semesters I–VIII total 163 listed credits.

The 166-credit planning baseline comprises the 163 listed Semester I–VIII credits and 3 academic credits for IP201 — Internship-I. Semester-level totals are preserved as supplied. The applicable batch syllabus and regulations must be checked before the calculation is treated as an officially verified programme-credit total.

The official IFHE/ICFAITech pages identify public curriculum resources, but the publicly available structure and older programme PDF have not yet been conclusively shown to match this student's admission batch. The current admissions page alone is not sufficient proof.

## 2. Recommendation set: 12 specific reasons

| # | Course/reference | Action | Evidence-based rationale and proposed change |
|---:|---|---|---|
| 1 | CS101 Computer Programming; CS102 Data Structures; CS201 OOP; CS203 Design and Analysis of Algorithms | KEEP | These provide programming and problem-solving foundations for software, data and AI roles. Preserve outcomes and prerequisite progression. |
| 2 | CS206 DBMS; CS302 Operating Systems; CS306 Computer Networks | KEEP | Data persistence, systems concepts and networking remain useful foundations for production applications and data pipelines. |
| 3 | MA101/MA102/MA202; ML201 | KEEP | Linear algebra, calculus, discrete mathematics and ML mathematics underpin AI/ML methods. Do not remove mathematics merely to make room for trends. |
| 4 | DS202 Industry Coding Practice (Python/R) | UPDATE | Require Git-based collaboration, unit tests, debugging, code review, readable documentation and reproducible runs as assessed deliverables. |
| 5 | CS205 Web-Enabled Technologies | UPDATE | Add API contracts, authentication/authorization, validation, automated API tests, error handling and secure configuration to a practical assessment. |
| 6 | DS305 Data Wrangling and Visualization | UPDATE | Assess data profiling, missing/duplicate/outlier handling, schema validation, reproducible transformations and communication of limitations. |
| 7 | DS307 Big Data Systems | UPDATE | Include a small end-to-end pipeline with ingestion, transformation, data-quality checks, orchestration concepts and cost/performance trade-offs. |
| 8 | CS307 Cloud Computing; verify code, title and credits against the batch syllabus | UPDATE | Assess deployment architecture, IAM/access control, logs/monitoring, cost awareness, backup/recovery and a documented deployment or equivalent lab. |
| 9 | DS408 Generative AI; verify provisional code | UPDATE | Add retrieval/grounding, evaluation sets, hallucination/error analysis, privacy, prompt-injection awareness and human verification. A demo alone is insufficient evidence of quality. |
| 10 | DS304 Machine Learning; DS306 Deep Learning; DS311 NLP; ML303 Reinforcement Learning | UPDATE | Keep core theory; require baseline comparisons, data-leakage checks, appropriate metrics, error analysis, reproducible experiments and documented limitations. |
| 11 | Proposed software testing/CI practice | ADD, conditional | If no equivalent compulsory assessed coverage exists, add a small lab/module or embed equivalent assessed work in existing coding/web courses. Check the published programme's existing Software Testing course before adding a duplicate. |
| 12 | Proposed data engineering and responsible-AI assessment, integrated with the Task 1 workflow capstone | ADD, conditional | Add assessed pipeline/data-quality and AI-governance tasks through an elective, lab or capstone where credit rules permit. If new credits are not permitted, replace a duplicative assessment or use an approved interdisciplinary elective. |

### REDUCE decisions

No existing course is marked REDUCE. A reduction should only be proposed after reviewing the actual syllabus, learning outcomes, contact hours and assessments. A safe conditional option is to reduce duplicated introductory tool demonstrations—not core theory or required outcomes—if a documented content-overlap audit confirms duplication. Record the affected course/topic and hours after reviewing the official course descriptions. Do not invent a reduction or claim a subject is obsolete.

## 3. Job-description comparison

See `job-description-comparison.md` for dated public postings and the requirement-to-course-gap matrix. These postings are market signals, not a representative survey of all entry-level hiring. At least one source is a role labelled “AI Engineer” and may be more experienced than a new graduate; it should not be presented as an entry-level eligibility guarantee.

## 4. AI-assisted exercises and verification

Five subject-specific AI-assisted exercises are documented in ai-verification-log.md: Java programming, SQL joins, machine-learning evaluation, data wrangling and grounded question answering.

The exercises were completed in this ChatGPT conversation on 22 October 2026 using ChatGPT (GPT-6). The log records the prompts, expected or generated results, verification approach and limitations for each exercise. The results were checked through manual reasoning, calculations or comparison with the supplied passage, as appropriate.

Verification limitations: Local Java and SQL execution was not performed, and independent verification against the applicable official course materials remains incomplete. These exercises demonstrate examples of AI-assisted learning and verification, not independently established subject proficiency. No exercise output, execution result or error is claimed beyond what is documented in the log.

Only synthetic or non-confidential examples were used. The recorded limitations must be considered when interpreting the evidence.

## 5. Proposed credit changes and feasibility

See `credit-plan.md` and the interactive `course-comparison/index.html`.

The planning calculation uses an overall academic baseline of 166 credits. The listed Semester I–VIII courses total 163 credits, and semester-level totals remain as shown in the curriculum map.

The affected-course set consists of these 11 existing courses:

- DS202 — Industry Coding Practice (Python/R): 3 credits
- CS205 — Web-Enabled Technologies: 4 credits
- DS304 — Machine Learning: 3 credits
- DS305 — Data Wrangling and Visualization: 3 credits
- DS306 — Deep Learning: 4 credits
- DS307 — Big Data Systems: 3 credits
- SP301 — Special Project: 3 credits
- DS311 — Natural Language Processing: 3 credits
- ML303 — Reinforcement Learning: 3 credits
- CS307 — Cloud Computing: 4 credits
- DS408 — Generative AI: 3 credits

**Affected credits:** 36  
**Overall academic baseline:** 166  
**Affected-credit share:** 36 ÷ 166 × 100 = **21.69%**

The affected credits represent courses whose assessed outcomes are proposed for improvement. They are not additional credits, and the proposal does not claim that new credits have been approved.

Before final submission:

1. Verify the official denominator against the applicable batch syllabus and regulations.
2. Confirm required credits and select only one valid option from each mutually exclusive elective group; do not sum all elective choices.
3. Identify updated, reduced and added credits separately, avoiding double-counting.
4. Confirm that unchanged and changed credits reconcile with the approved programme total.
5. If regulations prevent a new credit-bearing course, propose an equivalent assessment or approved elective route.

The interactive calculator is editable for transparent planning; it does not establish official approval.

## 6. Task 1-derived proposed lab/capstone

**Proposed title:** Approval Workflow Tracker and Exception-Handling Lab

**Host course:** CS205 Web-Enabled Technologies or an approved software engineering/project lab. Host selection is conditional on verification of the curriculum.

**Prerequisite knowledge:** Programming fundamentals, relational data modelling, web/API basics, authentication, Git and basic testing.

**Learning outcomes:**

1. Model a multi-stage approval workflow.
2. Enforce role-based actions.
3. Preserve the last confirmed state after a failed update.
4. Detect missing and duplicate data.
5. Test and document workflow behaviour.
6. Calculate value using measured observations rather than assumptions.

**Synthetic dataset:** Invented event IDs, proposal dates, status transitions, role IDs, missing-field flags and simulated update failures. No real student, staff, signature, budget or confidential event records.

**Milestones:**

- M1: Workflow and data dictionary.
- M2: Schema/API and role rules.
- M3: User interface and status tracker.
- M4: Automated tests and failure recovery.
- M5: Evaluation, limitations and demonstration.

**Acceptance tests:**

- A valid, authorized transition succeeds.
- Unauthorized approval is rejected.
- Missing required fields are rejected with actionable feedback.
- Duplicate submission is handled safely.
- A failed update leaves the last confirmed state intact and permits retry.
- The audit log records actor/action/time using synthetic IDs.
- The value calculation reports baseline and observed follow-up effort separately.

**Measured-value rule:** Time saved = measured follow-up effort avoided − setup effort − maintenance effort − support/review effort. If no controlled measurement is conducted, report the calculation method only and claim no savings.

## 7. Validation, strongest claim and limitations


**Feedback status**: No faculty or recent-graduate feedback has been obtained or documented. Therefore, the recommendations have not been externally validated. The proposal remains based on the student's academic-record course map, available public curriculum references, the limited job-posting sample and the proposed assessment improvements.

**What would change my mind**: Evidence that the current course already assesses a proposed skill deeply and consistently would change an ADD recommendation to KEEP or UPDATE. Evidence of prerequisite or regulatory constraints would favour an embedded assessment or approved elective instead of a new course.

**Evidence that could disprove the strongest claim**: A batch-specific syllabus and assessment rubrics showing that software testing, data quality, production data pipelines, cloud operations and responsible-AI evaluation are already taught and assessed to an adequate depth.

**Limitations**:

The course map is transcribed from the student's academic record.

The official curriculum version applicable to the 2023–2027 batch has not yet been conclusively matched.

The listed Semester I–VIII totals are 163 credits, while the overall academic baseline used for planning is 166 credits.

The job-description sample is small; postings may expire or target experienced applicants.

AI-assisted exercises were manually checked, but local Java/SQL execution and independent course-reference verification remain incomplete.

Faculty and recent-graduate feedback has not been obtained or documented.

No real time-savings measurement has been conducted.

The proposal is not an official university decision.

## Appendices

- Full student-record course map: `curriculum-map.md`
- Job requirements and dated sources: `job-description-comparison.md`
- Five AI verification records: `ai-verification-log.md`
- Editable credit assumptions and calculator: `credit-plan.md`, `course-comparison/index.html`
- Official references and access date: `../sources/references.md`
