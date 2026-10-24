# AI Exercise Log

## Purpose

This log documents five AI-assisted exercises covering core Computer Science subjects. Each exercise includes the problem, solution, expected result, and key learning.

## Exercise 1: Data Structures — Linear Search and Binary Search

**Problem:** Find the number `40` in a sorted list using linear search and binary search.

**Code:**

```python
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1


def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) // 2

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1

    return -1


numbers = [10, 20, 30, 40, 50]

print("Linear Search:", linear_search(numbers, 40))
print("Binary Search:", binary_search(numbers, 40))
```

**Expected output:**

```text
Linear Search: 3
Binary Search: 3
```

**Result:** Both algorithms are designed to return index `3` for the target value `40`.

**Learning:** Linear search checks elements sequentially. Binary search repeatedly halves the search range and requires sorted input.

## Exercise 2: DBMS — Aggregate Functions and HAVING

**Problem:** Calculate the average salary in each department and display only departments with an average salary greater than 50,000.

**SQL query:**

```sql
SELECT department_id, AVG(salary) AS average_salary
FROM employees
GROUP BY department_id
HAVING AVG(salary) > 50000;
```

**Expected result:** The query returns departments whose average salary exceeds 50,000, provided the table and columns exist.

**Result:** The query uses `GROUP BY` to group employees by department, `AVG()` to calculate the average, and `HAVING` to filter grouped results.

**Learning:** `WHERE` filters individual rows before grouping, while `HAVING` filters groups after aggregation.

## Exercise 3: AI/ML — Understanding Overfitting

**Problem:** Explain overfitting and identify methods to reduce it.

**Solution:** Overfitting occurs when a model learns the training data too closely, including noise and unimportant patterns. It performs well on training data but poorly on unseen data.

**Methods to reduce overfitting:**
1. Use more representative training data.
2. Apply regularization.
3. Use dropout in suitable neural networks.
4. Reduce model complexity.
5. Apply cross-validation.
6. Use early stopping when appropriate.

**Result:** The explanation distinguishes training performance from generalization and identifies common techniques to reduce overfitting.

**Learning:** A good machine learning model should perform well on unseen data rather than simply memorize training examples.

## Exercise 4: Operating Systems — Process vs Thread

**Problem:** Explain the difference between a process and a thread.

| Process | Thread |
|---|---|
| A program in execution with its own address space and resources. | An execution unit within a process. |
| Processes generally have separate address spaces. | Threads in the same process share memory and many resources. |
| Communication often requires inter-process communication mechanisms. | Threads can communicate through shared memory. |
| Process management may involve greater overhead. | Thread management can involve lower overhead, depending on the system. |

**Result:** Processes provide isolation, while threads allow concurrent execution within a process and can share resources.

**Learning:** Shared memory between threads requires appropriate synchronization to prevent race conditions.

## Exercise 5: Software Engineering and Testing — Milestone Tracker

**Problem:** Define test cases for a student project milestone tracker.

| Test case | Input or action | Expected result |
|---|---|---|
| Valid submission | Enter all required fields | Submission is accepted |
| Missing information | Leave a required field empty | Submission is rejected with a clear message |
| Duplicate submission | Submit the same milestone details again | Duplicate is detected according to defined rules |
| Unauthorized approval | A student attempts to approve a milestone | Approval is denied |
| Error recovery | Submit empty replacement content | Invalid content is rejected and existing valid content is preserved |

**Result:** These test cases define expected behavior for validation, duplicate detection, authorization, and error recovery.

**Learning:** Testing helps identify defects and check whether the software behaves according to its requirements. A browser role selector alone does not provide production-level security.

## Overall Summary

The five exercises demonstrate how AI assistance can support learning in Data Structures, DBMS, AI/ML, Operating Systems, and Software Engineering.

The exercises provide examples of algorithm implementation, SQL queries, conceptual explanations, and software test design. Code outputs and prototype behavior should be confirmed in the relevant environment before being reported as executed tests.

## Limitations

- The examples are educational and may require adaptation to the available environment.
- SQL output depends on the data stored in the database.
- AI-generated explanations should be reviewed for technical accuracy.
- Expected results describe intended behavior and are not, by themselves, evidence of execution.
 checks have been completed.
