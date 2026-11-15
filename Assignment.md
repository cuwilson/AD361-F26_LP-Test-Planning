## Part 1: Define the Context

| Section | Description |
| -- | -- |
| Test Objective | Users can view their bookings |
| Test Objective | Users can edit values already entered for a booking before submition |
| In scope | Booking form, booking value adjustments, and booking list |
| Out of scope | cancelation form |
| Test basis | Information required to make a booking, booking form code, appropriate user stories for creating a booking and viewing bookings |
| Assumption of constraint | Code coverage must be 94% |

## Part 2: Identify Roles and Responsibilities

| Role | Responsibilities | When Involved | Communication |
| -- | -- | -- | -- | 
| Tester | Designs and executes tests | Before and during test execution | Reports to the PM about results |
| Project Manager | review the effort estimates. schedules tester's time and budget accordingly. sync with developers with test results | Before, during, and after test execution | Everyone reports to them |
| Test Expert(s) | estimates the effort involved in testing | before tests are written | Reports directly to Project Manager | 

## Part 3: Define the Test Approach

| Test Area | Test Level or Type | Technique | Manual or Automated | Deliverable |
| -- | -- | -- | -- | -- |
| Booking form inputs | Component / Functional testing | Boundary value analysis | Automated | Jest test files and coverage report |
| Booking form validation | Component / Functional testing | Equivalence partitioning | Automated | Test cases and test results |
| Booking value adjustments | System / Functional testing | State transition testing | Manual | Test cases and test results |
| View bookings | System / Functional testing | Use case testing | Manual | Test cases and defect reports |
| Booking functionality after changes | Regression testing | Retesting existing test cases | Automated | Regression test results |

## Part 4: Identify Test Requirements

| Requirement | Value |
| -- | -- |
| Test environment | Test database with users and rentals, "dummy" payment methods |
| Browsers or devices | 3 browsers: Chrome, Firefox, Safari. 3 devices: Android phone, iPhone, Windows PC |
| Testing tools | Jest for automated testing, browser developer tools for manual testing, GitHub Issues for defect tracking |
| Test data | Test user accounts, sample rentals, valid and invalid booking dates, guest counts, and existing bookings |
| Access or permissions | Access to the test application, test database, source code, and GitHub repository |
| People or training | Tester familiar with booking requirements, test expert for estimating testing effort, developer for defect resolution, PM to oversee |


## Part 5: Create a Risk Register

| Risk | Type | Likelihood | Impact | Mitigation |
| -- | -- | -- | -- | -- |
| Users can create bookings with invalid dates or guest counts | Product | Medium | High | Prioritize boundary value and input validation testing |
| Booking changes are not saved or displayed correctly | Product | Medium | High | Test value adjustments and verify booking details after submission |
| Application behaves differently across browsers or devices | Product | Medium | Medium | Test on all selected browsers and devices |
| Testing takes longer than estimated | Project | Medium | Medium | Prioritize high-risk tests and monitor testing progress |


## Part 6: Define Entry Criteria

| Entry Criteria | Requirement |
| -- | -- |
| Test environment | Application and test database are accessible and functioning |
| Test cases | All planned test cases have been written and reviewed |
| Test data | Test users, rentals, and sample bookings have been created |
| Access | Testers have the required accounts and permissions |


## Part 7: Define Exit Criteria

| Exit Criteria | Requirement |
| -- | -- |
| Test execution | 100% of planned test cases have been executed |
| Code coverage | Automated tests achieve at least 94% code coverage |
| Critical defects | Zero unresolved critical or high-severity defects |
| Regression testing | All regression tests pass even after any defect fixes |

## Part 8: Create a Test Schedule

| Activity | Responsible Role | Time | Dependency |
| -- | -- | -- | -- |
| Review requirements and define test scope | Tester, Project Manager | Day 1 | Requirements are available |
| Estimate testing effort and finalize schedule | Test Expert, Project Manager | Day 1 | Test scope has been defined |
| Design test cases and prepare test environment | Tester | Day 2 | Test scope and schedule are finalized |
| Coordinate with developers to confirm application readiness | Project Manager | Day 2 | Testing requirements are identified |
| Execute tests and report defects | Tester | Days 3–4 | Test environment is ready and developers confirm application readiness |
| Run regression tests and review final results | Tester, Project Manager | Day 5 | Initial testing is complete and reported defects have been addressed |


## Part 9: Define the Communication Plan

| Information | Audience | Method | Frequency |
| -- | -- | -- | -- |
| Testing estimates | Project Manager | Initial meeting for requirements, then email | Before testing begins |
| Test progress and results | Project Manager | Daily status report | Daily during testing |
| Defects and required fixes | Developers | GitHub Issues and PM communication | When defects are identified |
| Developer updates and resolved defects | Tester | Project Manager updates | When fixes are available |
| Final test results and coverage report | Project Manager, Developers | Test completion report | At the end of testing |


