# AI-Assisted Learning Exercise Log

## Objective

Evaluate how AI tools can support learning in five computer science subjects. Each exercise records the prompt, an illustrative output, a verification method, and corrections or limitations.

**Status:** Planned examples — complete the verification checks before marking these exercises as completed.

## Exercise 1: Data Structures and Algorithms

### Prompt

"Explain the time complexity of linear search and binary search. Provide a Python example of each and explain when binary search can be used."

### Illustrative AI output

- Linear search checks elements one by one and takes O(n) time in the worst case.
- Binary search repeatedly halves the search interval and takes O(log n) time.
- Binary search requires sorted data.

### Verification

1. Run both implementations on the same test array.
2. Test successful and unsuccessful searches.
3. Check the time-complexity claims against the algorithm logic and a trusted algorithms textbook or course resource.

### Correction and learning

Binary search must not be applied directly to an unsorted array unless the data is sorted first or another suitable strategy is used. Sorting also has a cost that may matter in a real application.

### Status

Pending practical verification.

---

## Exercise 2: Database Management Systems

### Prompt

"Write an SQL query to calculate the average salary in each department using an employees table with department_id and salary columns. Explain GROUP BY and HAVING."

### Illustrative AI output

```sql
SELECT department_id, AVG(salary) AS average_salary
FROM employees
GROUP BY department_id;
```

To display only departments with an average salary greater than 50000:

```sql
SELECT department_id, AVG(salary) AS average_salary
FROM employees
GROUP BY department_id
HAVING AVG(salary) > 50000;
```

### Verification

1. Run the queries in a database containing sample employee records.
2. Calculate one department's average manually.
3. Confirm that HAVING filters grouped results, while WHERE filters rows before grouping.

### Correction and learning

The example assumes the table and column names exist and that salary values use a suitable numeric type. Departments with no employee records will not appear in this result.

### Status

Pending database execution.

---

## Exercise 3: Artificial Intelligence and Machine Learning

### Prompt

"Explain overfitting in machine learning and suggest three methods to reduce it. Give a simple example."

### Illustrative AI output

Overfitting occurs when a model learns the training data too closely, including noise, and performs poorly on unseen data.

Possible methods to reduce overfitting include:
1. Regularization.
2. Cross-validation and appropriate model selection.
3. Early stopping or collecting more representative training data.

### Verification

1. Consult a trusted machine-learning textbook or course resource.
2. Train a simple model and compare training performance with validation performance.
3. Check that validation data is not used to fit the model's parameters.

### Correction and learning

A large gap between training and validation performance can indicate overfitting, but it is not conclusive by itself. Data leakage, distribution differences, and other issues should also be considered.

### Status

Pending practical experiment.

---

## Exercise 4: Operating Systems

### Prompt

"Explain the difference between a process and a thread. Give one example of each and describe one advantage of multithreading."

### Illustrative AI output

- A process is a running program with its own process-level resources and address space.
- A thread is an execution unit within a process. Threads in the same process typically share its address space.
- Multithreading can improve responsiveness and allow concurrent work.

### Verification

1. Compare the definitions with the operating-systems textbook or course notes.
2. Use a simple multithreaded program to observe concurrent execution.
3. Check the program's output and distinguish concurrency from guaranteed parallel execution.

### Correction and learning

Multithreading does not automatically make every program faster. Shared data may require synchronization, and threads can introduce race conditions.

### Status

Pending practical verification.

---

## Exercise 5: Software Engineering and Testing

### Prompt

"Suggest test cases for a student project milestone tracker that accepts milestone submissions and allows authorized users to approve them."

### Illustrative AI output

| Test case | Expected result |
|---|---|
| Submit a valid milestone | Submission is accepted |
| Submit without a required field | Validation error is displayed |
| Submit a duplicate milestone | Duplicate is rejected or handled according to defined rules |
| Approve as an unauthorized user | Approval is denied |
| Recover from a simulated error | A useful error message is shown and the application remains usable where possible |

### Verification

1. Execute each test against the actual milestone tracker.
2. Record the observed result and compare it with the expected result.
3. Investigate any mismatch and retest after a correction.
4. Distinguish interface-demo behavior from real authentication and server-side enforcement.

### Correction and learning

A role selector in a front-end prototype is not secure authentication. A production application must enforce permissions on the server or another trusted backend.

### Status

Pending execution against the prototype.

---

## Overall Reflection

AI can help explain concepts, generate starter code, and suggest test cases. However, its responses can contain errors, omit assumptions, or overlook security issues.

For reliable use:
- Verify code by executing it.
- Check explanations against trusted learning resources.
- Record actual results rather than assumed results.
- Document corrections and limitations.
- Do not treat an AI-generated answer as evidence that a system works.

## Evidence to Add

For each exercise, retain the actual prompt and response, a screenshot or output from the verification process, and any correction made. Update each status only after the corresponding checks have been completed.
