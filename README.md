# TITAN CMMS - Web Application Quality Assurance

## 📌 Project Overview
**TITAN CMMS** (titanmms.com) is a comprehensive Computerized Maintenance Management System. This repository hosts the complete Quality Assurance (QA) artifacts generated during the testing lifecycle of the web application. The project focuses on ensuring the stability of marketing funnels, form submissions, and UI responsiveness across various devices.

**Client:** Logic Unit
**QA Focus:** Functional Testing, UI/UX Validation, Form Logic, and Mobile Responsiveness.

## 📂 Repository Contents
This repository is organized into the following documentation modules:
* **Test Scenarios:** High-level testing scope (TS_001 to TS_033), prioritizing critical business flows like "Request Demo" and "Pricing".
* **Test Cases:** Detailed steps for modules including *Home, Features, Resources, Industries, Blog, and Contact Us*.
* **Execution Results:** Real-time logs of test execution (Pass/Fail status).
* **Bug Reports:** Documented defects with reproduction steps and severity analysis.

## 📊 Testing Statistics & Efficiency
The testing strategy utilized a module-based approach. Below is a breakdown of the testing efficiency and coverage derived from the execution logs:

| Metric | Details |
| :--- | :--- |
| **Total Test Scenarios** | 33+ High-level scenarios |
| **Modules Covered** | 10 (Home, Features, IoT, CMMS Software, Pricing, etc.) |
| **Critical Flows** | Request Demo, Contact Forms, Resource Navigation |
| **Defect Density** | Moderate (High concentration in UI/UX interactions) |
| **Test Environment** | Web Browsers (Chrome, Edge), Mobile Viewport (Android) |

### **Module Stability Assessment**
| Module | Status | Observations |
| :--- | :--- | :--- |
| **Contact Forms** | 🟢 **Stable** | "Request Demo" and "Contact Us" forms submit correctly with valid data. |
| **Navigation** | 🟠 **Risk** | Several internal links (Resources/Industries) redirect incorrectly. |
| **UI/UX** | 🔴 **Unstable** | Consistent "Hover" state issues across multiple pages. |
| **Pricing** | 🟡 **Mixed** | Form functionality works, but input validation is weak. |

## 🐞 Defect Analysis & Bug Tracking
A detailed analysis of the `TITAN BugReport.xlsx` and Execution logs highlights specific areas for improvement.

### **1. The "Vanishing Text" UI Bug (High Frequency)**
**Severity:** Medium (UI/UX)
**Observation:** Across almost all pages (Home, Features, IoT, CMMS Software), hovering over the "Request Demo" button causes the text to disappear or the button to behave inconsistently.
* *Affected Test Cases:* `TC_HM_001`, `TC_FE_001`, `TC_RS_001`, `TC_IN_001`, `TC_IOT_001`.

### **2. Input Validation Failure**
**Severity:** High (Data Integrity)
**Observation:** The **Pricing Page** form accepts invalid data types.
* *Defect:* Entering numeric values (e.g., "981") into the "First Name" and "Last Name" fields does not trigger an error; the form is submitted successfully.
* *Reference:* `TC_PR_002`

### **3. Mobile Responsiveness**
**Severity:** Medium
**Observation:** The website footer does not render correctly on mobile devices (Android), breaking the layout compared to the desktop version.
* *Reference:* `TC_HM_030`

### **4. Navigation Logic Errors**
**Severity:** Low
**Observation:** "Read More" buttons in the *Industries* and *Resources* sections often redirect to the Home page or "Request Demo" page instead of the specific relevant blog post or article.

## 🛠 Tools & Methodologies
* **Manual Testing:** Exploratory and Scripted testing.
* **Cross-Browser Testing:** Verified on Chrome and Edge.
* **Spreadsheet Management:** Test cases and bugs tracked via structured Excel logs.

## 📝 Author
**Meesum**
*QA Engineer*

---
*This repository serves as a professional portfolio demonstrating proficiency in Black Box Testing, Defect Lifecycle Management, and Test Documentation.*
