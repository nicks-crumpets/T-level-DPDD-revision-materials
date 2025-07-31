# Gantt charts

Has:

- Individual tasks
- Duration of tasks
- Duration of projects
- Start and end dates

1. Understand the task and requirements

Read task brief carefully

- Understand the goals of the project
- Identify the key deliverables

**Review provided info**

- Study the team profiles, task list and financial information

1. Break down the tasks 

**List all tasks**

- Use the provided task list

1. Create a Gantt chart

Map all of the tasks to the timeline, making sure that you don’t go over the teams capacity for the week

1. Develop the resource and cost plan

**Assign tasks to team members**

- Match the tasks to team members based on their skills

—

---

# Solving an example question

## Understanding the constraints

**Total available hours** → ****595 hours (35 hours/week × 17 weeks)

**Team Capacity →** 175 hours/week (5 team members × 35 hours/week)

**Task List →** Provided in the task brief

**Assumptions**:

- 3 minor faults per module (18 minor faults total)
- No more than 3 major faults in total

**Total Project Hours**: 1,193 hours.

**Available Hours**: 595 hours/week (35 hours/week x 17 weeks)

![image.png](Gantt%20charts%20184530129127805da947d882e3df1d39/image.png)

## Working out dependencies

Determine which tasks must be completed before others can start.
For example:

- Infrastructure upgrade must be completed before server installation.
- Module development must be completed before testing.
- Testing must be completed before deployment.
- Deployment must be completed before user training.

| **Task** | **Dependency** |
| --- | --- |
| Upgrade Infrastructure | None |
| Install Physical Server | Upgrade Infrastructure |
| Develop Module 1 | None |
| Develop Module 2 | None |
| Develop Module 3 | None |
| Develop Module 4 | None |
| Develop Module 5 | None |
| Develop Module 6 | None |
| Create a Test Plan | None |
| Unit Testing | Module Development Completed |
| Integration Testing | Unit Testing Completed |
| Fixing and Regression Testing | Integration Testing Completed |
| User/Acceptance Testing | Fixing and Regression testing Completed |
| Deploy Modules | All modules Developed, Tested and fixed |
| User Training | Deployment Completed |

## Assigning tasks to team members

![image.png](Gantt%20charts%20184530129127805da947d882e3df1d39/image%201.png)

## Weekly structure

| **Week** | **Task** | **Assigned to** | **Hours** |
| --- | --- | --- | --- |
| 1 | Upgrade Infrastructure | Marius Bronski | 21 |
|  | Create a test plan | Sarah O’Toole | 14 |
| 2 | Install Physical Server | Marius Bronski | 7 |
|  | Develop Module 1 – Back-End | Gina Diaz | 35 |
|  | Develop Module 2 – User Interface | Ahad Shafiq | 35 |
|  | Develop Module 3 – Information Feed | Terry Duran | 35 |
|  | Develop Module 4 – Investments | Sarah O’Toole | 35 |
| 3 | Develop Module 1 – Back-End | Gina Diaz | 35 |
|  | Develop Module 2 – User Interface | Ahad Shafiq | 35 |
|  | Develop Module 3 – Information Feed | Terry Duran | 35 |
|  | Develop Module 4 – Investments | Sarah O’Toole | 35 |

*Module 1 = 5 weeks (finish wk 6)
Module 2 = 2 weeks (finish wk 3)
Module 3 = 4 weeks (finish wk 5)
Module 4 = 4 weeks (finish wk 5)
Module 5 = 4 weeks (start wk 5 – finish wk 8)
Module 6 = 3 weeks (start wk 5 – finish wk 8)*

| **Week** | **Task** | **Assigned to** | **Hours** |
| --- | --- | --- | --- |
| 4 | Develop Module 1 – Back-End | Gina Diaz | 35 |
|  | Develop Module 3 – Information Feed | Terry Duran | 35 |
|  | Develop Module 4 – Investments | Sarah O’Toole | 35 |
|  | Deploy Module 2 | Marius Bronski | 7 |
|  | Unit Test Module 2 | Ahad Shafiq | 21 |
| 5 | Develop Module 1 – Back-End | Gina Diaz | 35 |
|  | Develop Module 3 – Information Feed | Terry Duran | 21 |
|  | Develop Module 6 - Communications | Terry Duran | 14 |
|  | Develop Module 4 – Investments | Sarah O’Toole | 7 |
|  | Develop Module 5 – Data Analytics | Sarah O’Toole | 28 |
| 6 | Develop Module 5 – Data Analytics | Sarah O’Toole | 35 |
|  | Develop Module 1 – Back End | Gina Diaz | 7 |
|  | Develop Module 6 – Communications | Terry Duran | 35 |
|  | Deploy Modules 1, 3, 4 | Marius Bronski | 21 |
|  | Unit Test Module 1, 3 | Ahad Shafiq | 21, 14 |

*Module 1 = 5 weeks (finish wk 6)
Module 2 = 2 weeks (finish wk 3)
Module 3 = 4 weeks (finish wk 5)
Module 4 = 4 weeks (finish wk 5)
Module 5 = 4 weeks (start wk 5 – finish wk 8)
Module 6 = 3 weeks (start wk 5 – finish wk 8)*

| **Week** | **Task** | **Assigned to** | **Hours** |
| --- | --- | --- | --- |
| 7 | Unit Test 3 | Ahad Shafiq | 7 |
|  | Integration Testing 1, 2 | Ahad Shafiq | 14, 14 |
|  | Develop Module 5 – Data Analytics | Sarah O’Toole | 35 |
|  | Develop Module 6 – Communications | Terry Duran | 35 |
| 8 | Develop Module 5 – Data Analytics | Sarah O’Toole | 14 |
|  | Develop Module 6 – Communications | Terry Duran | 21 |
|  | Deploy Modules 5, 6 | Marius Bronski | 14 |
|  | Unit Test 4 | Terry Duran | 14 |
|  | Integration Testing 3, 4 | Ahad Shafiq | 14, 14 |
|  | Unit Test 5 | Ahad Shafiq | 7 |

*Module 1 = 5 weeks (finish wk 6)
Module 2 = 2 weeks (finish wk 3)
Module 3 = 4 weeks (finish wk 5)
Module 4 = 4 weeks (finish wk 5)
Module 5 = 4 weeks (start wk 5 – finish wk 8)
Module 6 = 3 weeks (start wk 5 – finish wk 8)*

---