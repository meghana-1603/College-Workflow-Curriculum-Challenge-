# AI-Assisted Exercise Verification Log

## Purpose

Document five AI-assisted learning exercises across programming, databases, machine learning, data quality, and generative AI/NLP.

## Important Note

The prompts and responses below were produced in this ChatGPT conversation on 22 October 2026. The results were checked through manual reasoning against the supplied code, synthetic data, calculations, or source passage. Local Java and SQL execution and independent review against course materials have not been completed. These limitations are stated honestly rather than presenting unperformed tests as completed.

## Shared Record Information

- **AI tool/model:** ChatGPT (GPT-6)
- **Date of AI responses:** 22 October 2026
- **Data used:** Self-created examples and synthetic data; no confidential information.
- **Verification approach:** Manual tracing, arithmetic, inspection of synthetic rows, and comparison with the supplied passage.
- **Evidence status:** This log records the responses and manual checks in this conversation. No separate screenshots or execution-result files are claimed.

---

## Exercise 1 — Programming / Data Structures

**Course:** CS101 Computer Programming or CS102 Data Structures; exact course placement should be checked against the applicable batch syllabus.

**Learning outcome:** Trace a loop, explain array operations, and determine program output.

### Task and prompt

Ask the AI to explain a short Java program, predict its output, and identify an edge case.

**Prompt used:**

> Explain this Java program line by line. Predict the exact output and explain why. Also identify one edge case or limitation.

```java
public class Main {
    public static void main(String[] args) {
        int[] numbers = {2, 4, 6, 8};
        int total = 0;

        for (int i = 0; i < numbers.length; i++) {
            total += numbers[i];
        }

        System.out.println(total);
        System.out.println(numbers.length);
    }
}
```

### Actual AI response

The array contains four integers: `2, 4, 6, 8`. The loop adds each element to `total`. Their sum is 20, and the array length is 4.

Expected output:

```text
20
4
```

An edge case is an empty array. The loop would execute zero times, so `total` would remain 0 and the array length would be 0.

### Verification

- **Method:** Manually traced the loop and calculated the sum.
- **Check:** \(2 + 4 + 6 + 8 = 20\); the array has four elements.
- **Result:** No error was found in the manual check.
- **Local execution:** Not performed; the expected output has not been confirmed by running a Java compiler.
- **What AI helped with:** Explaining loop execution and identifying an edge case.
- **Human judgment still required:** Running the program, checking compiler/runtime behaviour, and confirming that the explanation matches the observed output.
- **Evidence:** This conversation; no separate execution screenshot.

---

## Exercise 2 — Database Management Systems

**Course:** CS206 Database Management Systems.

**Learning outcome:** Write a `LEFT JOIN` query and understand join keys, unmatched rows, and `NULL` behaviour.

### Task and prompt

Use synthetic student and enrollment tables to count enrollments per student, including students with no enrollments.

**Prompt used:**

> Given these synthetic tables, write a SQL query that returns each student's name and enrollment count, including students with zero enrollments. Explain the join keys and NULL behavior.
>
> Students: `(1, 'Asha')`, `(2, 'Bilal')`, `(3, 'Chen')`
>
> Enrollments: `(1, 'AI')`, `(1, 'DBMS')`, `(2, 'AI')`, `(NULL, 'Cloud')`

### Actual AI response

```sql
SELECT s.name, COUNT(e.student_id) AS enrollment_count
FROM Students AS s
LEFT JOIN Enrollments AS e
    ON s.student_id = e.student_id
GROUP BY s.student_id, s.name
ORDER BY s.student_id;
```

Expected result:

| name | enrollment_count |
|---|---:|
| Asha | 2 |
| Bilal | 1 |
| Chen | 0 |

The join matches `Students.student_id` with `Enrollments.student_id`. The `LEFT JOIN` retains Chen even though no matching enrollment exists. `COUNT(e.student_id)` ignores `NULL`, giving Chen a count of zero. The enrollment row with a `NULL` student ID matches none of the listed students.

### Verification

- **Method:** Manually matched the enrollment rows to student IDs and checked the expected counts.
- **Result:** No error was found in the manual check.
- **SQL execution:** Not performed; the query has not been run in SQLite, MySQL, or PostgreSQL.
- **What AI helped with:** Query structure, join selection, grouping, and handling unmatched rows.
- **Human judgment still required:** Running the query against actual tables, checking the database dialect, and testing duplicate enrollment records.
- **Evidence:** This conversation; no separate database execution screenshot.

---

## Exercise 3 — Machine Learning

**Course:** DS304 Machine Learning.

**Learning outcome:** Select appropriate classification metrics and explain why accuracy may be misleading.

### Task and prompt

Consider a synthetic binary-classification dataset with 90 negative cases and 10 positive cases. The model predicts every case as negative, and missing a positive case is particularly costly.

**Prompt used:**

> A synthetic classification dataset has 90 negative cases and 10 positive cases. A model predicts every case as negative. Missing a positive case is particularly costly. Recommend suitable evaluation metrics, explain why accuracy alone can mislead, and identify possible data-leakage risks.

### Actual AI response

The model achieves 90% accuracy despite missing every positive case.

| Confusion-matrix measure | Result |
|---|---:|
| True positives (TP) | 0 |
| False negatives (FN) | 10 |
| False positives (FP) | 0 |
| True negatives (TN) | 90 |
| Accuracy | 90% |
| Positive-class recall | 0% |

Accuracy is misleading because the dataset is imbalanced and the model fails to identify any positive cases. Recall should be considered because missing positives is costly. Precision, specificity, and the precision-recall trade-off may also be useful. An F-beta score with beta greater than 1 may be appropriate if recall deserves greater weight, depending on the application.

Potential leakage risks include using information from the future, fitting preprocessing steps on the entire dataset before splitting, and placing related records in both training and test sets when a grouped split is needed.

### Verification

- **Method:** Manually calculated the metrics using the stated class counts.
- **Accuracy:** \((TP + TN)/100 = (0 + 90)/100 = 90\%\).
- **Recall:** \(TP/(TP + FN) = 0/(0 + 10) = 0\%\).
- **Result:** No error was found in the manual calculations.
- **Course-reference check:** Not yet completed against the applicable course notes or a separate authoritative ML reference.
- **What AI helped with:** Explaining metric selection and common leakage risks.
- **Human judgment still required:** Selecting the metric based on real error costs, validating assumptions, and checking the concepts against course material.
- **Evidence:** This conversation; no separate calculation screenshot.

---

## Exercise 4 — Data Wrangling / Big Data

**Course:** DS305 Data Wrangling and Visualization or DS307 Big Data Systems; exact course placement should be checked against the applicable batch syllabus.

**Learning outcome:** Identify data-quality problems and design a reproducible cleaning process without silently discarding records.

### Task and prompt

Use a synthetic table containing missing values, duplicate rows, an invalid date, and a negative amount.

**Prompt used:**

> For this synthetic table, propose data-quality checks and a reproducible cleaning plan. Do not silently delete rows. Explain how every change would be logged.

```text
id, date, amount
A1, 2026-01-03, 100
A2, 2026-01-04, NULL
A3, 2026-01-04, 50
A3, 2026-01-04, 50
A4, 2026-13-02, 70
A5, 2026-01-06, -5
```

### Actual AI response

1. **Missing amount:** Flag A2. Do not impute a value without an approved rule or supporting evidence.
2. **Possible duplicate:** The two A3 rows are identical. Check the business key and source before removing either row; identical values alone do not prove duplication.
3. **Invalid date:** A4 contains month 13, which is not a valid calendar month. Flag or quarantine it for correction.
4. **Negative amount:** A5 has amount `-5`. Confirm the business rules before treating this as invalid because refunds or adjustments can legitimately be negative.
5. **Reproducibility:** Preserve the raw data, record validation rules, log affected row IDs and changes, and produce a cleaned dataset with a change log.

### Verification

- **Method:** Manually inspected all six rows against the proposed checks.
- **Result:** A2 has a missing amount; A3 appears twice; A4 has an invalid month; A5 requires confirmation of the business rule.
- **Error found:** No error was found in the manual check. This does not establish that the plan has been tested on a running data pipeline.
- **Code execution:** Not performed.
- **What AI helped with:** Identifying candidate data-quality checks and proposing an auditable cleaning workflow.
- **Human judgment still required:** Establishing the true business key, deciding whether negative values are valid, and approving corrections.
- **Evidence:** This conversation; no separate dataset or execution screenshot.

---

## Exercise 5 — Generative AI / NLP

**Course:** DS408 Generative AI or DS311 Natural Language Processing; exact course placement should be checked against the applicable batch syllabus.

**Learning outcome:** Ground answers in a source passage, cite supporting text, and abstain when the answer is not provided.

### Task and prompt

Use a short, self-created passage and ask the AI two questions.

**Prompt used:**

> Answer using only the passage below. Cite the exact sentence supporting each factual claim. If the passage does not contain the answer, say “not stated.”
>
> Passage:
>
> The campus library opens at 8:30 a.m. on weekdays.
>
> Students may borrow up to four books for 14 days.
>
> The library is closed on Sundays.
>
> A valid student ID is required to borrow books.
>
> Questions:
>
> 1. How many books may a student borrow and for how long?
> 2. Is the library open on Saturday?

### Actual AI response

1. Students may borrow up to four books for 14 days. Supporting sentence: “Students may borrow up to four books for 14 days.”
2. Saturday opening status: **not stated**.

### Verification

- **Method:** Compared each answer with the supplied passage.
- **Result:** The borrowing limit and duration are explicitly stated. Saturday opening hours are not stated, so the response correctly abstains.
- **Error found:** No error was found in the manual check.
- **What AI helped with:** Extracting a grounded fact and identifying missing information.
- **Human judgment still required:** Checking that every claim is supported by the source and ensuring that unsupported details are not added.
- **Evidence:** This conversation; no separate screenshot.

---

## Summary Table

| Subject | Model/version | AI response date | Verification method | Error found/correction | Evidence |
|---|---|---|---|---|---|
| Programming / Data Structures | ChatGPT (GPT-6) | 22 Oct 2026 | Manual loop trace and arithmetic | No error found in manual check; local execution pending | This conversation |
| DBMS | ChatGPT (GPT-6) | 22 Oct 2026 | Manual join and row-count check | No error found in manual check; SQL execution pending | This conversation |
| Machine Learning | ChatGPT (GPT-6) | 22 Oct 2026 | Confusion-matrix calculations | No error found in manual calculations; course-reference check pending | This conversation |
| Data Wrangling / Big Data | ChatGPT (GPT-6) | 22 Oct 2026 | Manual inspection of synthetic rows | No error found in manual check; code execution pending | This conversation |
| Generative AI / NLP | ChatGPT (GPT-6) | 22 Oct 2026 | Claim-to-source comparison | No error found in manual check | This conversation |

## Overall Findings and Limitations

- Five AI-assisted exercises were completed in this conversation, with prompts, responses, and manual verification notes recorded.
- The manual checks support the stated expected outputs, SQL result counts, classification metrics, data-quality observations, and passage-grounded answers.
- These checks are not equivalent to independent execution in a Java environment, SQL database, or data-processing pipeline.
- The machine-learning exercise has not yet been checked against separate course notes or an authoritative reference.
- No separate screenshots or execution-result files are claimed.
- The log should be updated if further local tests or independent reference checks are performed.

**Evidence integrity statement:** The records above describe the AI responses and manual checks actually performed in this conversation. They do not claim local execution or independent testing that has not occurred.