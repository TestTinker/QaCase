
# **WeMine – Manual Test Cases, UI Automation & API Automation**

This repository contains **Manual Test Cases**, **UI Automation**, and **API Automation** for the WeMine application.

✔ Flow 0 — **Sign In**  
Combines **API + functional testing** to ensure authentication works correctly across backend and frontend.

✔ Flow 1 — **Equipment Inspection Form**  
Functional UI testing ensures dynamic fields behave correctly and validations work properly.

✔ Flow 2 — **Safety Hazard Report**  
Functional UI testing ensures the entire hazard reporting workflow performs as expected.

Automation uses **Playwright (TypeScript)** and includes:  
✔ Web automation  
✔ API automation  
✔ Page Object Model (POM)  
✔ Hooks, Steps, Models, Utilities  
✔ Allure Reporting

---

## **📁 Repository Structure**

```
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
│   │
│   ├── tests/
│   │     ├── features/
│   │     ├── hooks/
│   │     ├── models/
│   │     ├── objectRepository/
│   │     ├── pages/
│   │     ├── steps/
│   │     ├── utils/
```

---

## **📝 Manual Test Cases**

Manual test cases are located in:

📂 `manual/TC/`

Each file covers full positive and negative test scenarios with structured steps and validations.

Execution evidence (screenshots, logs, recordings) is stored in:

📂 `manual/Evidence/<TC_GROUP_ID>/`

---

## **🤖 Automation Overview (Playwright)**

This project uses **Playwright (TypeScript)** for:

✔ UI Testing (Web + Mobile viewport simulation)  
✔ API Testing  
✔ Page Object Model (POM)  
✔ BDD-style folder organization  
✔ Allure reporting

Automation code is located in:

📂 `automation/tests/`

---

## **📂 features/**

Contains feature-style scenario descriptions defining system behavior.

---

## **📂 pages/**  
**(Page Object Model)**

Stores UI interaction logic.

Example files:

```
pages/
├── login.page.ts
├── equipment-inspection.page.ts
└── hazard-report.page.ts
```

---

## **📂 objectRepository/**

Central storage for selectors and locators used by Page Objects.

---

## **📂 steps/**

Houses step definitions linking feature scenarios to Playwright automation logic.

---

## **📂 models/**

Contains TypeScript interfaces and data models:

✔ API payload schemas  
✔ UI form data structures  

Example:

```
models/
├── login.model.ts
├── equipment.model.ts
└── hazard.model.ts
```

---

## **📂 hooks/**

Includes base test configuration:

✔ Setup  
✔ Teardown  
✔ Browser lifecycle  
✔ Screenshot on failure  
✔ Context initialization  

---

## **📂 utils/**

Utility helpers:

✔ API client wrapper  
✔ File operations  
✔ Data/time formatters  
✔ Random value generators  

---

## **📊 Allure Reporting**

Allure is used to generate rich test reports containing:

✔ Logs  
✔ Screenshots  
✔ API requests/responses  
✔ Step tracing  
✔ Error stack traces  
✔ Dashboard summary  

Reports are stored in:

📂 `automation/reports/`

---

## **🏁 Summary**

This repository provides:

✔ Full manual test coverage  
✔ Web UI automation using Playwright + POM  
✔ API automation with Playwright API client  
✔ Clear BDD-style test organization  
✔ Reusable models, utilities, and hooks  
✔ Integrated Allure reporting  
✔ Clean, scalable folder structure  
