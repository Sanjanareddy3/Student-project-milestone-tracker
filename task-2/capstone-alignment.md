# Capstone Alignment: Student Project Milestone Tracker

## 1. Project Overview

The Student Project Milestone Tracker is a browser-based prototype designed to help students and faculty supervisors track project milestones, submissions, deadlines, feedback, and approvals.

The project demonstrates how Computer Science concepts can be applied to a practical academic workflow.

## 2. Alignment with CSE Courses

| Course | Concepts Applied | Project Connection |
|---|---|---|
| Data Structures | Searching, filtering, and organizing records | Finding milestones and filtering project information |
| Object-Oriented Programming | Encapsulation, modularity, and reusable logic | Organizing application functionality into manageable components |
| Database Management Systems | Data modelling, keys, validation, and queries | Designing a persistent database for projects and milestones |
| Web Technologies | HTML, CSS, and JavaScript | Building the browser interface and interactive features |
| Software Engineering | Requirements, design, implementation, and maintenance | Developing the tracker using a structured workflow |
| Software Testing | Test cases, validation, and error handling | Checking valid submissions, missing fields, duplicates, and recovery |
| Artificial Intelligence | Text summarization and classification concepts | Potential future support for summarizing non-confidential feedback |
| Cloud Computing | Hosting, storage, access management, and deployment | Potential future deployment as a shared online application |

*Note: The course mapping is provisional and should be checked against the curriculum applicable to the 2023 admission batch.*

## 3. Learning Outcomes

The project supports the following learning outcomes:

1. Translate a practical problem into functional requirements.
2. Design an interface for different user roles.
3. Apply input validation and duplicate detection.
4. Define milestone statuses and approval workflows.
5. Create and evaluate test cases.
6. Identify security, reliability, and data-management limitations.
7. Propose improvements based on user needs and technical constraints.

## 4. Current Prototype Features

The prototype demonstrates:

- Milestone creation and submission.
- Required-field validation.
- Duplicate detection.
- Simulated student and faculty-supervisor workflows.
- Approval and revision states.
- Audit history and test scenarios.

## 5. Current Limitations

The prototype uses browser-side storage and simulated roles. It does not provide genuine authentication, secure server-side authorization, centralized database persistence, cloud backup, or institutional integration.

The demonstration is intended for synthetic data only. The role selector should not be treated as a production security mechanism.

## 6. Proposed Future Improvements

| Area | Proposed improvement | Benefit |
|---|---|---|
| Database | Integrate a relational database | Persistent and structured records |
| Authentication | Implement secure login and role-based authorization | Protect student and supervisor actions |
| Testing | Add automated unit and integration tests | Improve reliability |
| Reporting | Add progress dashboards and overdue summaries | Make project status easier to monitor |
| Notifications | Add deadline reminders | Help users track upcoming milestones |
| AI assistance | Offer optional summaries of non-confidential feedback | Make lengthy feedback easier to review |
| Cloud deployment | Host the application using an appropriate cloud service | Enable authorized access across devices |

AI features should remain optional, and important approval decisions should remain under authorized human control.

## 7. Evaluation Approach

The project can be evaluated using:

- Functional testing of milestone creation, submission, and review.
- Validation and duplicate-detection tests.
- Authorization tests using genuine access controls in a future production implementation.
- Usability feedback from permitted student and faculty-supervisor evaluations.
- Reliability testing for saving, retrieval, and recovery.
- Comparison of baseline and post-implementation workflow times during an approved pilot.

No real campus workflow improvements or time savings are claimed without measured evidence.

## 8. Conclusion

The Student Project Milestone Tracker demonstrates the practical application of web development, database design, software engineering, and testing concepts. Future integration with secure authentication, persistent storage, and reporting features could make it more suitable for real academic project management.

This project is a prototype and a learning exercise, not an officially adopted institutional system.

