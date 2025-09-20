# ERM for Hybrid Workforce 💼

![License: MIT](https://img.shields.io/badge/License-MIT-blue)
![Built with Salesforce DX](https://img.io/badge/Built%20with-Salesforce%20DX-orange)
![Status: In Development](https://img.shields.io/badge/Status-In%20Development-brightgreen)
![Program: TCS SmartBridge](https://img.shields.io/badge/Program-TCS%20SmartBridge-purple)

A Salesforce-powered ecosystem designed to **digitize employee engagement, streamline hybrid work management, and improve workforce productivity and retention**. This platform connects employees, managers, HR, and leadership to create a more efficient, data-driven, and employee-centric workplace.

## 📑 Table of Contents
- [Problem Statement](#-problem-statement)
- [Our Solution](#-our-solution)
- [Key Features (Phase 1)](#-key-features-phase-1)
- [Technology Stack](#-technology-stack)
- [Getting Started](#-getting-started)
- [Repository Structure](#-repository-structure)
- [Project Context](#-project-context)

---

## ❗ Problem Statement

Companies with hybrid workforces face challenges in maintaining engagement, ensuring well-being, and monitoring productivity. Employees working remotely or on flexible schedules often feel disconnected, while managers struggle to track team performance, work schedules, and engagement. Disparate systems for surveys, scheduling, and HR management lead to inefficiencies, low morale, and increased attrition risk.

---

## 💡 Our Solution

**ERM for Hybrid Workforce** is a Salesforce-based platform that provides a **central hub for all employee interactions**. It's designed to create a unified ecosystem for all stakeholders in a hybrid work environment.

- **For Employees:** Access a mobile-friendly portal to manage schedules, provide real-time feedback, and access company resources.
- **For Managers:** Monitor team engagement, view schedules, track sentiment trends, and respond to feedback proactively.
- **For HR & Leadership:** Analyze organization-wide engagement trends, optimize hybrid scheduling, and make data-driven workforce decisions.

---

## ✨ Key Features (Phase 1)

- 🗓 **Hybrid Scheduling Module:** A dedicated component allowing employees to log office and remote days, providing managers with a consolidated view of their team's schedule.
- 📊 **Analytics & Dashboards:** Real-time reporting on engagement, attrition risks, and productivity trends using Tableau CRM.
- 📝 **Real-Time Feedback Collection:** A streamlined process for gathering employee feedback through pulse surveys, with AI-driven sentiment analysis to identify and address issues.
- 🔔 **Automated Alerts & Notifications:** Salesforce Flow and triggers to send automated reminders for surveys, one-on-one meetings, and HR follow-ups.
- 📚 **Knowledge Base:** A centralized repository for company policies, onboarding materials, and frequently asked questions, built on Salesforce Experience Cloud.
- 🤖 **Intelligent Automation:** Behind-the-scenes flows and triggers that automate feedback analysis, notifications, and escalation processes.

---

## 🛠 Technology Stack

- **Core Platform:** Salesforce Lightning Platform
- **UI:** Lightning Web Components (LWC) & Experience Cloud
- **Backend Logic:** Apex (Controllers, Triggers, Schedulable, Queueable)
- **Automation:** Salesforce Flow & Approval Processes
- **Analytics:** Tableau CRM (Einstein Analytics)
- **DevOps:** Salesforce DX, Visual Studio Code, Git & GitHub
- **AI/ML:** Einstein AI for sentiment analysis of employee feedback

---

## ⚡ Getting Started

Follow these steps to get a copy of the project up and running in your Salesforce environment.

### Prerequisites

- Salesforce CLI
- Visual Studio Code with the Salesforce Extension Pack
- A Salesforce Developer Edition Org or Sandbox

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/erm-hybrid-workforce.git](https://github.com/your-username/erm-hybrid-workforce.git)
    cd erm-hybrid-workforce
    ```
2.  **Authorize your Salesforce Org:**
    ```bash
    sfdx auth:web:login --setalias my-dev-org --instanceurl [https://login.salesforce.com](https://login.salesforce.com)
    ```
3.  **Deploy the source code to your org:**
    ```bash
    sfdx force:source:deploy --targetusername my-dev-org --sourcepath force-app
    ```
4.  **Assign Permission Sets:**
    ```bash
    # Assign the 'Employee' permission set
    sfdx force:user:permset:assign --targetusername my-dev-org --permsetname Employee
    
    # Assign the 'Manager' permission set
    sfdx force:user:permset:assign --targetusername my-dev-org --permsetname Manager
    ```
    *(Note: Permission set names are examples and should be adjusted based on your project's final configuration.)*

---

## 📂 Repository Structure
