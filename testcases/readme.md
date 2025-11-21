This repository contains Manual Test Cases, UI Automation, and API Automation for:
✔ Flow 0 — Sign In
Combining API + functional provides full coverage of the authentication flow, ensuring both frontend and backend work together correctly.

✔ Flow 1 — Equipment Inspection Form
Functional UI Testing gives full coverage with the least friction and ensure the form behaves correctly from a user's perspective.

✔ Flow 2 — Safety Hazard Report
Functional UI Testing gives full coverage with the least friction and ensure the form behaves correctly from a user's perspective.

Automation is implemented using Playwright (TypeScript) with support for:
✔ Web automation
✔ API automation
✔ Page Object Model (POM)
✔ Hooks, Steps, Models, and Utilities
✔ Allure Reporting

📁 Repository Structure
testcases/
├── manual/
│   ├── TC/
│   │     ├── TC_F0_SignIn-v1.0.xlsx
│   │     ├── TC_F1_EquipmentInspectionForm-v1.0.xlsx
│   │     └── TC_F2_SafetyHazardReport-v1.0.xlsx
│   ├── Evidence/
│   │     ├── TC_F0/
│   │     ├── TC_F1/
│   │     └── TC_F2/
│
├── automation/
│   ├── reports/
│   │     ├── allure-report/
│   │     ├── allure-results/
│   ├── tests/
│   │     ├── features/
│   │     ├── hooks/
│   │     ├── models/
│   │     ├── objectRepository/
│   │     ├── pages/
│   │     ├── steps/
│   │     ├── utils/


📝 Manual Test Cases

Manual test cases are stored in:
📂 manual/TC/
Each file contains structured test steps, expected results, and coverage for both positive and negative scenarios.

Evidence of execution (screenshots, videos, and logs) is placed under:
📂 manual/Evidence/<TC_GROUP_ID>/


🤖 Automation Overview (Playwright)

Automation uses Playwright (TypeScript) to handle:
✔ UI Testing (Web + Mobile Emulation)
✔ API Testing
✔ POM Structure
✔ BDD-Style Folder Organization
✔ Allure Reporting

Automation code is located in:
📂 automation/tests/


Below is an explanation of each component under automation/tests/.

📂 features/

Contains feature files describing system behavior in a Gherkin-like style.


📂 pages/ (Page Object Model)

Stores UI interaction logic and page abstractions.

Example files:

pages/
├── login.page.ts
├── equipment-inspection.page.ts
└── hazard-report.page.ts


📂 objectRepository/

Contains a centralized repository of selectors/locators, separate from POM logic.


📂 steps/

Contains step definition files that bind feature steps to actual automation code.


📂 models/

Contains TypeScript interfaces and data models for:
✔ API payloads
✔ UI form datasets

Example:

models/
├── login.model.ts
├── equipment.model.ts
└── hazard.model.ts

📂 hooks/

Contains global configuration:
✔ Test initialization
✔ Browser setup
✔ Authentication hooks
✔ Screenshot on failure
✔ Cleanup routines

📂 utils/

General-purpose utilities such as:
✔ API client wrapper
✔ File upload helpers
✔ Data generators
✔ Date formatter
✔ Randomizers


📊 Allure Reporting

Allure is integrated to generate rich, interactive test reports including:
✔ Step logs
✔ Screenshots
✔ API request/response attachments
✔ Error stack traces
✔ Scenario breakdown
✔ Summary dashboard

All reports are stored in:
automation/reports/


🏁 Summary

This repository provides:
✔ Full manual test coverage
✔ UI automation using Playwright + POM
✔ API automation with Playwright’s API client
✔ Clear BDD-style separation
✔ Centralized locators and utilities
✔ Allure reporting for detailed analysis
✔ Clean, scalable folder structure for long-term maintenance