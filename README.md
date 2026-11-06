<div align="center">
  <img src="assets/inti-university-seeklogo.png" alt="INTI International University Logo" width="380"/>
  <br><br>

  # 🛡️ Enterprise Software Quality Assurance (SQA) & Configuration Management Framework
  ### *Theoretical & Empirical Analysis of ISO/IEC 9126, McCall’s Quality Models, IEEE 610.12 Defect Taxonomy, and SCM Lifecycle Governance on Meta Platforms (Facebook) & DigitalConnect Solutions*

  ![Scholarship](https://img.shields.io/badge/Scholarship-Fully_Funded_Student_Mobility_Program_(June_2026)-B31B1B?style=for-the-badge)
  ![Host Institution](https://img.shields.io/badge/Host_University-INTI_International_University_(Nilai,_Malaysia)-003366?style=for-the-badge)
  <br>
  ![SQA Models](https://img.shields.io/badge/SQA_Frameworks-ISO_9126_%7C_McCall's_%7C_IEEE_610.12-0A66C2?style=for-the-badge&logo=checkmarx&logoColor=white)
  ![Case Study](https://img.shields.io/badge/Case_Study-Meta_Platforms_(Facebook)-0866FF?style=for-the-badge&logo=meta&logoColor=white)
  ![SCM](https://img.shields.io/badge/SCM-Change_%7C_Version_%7C_Build_%7C_Release-6C5CE7?style=for-the-badge&logo=git&logoColor=white)
  ![Figma](https://img.shields.io/badge/UI_Prototyping-Figma_8--Module_Architecture-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
  ![Status](https://img.shields.io/badge/Project_Status-Completed-success?style=for-the-badge)

  **Course / Module:** SDT4202 – Software Quality (Section 6MB1 / Group 2)  
  **Programme:** Bachelor of Computer Science (BCSI) | **Coursework Weight:** 30% (LO2)  
  **Session:** June 2026 | **Institution:** INTI International University, Nilai, Malaysia  
  **Lecturer / Examiner:** Noor Zuhaili Md Yasin (`noorzuhaili.mdyasin@newinti.edu.my`)  
  **Domain:** Software Quality Assurance (SQA), Software Configuration Management (SCM) & Enterprise System Architecture

</div>

---

## 📖 Table of Contents

- [📌 Project Overview](#-project-overview)
- [🎯 Problem Statement, Business Context & Quality Philosophies](#-problem-statement-business-context--quality-philosophies)
- [📐 Theoretical SQA Models & Defect Frameworks](#-theoretical-sqa-models--defect-frameworks)
- [🔍 Empirical Case Study: 4 Major Meta (Facebook) SQA Failures (2018–2024)](#-empirical-case-study-4-major-meta-facebook-sqa-failures-20182024)
- [🛠️ Tech Stack, Tools & Methodologies](#️-tech-stack-tools--methodologies)
- [🏗️ System Architecture & SCM Governance Pipelines](#️-system-architecture--scm-governance-pipelines)
- [✨ Core SCM Pillars & Proposed Lifecycle Models](#-core-scm-pillars--proposed-lifecycle-models)
- [📸 Visual Walkthrough & 8-Module System Build Prototype](#-visual-walkthrough--8-module-system-build-prototype)
- [🧱 Deep-Dive Technical Governance & CCB Artifacts](#-deep-dive-technical-governance--ccb-artifacts)
- [📂 Repository File Structure](#-repository-file-structure)
- [🚀 Viewing & Reproduction Guide](#-viewing--reproduction-guide)
- [👥 Project Team & Author Details](#-project-team--author-details)

---

## 📌 Project Overview

Completed during the **June 2026 Session** at **INTI International University, Nilai, Malaysia** under a **Fully Funded International Student Mobility Scholarship Program**, this project delivers a comprehensive theoretical and applied investigation into **Software Quality Assurance (SQA)** and **Software Configuration Management (SCM)** for hyperscale cloud platforms. Conducted for **SDT4202 – Software Quality** under the supervision of **Lecturer Noor Zuhaili Md Yasin**, the study evaluates the operational, financial, and workforce consequences of planned and unplanned software changes (**Learning Outcome LO2**).

The research centers on **Meta Platforms, Inc. (Facebook)**—one of the world's largest distributed cloud ecosystems serving **3+ billion Daily Active Users (DAU)** and **~2.9 billion Monthly Active Users (MAU)**—alongside an enterprise release recovery framework for **DigitalConnect Solutions**. The study bridges classical software engineering quality theory with real-world incident post-mortems by evaluating four publicly documented software quality failures at Meta between **2018 and 2024**:
1. **Cambridge Analytica Graph API Data Privacy Breach (2018)** — Affecting **87 million users** and resulting in a **$5 billion FTC penalty** plus a **$725 million class-action settlement**.
2. **Contact Importer Mass Scraping Vulnerability (2019–2021)** — Exposing **533 million user profiles across 106 countries** and triggering a **€265 million (~$276 million) GDPR fine**.
3. **Global BGP Backbone Configuration Outage (October 2021)** — Causing a **6-hour worldwide blackout** across Facebook, Instagram, WhatsApp, Messenger, and Oculus for **3.5 billion users**, costing **~$60 million in direct ad revenue** and a **5% market capitalization drop**.
4. **Password Reset Brute-Force Account Takeover Flaw (2024)** — A critical authentication defect lacking rate-limiting on 6-digit recovery codes, remediated via formal Change Control Board (CCB) governance (`META-FB-2024-SEC-001`).

To translate theoretical SQA models into actionable engineering practice, the project formulates end-to-end **7-Stage Change Management**, **7-Stage Version Management**, and **10-Stage Controlled Release Management** models, complemented by a **3-Tier Modular Facebook Clone Architecture** and an **8-screen high-fidelity Figma UI prototype** engineered to satisfy **McCall's** and **ISO/IEC 9126** quality attributes.

---

## 🎯 Problem Statement, Business Context & Quality Philosophies

### 🌐 The Hyperscale Software Quality Challenge
In distributed cloud architectures operating across millions of servers across North America, Europe, and Asia, thousands of code commits and network configuration updates are deployed daily. A single unvalidated change, unversioned router script, or missing API rate-limit cascades via a **domino effect** across interconnected microservices—resulting in global service blackouts, mass privacy breaches, multi-billion-dollar regulatory sanctions, and severe reputational erosion.

### 🏛️ Foundational Software Quality Philosophies
This study evaluates Meta's engineering failures and proposed remediations through two foundational quality paradigms:

| Quality Paradigm | Theorist | Core Theoretical Definition | Application to Meta Platforms (Facebook) |
| :--- | :---: | :--- | :--- |
| **Conformance to Requirements** | **Philip B. Crosby (1979)** | Quality is defined strictly as adherence to explicitly documented functional, security, and performance specifications. Any deviation from specification constitutes a **software defect**. | Evaluates whether Graph API permissions, Contact Importer rate limits, BGP router configurations, and 2FA password reset endpoints strictly conform to internal security specifications and GDPR/FTC privacy mandates. |
| **Fitness for Use** | **Joseph M. Juran (1970)** | Quality is measured by the degree to which a software system fulfills real-world user needs, maintains high availability, and delivers reliable user satisfaction under production workloads. | Assesses whether ~3 billion daily users, businesses, and advertisers can continuously communicate, transact via Facebook Pay, and interact safely without service blackouts or account takeovers. |

---

## 📐 Theoretical SQA Models & Defect Frameworks

A central contribution of this project is the rigorous application of four classical Software Quality Assurance models to diagnose root causes and architect preventative engineering controls.

### 1️⃣ IEEE Standard 610.12 Defect Causal Chain
Rather than treating "bugs" monolithically, this study classifies every software failure across the formal three-stage **IEEE Std 610.12** causal progression:

```text
+---------------------------------------------------------------------------------------------------+
|                           IEEE STD 610.12 DEFECT CAUSAL TAXONOMY                                  |
+---------------------------------------------------------------------------------------------------+
|                                                                                                   |
|  [ 1. SOFTWARE ERROR ]           [ 2. SOFTWARE FAULT ]            [ 3. SOFTWARE FAILURE ]         |
|  Human mistake made by an   -->  Static defect manifested    -->  Dynamic, externally observable  |
|  architect, developer, or        inside the source code,          deviation of system behavior    |
|  network engineer during         API logic, or router             from user expectations or       |
|  design/configuration.           configuration file.              system specifications.          |
|                                                                                                   |
|  * Example (2024 ATO):           * Example (2024 ATO):            * Example (2024 ATO):           |
|    Developer omits rate-           Password Reset Module v4.3       Attackers brute-force         |
|    limiting logic in auth          accepts unlimited 6-digit        6-digit tokens and hijack     |
|    specification design.           code attempts for 2 hours.       arbitrary user accounts.      |
+---------------------------------------------------------------------------------------------------+
```

### 2️⃣ ISO/IEC 9126 Software Quality Model
The **ISO/IEC 9126** standard evaluates software quality across **6 primary characteristics** and their sub-characteristics. Within this project, every historical incident and UI/UX prototype module is audited against these six pillars:

| ISO/IEC 9126 Characteristic | Key Sub-Characteristics Evaluated | Theoretical Definition & Role in SQA |
| :--- | :--- | :--- |
| **1. Functionality** | *Suitability, Accuracy, Interoperability, Security* | Capability of the software to provide functions that meet stated and implied needs while preventing unauthorized access to data (**Security**). |
| **2. Reliability** | *Maturity, Fault Tolerance, Recoverability* | Capability of the software to maintain a specified level of performance under stated conditions (**Fault Tolerance**) and re-establish service rapidly after a crash (**Recoverability**). |
| **3. Usability** | *Understandability, Learnability, Operability* | Effort required for diverse global users to recognize the logical concept, learn navigation flows, and operate interfaces with minimal cognitive load. |
| **4. Efficiency** | *Time Behavior, Resource Utilization* | Relationship between system response/processing times (**Time Behavior**), throughput rates, and cloud computing resources consumed under peak load. |
| **5. Maintainability** | *Analyzability, Changeability, Stability, Testability* | Effort required to diagnose root causes of failures (**Analyzability**), implement code/config modifications (**Changeability**), and validate changes without side effects. |
| **6. Portability** | *Adaptability, Installability, Co-existence* | Ability of the software to be transferred and rendered consistently across heterogeneous desktop browsers, mobile OS environments, and cloud data centers. |

### 3️⃣ McCall’s Quality Factor Model (1977)
**McCall’s Model** organizes **11 software quality factors** into three lifecycle perspectives, bridging user-facing operational behavior with internal engineering maintainability:

* **Product Operation (Using the Software):**
  * **Correctness:** Extent to which a program satisfies its specifications and fulfills user objectives (e.g., accurate profile rendering and strict input validation).
  * **Reliability:** Extent to which a system performs its intended functions with required precision without failing under normal or adverse conditions.
  * **Efficiency:** Amount of computing resources and code required by a program to perform its function.
  * **Integrity:** Extent to which access to software or data by unauthorized persons can be controlled (critical in mitigating API harvesting, scraping, and brute-force attacks).
  * **Usability:** Effort required to learn, operate, prepare input for, and interpret output of a program.
* **Product Revision (Changing the Software):**
  * **Maintainability:** Effort required to locate and fix an error in an operational program (severely compromised during the October 2021 BGP outage when internal diagnostic tools went offline).
  * **Flexibility:** Effort required to modify an operational program for adaptive or perfective enhancements.
  * **Testability:** Effort required to test a program to ensure that it performs its intended function (highlighted in the 2024 password reset flaw discovered externally via Bug Bounty rather than internal QA).
* **Product Transition (Adapting the Software to New Environments):**
  * **Portability:** Effort required to transfer the software from one hardware or operating system environment to another.
  * **Reusability:** Extent to which modular software components can be reused in other applications.
  * **Interoperability:** Effort required to couple one system with another (e.g., third-party integrations via Facebook Graph API).

### 4️⃣ Galin’s 9 Causes of Software Defects
Following **Daniel Galin’s SQA taxonomy**, software defects originate from nine distinct lifecycle breakdowns, which this report maps directly to Meta’s operational failures:
1. **Faulty requirements definition** (erroneous, incomplete, or ambiguous security requirements).
2. **Client-developer communication failures**.
3. **Deliberate deviations from software requirements** (shortcuts taken during maintenance or configuration).
4. **Logical design errors** (flawed algorithmic or architectural modeling).
5. **Coding errors** (implementation bugs in source code or router configuration syntax).
6. **Non-compliance with documentation and coding instructions** (bypassing internal privacy/security guidelines).
7. **Shortcomings of the testing process** (omitting automated abuse, regression, or penetration testing).
8. **Procedure errors** (flawed operational deployment or recovery workflows).
9. **Documentation errors** (outdated or inaccurate configuration/version records).

---

## 🔍 Empirical Case Study: 4 Major Meta (Facebook) SQA Failures (2018–2024)

The table below synthesizes the multi-framework theoretical diagnosis across all four documented Meta incidents analyzed in this study:

| # | Incident & Timeline | Root Cause & SCM Breakdown | IEEE 610.12 Defect Chain | ISO 9126 Factors Violated | McCall’s Factors Violated | Galin Defect Causes | Financial & Business Impact | Meta’s Engineering Remediation |
| :-: | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **Cambridge Analytica Data Breach**<br>*(2018)* | Unreviewed **Graph API** change allowed 3rd-party quiz apps to harvest data of installing users **and all their friends** (~87M users) without consent. | • **Error:** Logical design omission in consent boundary.<br>• **Fault:** Over-permissive API endpoint.<br>• **Failure:** Mass unauthorized data harvesting. | • **Functionality** *(Security)* | • **Integrity**<br>• **Correctness** | • Cause 1 *(Faulty requirements)*<br>• Cause 6 *(Non-compliance with privacy rules)* | • **$5.0 Billion** FTC fine (2019)<br>• **$725 Million** user settlement (2022)<br>• US Congressional hearings | • Restricted Graph API friend data access<br>• Mandatory **App Review** gate<br>• Launched **Data Abuse Bounty**<br>• Expanded security staff by **15,000+** |
| **2** | **533M User Data Scraping Vulnerability**<br>*(2019–2021)* | **Contact Importer** feature updated without rate-limiting or bot-abuse testing, allowing attackers to enumerate **533M profiles** across 106 countries via phone lists. | • **Error:** Flawed lookup design.<br>• **Fault:** Missing rate-limiting in Contact Importer.<br>• **Failure:** Automated mass profile scraping. | • **Functionality** *(Security)*<br>• **Reliability** *(Fault Tolerance)* | • **Integrity**<br>• **Reliability** | • Cause 1 *(Faulty security requirements)*<br>• Cause 7 *(Testing shortcomings)* | • **€265 Million** (~$276M) Irish DPC GDPR fine (Nov 2022)<br>• EU-wide regulatory investigations | • Patched Contact Importer with strict **Rate Limiting** (Aug 2019)<br>• Deployed automated bot/scraping detection<br>• Added abuse scenarios to QA pipelines |
| **3** | **Global Platform BGP Routing Outage**<br>*(Oct 4, 2021)* | Routine maintenance command on backbone routers withdrew all **BGP routes** globally; internal recovery tools shared the same production network, locking engineers out. | • **Error:** Human mistake in router command.<br>• **Fault:** Invalid BGP withdrawal config.<br>• **Failure:** 6-hour total global blackout (3.5B users). | • **Reliability** *(Recoverability)*<br>• **Efficiency** *(Time Behavior)*<br>• **Maintainability** *(Analyzability)* | • **Reliability**<br>• **Maintainability** | • Cause 3 *(Deliberate deviation)*<br>• Cause 5 *(Coding/config error)*<br>• Cause 7 *(Testing shortcuts)* | • **~$60 Million** lost ad revenue in 6 hrs<br>• **~5% stock drop** (billions in market cap)<br>• Physical datacenter break-in required | • Multi-level approval for network configs<br>• Isolated **out-of-band recovery network**<br>• Adopted **Conveyor** safe CI/CD tool<br>• Automated config rollback |
| **4** | **Password Reset Account Takeover (ATO)**<br>*(Early 2024)* | Password reset endpoint issued a **6-digit code** valid for **2 hours** without brute-force rate limiting, enabling full account takeover. | • **Error:** Omitted lockout threshold in auth design.<br>• **Fault:** Missing rate-limit in Password Reset v4.3.<br>• **Failure:** Unauthorized account compromise. | • **Functionality** *(Security)*<br>• **Reliability** *(Fault Tolerance)* | • **Integrity**<br>• **Testability** | • Cause 5 *(Coding error)*<br>• Cause 7 *(Shortcomings in security testing)* | • High-severity Bug Bounty payout<br>• Emergency security patch (`META-FB-2024-SEC-001`, $13k cost, 72 effort hrs) | • Enforced strict attempt rate-limiting & token expiration<br>• Mandatory penetration & regression testing prior to auth releases |

---

## 🛠️ Tech Stack, Tools & Methodologies

| Category | Technology / Framework | Purpose & Application in Project |
| :--- | :--- | :--- |
| **Quality Assurance Models** | **ISO/IEC 9126 & McCall’s Model (1977)** | Multi-dimensional evaluation of software quality across Product Operation, Product Revision, and Product Transition factors. |
| **Defect Classification** | **IEEE Std 610.12 & Galin’s 9 Causes** | Formal root-cause decomposition separating human Software Errors, code/config Software Faults, and external Software Failures. |
| **Quality Philosophies** | **Crosby (1979) & Juran (1970)** | Theoretical grounding in *Conformance to Requirements* (defect prevention) and *Fitness for Use* (user-centric reliability). |
| **Change Governance** | **CCB Change Request (`META-FB-2024-SEC-001`)** | 3-stage enterprise Change Control Board artifact covering impact analysis, WBS scheduling, effort hours, and budget allocation. |
| **Version Control & CI/CD** | **Git, GitHub, GitLab & Meta Conveyor** | Distributed/centralized repository management, 5-branch isolation strategy, semantic versioning, and staged continuous deployment. |
| **System Architecture** | **3-Tier Modular Client-Server Architecture** | Separation of Frontend UI Layer, Backend Application Layer (5 microservices/modules), and Database Layer (4 persistent stores). |
| **UI/UX Prototyping** | **Figma Interactive Design Suite** | High-fidelity 8-screen web prototype of the Facebook Clone designed to validate Usability, Integrity, Correctness, and Efficiency early. |
| **Documentation & Modeling** | **Microsoft Office, MATLAB & Architecture Diagrams** | Technical report compilation, workflow diagramming, and Turnitin originality verification (**3% Similarity Index**). |

---

## 🏗️ System Architecture & SCM Governance Pipelines

### 1️⃣ 3-Tier Modular System Architecture (Facebook Clone Build)
To demonstrate how software quality attributes (*Maintainability, Scalability, Integrity, Reliability*) are embedded directly into system design, the project models a modular **3-Tier Client-Server Architecture** dividing presentation interfaces, application logic, and persistent data stores:

<div align="center">
  <img src="assets/System%20Architecture%20Diagram.png" alt="System Architecture Diagram - Facebook Clone 3-Tier Modular Architecture" width="720"/>
  <p><i>Figure 1: Three-Tier Modular Client-Server Architecture for the Proposed Facebook Clone System (Frontend UI Layer, Backend Application Layer, and Database Layer).</i></p>
</div>

```text
+===================================================================================================+
|                                  FRONTEND (PRESENTATION / UI LAYER)                               |
|                                                                                                   |
|  +----------------+  +-------------+  +-------------+  +-------------+  +--------------+  +----+  |
|  | Login & Reg.   |  | Home Feed   |  | User Profile|  | Messaging   |  | Notification |  |Set-|  |
|  | Interface      |  | Interface   |  | Interface   |  | Interface   |  | Interface    |  |ting|  |
|  +----------------+  +-------------+  +-------------+  +-------------+  +--------------+  +----+  |
+=================================================|=================================================+
                                                  | HTTPS / REST & Real-Time WebSockets
                                                  v
+===================================================================================================+
|                                 BACKEND (APPLICATION LOGIC LAYER)                                 |
|                                                                                                   |
|  +-------------------+  +-------------------+  +-------------------+  +------------+  +--------+  |
|  | Authentication    |  | User Management   |  | Post Management   |  | Messaging  |  | Notif. |  |
|  | Module            |  | Module            |  | Module            |  | Module     |  | Module |  |
|  | (Rate-Limit/Auth) |  | (Profiles/Friends)|  | (Feed/Comments)   |  | (Sync/Chat)|  | (Alerts|  |
|  +-------------------+  +-------------------+  +-------------------+  +------------+  +--------+  |
+=================================================|=================================================+
                                                  | Encrypted Queries / ACID Transactions
                                                  v
+===================================================================================================+
|                                    DATABASE (PERSISTENCE LAYER)                                   |
|                                                                                                   |
|     +----------------------+   +----------------------+   +------------------+   +------------+   |
|     |      User Data       |   |      Posts Data      |   |  Messages Data   |   |   Friend   |   |
|     | (Credentials/Privacy)|   | (Media/Feed/Likes)   |   | (Chat Histories) |   |Connections |   |
|     +----------------------+   +----------------------+   +------------------+   +------------+   |
+===================================================================================================+
```

### 2️⃣ End-to-End SCM Governance & Release Workflow
Combining the report's **Change Management**, **Version Management**, and **Release Management (Figure 10)** models yields a unified 10-stage quality gate pipeline that prevents unvalidated code or network configurations from reaching production:

```text
  [1. Change Identification & Formal CR Submission]
                         |
                         v
  [2. Impact, Risk & Security Assessment (Project Manager)]
                         |
                         v
  [3. Multi-Level CCB & Security Approval Gate]
                         |
                         v
  [4. Controlled Branch Implementation & Semantic Versioning]
                         |
                         v
  [5. Sandbox Build & Pre-Release Validation Suite]
      |-- Functional & Integration Testing
      |-- Performance / Load & Regression Testing
      |-- Penetration, Rate-Limit & Automated Abuse Testing
      |-- User Acceptance Testing (UAT)
                         |
                         v
  [6. 5-Role Release Sign-Off (PM, SQA, Sec, Config, Ops)]
                         |
                         v
  [7. Staging Environment Deployment & Verification]
                         |
                         v
  [8. Controlled Production Rollout (Canary / Blue-Green / Phased)]
                         |
                         v
  [9. Post-Release Telemetry, Log & Support Monitoring]
                         |
                +--------+--------+
                |  Issue Found?   |
                +--------+--------+
                   /           \
               [YES]           [NO]
                /                 \
               v                   v
  [10A. Automated Rollback   [10B. Release Closure &
   & Out-of-Band Hotfix]      Version Audit Archival]
```

---

## ✨ Core SCM Pillars & Proposed Lifecycle Models

### 🔄 Pillar 1: Software Change Management
Software systems undergo continuous evolution across four IEEE/ISO maintenance categories, each requiring tailored SQA review gates:
1. **Corrective Maintenance (Reactive):** Fixing discovered defects or vulnerabilities (e.g., patching the 2024 password reset brute-force flaw in `Password Reset Module v4.3`).
2. **Adaptive Maintenance (Environmental):** Modifying software to comply with new operating systems, hardware, or regulatory frameworks (e.g., adapting data handling workflows for EU GDPR compliance).
3. **Perfective Maintenance (Enhancement):** Adding new features or optimizing performance (e.g., rolling out Facebook Stories, Reels, and Marketplace).
4. **Preventative Maintenance (Proactive):** Refactoring architecture or configurations to prevent future failures (e.g., decoupling Meta's out-of-band recovery network from the main production backbone after the October 2021 outage).

#### Proposed 7-Stage Change Management Model for Meta
* **Stage 1 – Change Identification:** Submit a formal Change Request (CR) detailing the defect/enhancement, affected artifacts, and business justification.
* **Stage 2 – Change Assessment:** Conduct architectural impact analysis, security risk assessment, WBS schedule estimation, and budget calculation.
* **Stage 3 – Change Approval:** Multi-level sign-off by Team Leads, Senior Security Architects, and the Change Control Board (CCB).
* **Stage 4 – Change Implementation:** Develop the change in an isolated development environment adhering strictly to secure coding and documentation standards.
* **Stage 5 – Change Testing:** Execute mandatory functional, security (brute-force/scraping abuse), performance, and regression test suites in a non-production sandbox.
* **Stage 6 – Change Deployment:** Roll out the change via **Meta Conveyor** using staged deployment with pre-verified rollback scripts.
* **Stage 7 – Change Review:** Monitor post-deployment telemetry and error rates over a defined stabilization window, triggering immediate rollback if anomalies occur.

---

### 🌿 Pillar 2: Software Version Management
To eliminate configuration drift and untracked API modifications across thousands of daily commits, the study establishes a comprehensive **Software Configuration Management (SCM)** versioning framework:

#### Semantic Versioning & 5-Tier Branching Strategy
| Branch / Version Tier | Designation / Format | Engineering Purpose & Governance Rule |
| :--- | :---: | :--- |
| **Main Branch** | `main` (`v1.0`, `v2.0`) | Holds only production-grade, fully certified releases. Direct commits are strictly prohibited. |
| **Development Branch** | `develop` | Primary integration branch where completed features are merged for continuous integration verification. |
| **Feature Branches** | `feature/*` | Isolated workspaces for developing new perfective enhancements without destabilizing the main codebase. |
| **Testing / Staging Branch** | `test/*` / `release/*` | Dedicated pre-release branch subjected to functional, security, load, and regression testing. |
| **Hotfix Branch** | `hotfix/*` (`v2.1`, `v4.3`) | Emergency corrective branch forked from `main` to patch critical production vulnerabilities (e.g., 2024 ATO fix). |

#### Proposed 7-Stage Version Management Lifecycle Model
1. **Stage 1 – Version Creation:** Engineers develop features, bug fixes, or infrastructure-as-code (IaC) router configurations in isolated branches.
2. **Stage 2 – Version Registration:** Commits are registered in a centralized Git/GitHub/GitLab repository with immutable metadata (Author ID, Timestamp, Change Description, CR ID).
3. **Stage 3 – Peer Code & Security Review:** Senior developers inspect code quality, permissions boundaries, and compliance with privacy standards.
4. **Stage 4 – Multi-Dimensional Version Testing:** Automated and manual execution of Functional, Security, Performance, and Regression suites.
5. **Stage 5 – Version Approval & Release Tagging:** Formal QA and management sign-off locks the version tag for production build preparation.
6. **Stage 6 – Post-Release Version Monitoring:** Real-time telemetry tracks version health, latency, and user feedback in production.
7. **Stage 7 – Automated Version Rollback:** Instantaneous restoration of the previous certified stable version tag if critical failures or security alerts arise.

---

### 🚀 Pillar 3: Enterprise Release Management (DigitalConnect Solutions & Meta)
Evaluating the parallel case of **DigitalConnect Solutions**—a cloud customer service platform plagued by payment failures, database synchronization bugs, high-traffic slowdowns, and unapproved production pushes—the report establishes a structured **Release Management & Recovery Plan**:

#### 5-Role Release Approval Governance Matrix
No software build may transition from staging to production without explicit sign-off across five accountable stakeholders:

| Stakeholder Role | Release Governance Accountability |
| :--- | :--- |
| **1. Project Manager** | Evaluates WBS schedule alignment, business continuity impact, and overall release readiness. |
| **2. SQA Team** | Certifies that 100% of functional, integration, load, regression, and UAT test criteria have passed. |
| **3. Security Team** | Validates vulnerability patches, API rate-limiting, authentication controls, and penetration test reports. |
| **4. Configuration Manager** | Audits semantic version tags, build artifacts, dependency mappings, and release documentation traceability. |
| **5. Operations / DevOps Team** | Verifies production environment stability, out-of-band recovery readiness, and automated rollback triggers. |

#### Controlled Deployment Strategies
Rather than high-risk "big-bang" production cutovers, enterprise updates are deployed using progressive exposure strategies:
* **Canary Release:** Routes a small percentage (e.g., 1%–5%) of live user traffic to the new version to validate real-world payment and authentication stability before wider rollout.
* **Blue-Green Deployment:** Maintains two identical production environments (*Blue = Current Live*, *Green = New Release*), switching router traffic only after Green passes full health checks and enabling instant zero-downtime rollback.
* **Phased / Staggered Rollout:** Gradually expands deployment across geographic regions and data centers.
* **Pilot Release:** Deploys updates to an internal dogfooding or beta user cohort prior to general availability.

---

## 📸 Visual Walkthrough & 8-Module System Build Prototype

Prior to code construction, an interactive **8-screen Facebook Clone Web Application prototype** was engineered in **Figma** to validate user requirements, reduce cognitive load, and embed **ISO/IEC 9126** and **McCall’s** software quality factors directly into the user interface layer.

> 🔗 **Live Interactive Figma Prototype:** [Open Facebook Clone SQA Prototype in Figma](https://www.figma.com/design/6Ml2UgiSTdDEt3Sjcc3pXL/Software-Quality-Group-project?node-id=20-4&t=PvpTJJUhgsq7jsRh-1)

###  🖥️ Comprehensive 8-Module Interface & SQA Justification Matrix

| Figure | System Build Interface Module | Functional Description | Embedded SQA & McCall / ISO 9126 Quality Justifications |
| :---: | :--- | :--- | :--- |
| **Fig. 2** | **Login Page UI**<br>*(Authentication Module)* | Authenticates existing users via email/phone and password or OAuth (Google/Apple) with password recovery links. | • **Usability:** Minimalist layout reduces cognitive load and accelerates task completion.<br>• **Integrity & Security:** Enforces password masking and integrates rate-limited authentication verification.<br>• **Efficiency:** Lightweight client-side form validation minimizes unnecessary server round-trips. |
| **Fig. 3** | **Registration Page UI**<br>*(Onboarding Module)* | Enables new users to provision accounts by submitting personal details, birthdates, gender, and strong credentials. | • **Correctness:** Strict field-level input validation prevents malformed or incomplete database records.<br>• **Integrity:** Enforces password complexity rules and confirmation matching to prevent weak credentials.<br>• **Usability:** Step-by-step visual hierarchy guides user onboarding smoothly. |
| **Fig. 4** | **Home Feed Page UI**<br>*(Core Interaction Module)* | Central social hub displaying Stories, post creation tools (Live Video, Photo/Video), and chronological/algorithmic news feeds. | • **Efficiency:** Optimized component rendering supports fast DOM updates and media loading.<br>• **Reliability:** Standardized feed card containers ensure consistent data rendering without layout shifts.<br>• **Usability:** Familiar 3-column navigation lowers learning time to near zero. |
| **Fig. 5** | **User Profile Page UI**<br>*(Identity & Timeline Module)* | Displays user cover/avatar photos, bio metadata, friend counts, photo grids, and personal timeline posts. | • **Correctness:** Deterministic relational queries ensure accurate binding of profile data and user posts.<br>• **Maintainability:** Modular UI sub-components (Intro, Photos, Posts) allow independent updates without regression.<br>• **Usability:** Clear tab navigation (`Posts`, `About`, `Friends`, `Photos`). |
| **Fig. 6** | **Friend Request Page UI**<br>*(Social Graph Module)* | Manages incoming friend requests (`Confirm`/`Delete`), "People You May Know" suggestions, and sent request cancellations. | • **Usability:** High-contrast primary/secondary action buttons prevent accidental clicks and speed up decision-making.<br>• **Correctness & Reliability:** Real-time state updates maintain bidirectional consistency in the `Friend Connections` database. |
| **Fig. 7** | **Messaging Page UI**<br>*(Real-Time Chat Module)* | Full-screen real-time messaging interface with searchable conversation lists, media sharing, and chat privacy controls. | • **Reliability:** Real-time message synchronization guarantees ordered, lossless chat delivery.<br>• **Efficiency:** Low-latency WebSocket payload transmission.<br>• **Integrity:** End-to-end access controls and "Privacy & Support" panel protect private communications. |
| **Fig. 8** | **Notification Page UI**<br>*(Activity Alert Module)* | Aggregates real-time system alerts, likes, comments, friend requests, and community updates with filtering tabs (`All`, `Unread`). | • **Correctness:** Event-driven triggers ensure immediate, accurate reflection of platform interactions.<br>• **Usability:** Categorized filter pills and "Mark as Read" batch actions streamline alert management.<br>• **Efficiency:** Paginated ("See Previous Notifications") rendering prevents memory bloat. |
| **Fig. 9** | **Settings Page UI**<br>*(Privacy & Security Module)* | Centralized control panel for Personal Information, Security, Privacy, Notifications, Language, Appearance, and Account Deactivation. | • **Integrity & Security:** Dedicated **Security** and **Privacy** tabs empower granular control over profile visibility (`Friends Only`).<br>• **Maintainability:** Centralized preference management isolates configuration logic.<br>• **Usability:** Clean left-hand sidebar taxonomy eliminates settings confusion. |

### 📊 Summary of SQA Improvements Achieved Through the Prototype Design

| McCall / ISO 9126 Quality Factor | Architectural & UI Implementation in Facebook Clone Prototype |
| :--- | :--- |
| **Correctness** | Client- and server-side input validation, deterministic state updates, and accurate relational data rendering across feeds and profiles. |
| **Reliability** | Fault-tolerant authentication flows, real-time message synchronization, and consistent component states across user sessions. |
| **Efficiency** | Streamlined form verification, paginated notification/feed loading, and optimized navigation hierarchy for fast page response times. |
| **Integrity** | Password masking, strong credential enforcement, rate-limited password recovery, and granular user privacy controls (`Friends Only`). |
| **Usability** | Intuitive, consistent navigation bars, clear visual hierarchy, high-contrast action buttons, and minimal cognitive load. |
| **Maintainability** | 3-Tier modular architecture decoupling 6 Frontend UI views, 5 Backend Application modules, and 4 Database stores. |
| **Portability** | Responsive web layout engineered for seamless cross-browser and multi-device (desktop/mobile) adaptability. |

---

## 🧱 Deep-Dive Technical Governance & CCB Artifacts

<details>
<summary><b>📋 Click to Expand: Formal Change Request (CR) & CCB Decision Artifact (META-FB-2024-SEC-001)</b></summary>
<br>

To demonstrate enterprise Change Management governance in action, the project includes a complete three-section **Change Request Form** addressing **Issue 4 (2024 Facebook Password Reset Account Takeover Vulnerability)**:

### Section 1: Submitter – General Information
| Field | Documented Specification |
| :--- | :--- |
| **Project Name** | Facebook Platform Security Enhancement Project |
| **Project Number** | `META-FB-2024-SEC-001` |
| **Project Owner / Requestor** | Meta Platforms, Inc. / Meta Security Engineering Team |
| **Program / Initiative** | Facebook Password Reset Security Improvement Initiative |
| **Type of Change Request (CR)** | ☑ **Defect** (Emergency Security Remediation) |
| **Priority Level** | ☑ **Mandatory** |
| **Date Submitted / Date Required** | `15/03/2024` / `25/03/2024` |
| **Brief Description of Request** | Modify the Facebook password reset mechanism to eliminate the 6-digit code brute-force account takeover vulnerability discovered in 2024. |
| **Technical Details of Change** | Update the password reset process by implementing stronger identity verification mechanisms, enhanced validation procedures, rate-limiting lockouts, and additional authentication controls to prevent unauthorized account access. |
| **Risk Identification & Analysis** | 1. Delays in deployment expose users to active account takeover attacks.<br>2. New authentication controls may slightly impact user convenience.<br>3. Extensive regression testing is required to ensure existing login flows remain intact. |

### Section 2: Project Manager – Initial Impact Analysis
* **Work Products & Version Baseline to be Modified:**
  1. `Password Reset Module` — **v4.3**
  2. `Security Requirements Specification` — **v2.5**
  3. `Security Test Cases` — **v3.1**
* **Mandatory SQA / QC Validation Activities:**
  1. Security Testing
  2. Penetration Testing
  3. Regression Testing

#### Schedule & Effort Impact Breakdown
| Deliverable Description | Effort Hours | Date Required | Schedule / WBS Impact |
| :--- | :---: | :---: | :--- |
| **1. Password Reset Security Enhancement** | 40 hrs | `25/03/2024` | Minor (`WBS 2.1`) |
| **2. Security Testing Report** | 24 hrs | `27/03/2024` | Minor (`WBS 3.2`) |
| **3. Updated Security Documentation** | 8 hrs | `28/03/2024` | None (`WBS 4.1`) |
| **Total Schedule & Effort Impact** | **72 Hours** | **5 Days Duration** | **Completion: `30/03/2024`** |

#### Budget & Financial Impact Breakdown
$$\text{Total Cost Impact} = \$8,000_{\text{ (Development)}} + \$4,000_{\text{ (Security Testing)}} + \$1,000_{\text{ (Documentation)}} = \$13,000$$

### Section 3: Change Control Board (CCB) – Final Decision
* **CCB Decision:** ☑ **Approved** (Signed `16/03/2024` by Meta Change Control Board Chairperson)
* **Decision Justification:** The password reset vulnerability presents a high risk to user accounts and Meta's global reputation. The security and trust benefits of immediate remediation far outweigh the `$13,000` cost and `5-day` (72-hour) schedule impact.
* **Mandatory Deployment Conditions:** The updated `Password Reset Module v4.3` must successfully pass both **Penetration Testing** and **Regression Testing** in staging before public production deployment.

</details>

<details>
<summary><b>📦 Click to Expand: Sample Enterprise Release Plan (DigitalConnect Solutions Recovery Model)</b></summary>
<br>

| Release Plan Attribute | Enterprise Specification |
| :--- | :--- |
| **Target System** | DigitalConnect Solutions – Cloud Customer Service & Payment Platform |
| **Release Objectives** | Remediate payment transaction failures, optimize high-load response times, patch authentication vulnerabilities, and fix database synchronization lag. |
| **Impacted System Modules** | 1. Payment Processing Module<br>2. User Login & Authentication Module<br>3. Customer Service Request Module<br>4. Database Integration & Synchronization Services |
| **Mandatory Pre-Release Test Suite** | Functional Testing, Regression Testing, Database Integration Testing, High-Load Performance Testing, Security/Penetration Testing, and User Acceptance Testing (UAT). |
| **Controlled Deployment Strategy** | Phased Rollout / Canary Release starting with an isolated pilot user cohort before full traffic cutover. |
| **Automated Rollback Triggers** | Automatically revert to previous stable build if:<br>• Critical system crash occurs<br>• Unresolved security/intrusion alert fires<br>• Payment transaction error rate exceeds defined SLA threshold |
| **Required Release Sign-Offs** | Project Manager, SQA Team, Security Team, Configuration Manager, and DevOps/Operations Team. |

</details>

---

## 📂 Repository File Structure

```text
Software-Quality-Assurance-Meta-Case-Study/
├── assets/
│   ├── inti-university-seeklogo.png         # Official INTI International University Header Logo
│   └── System Architecture Diagram.png      # 3-Tier Modular Client-Server Architecture Diagram
├── Project Report.pdf                       # Full 59-Page Academic Report, CCB Form & Turnitin Audit (3% Similarity)
└── README.md                                # Executive Portfolio Documentation & Theoretical SQA Analysis
```

---

## 🚀 Viewing & Reproduction Guide

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/shahadathossain/Software-Quality-Assurance-Meta-Case-Study.git](https://github.com/shahadathossain/Software-Quality-Assurance-Meta-Case-Study.git)
   cd Software-Quality-Assurance-Meta-Case-Study
   ```
2. **Explore the Interactive Figma System Build Prototype:**
   * Open the live Figma workspace directly in your browser to inspect all 8 UI screens (`Login`, `Registration`, `Home Feed`, `Profile`, `Friend Requests`, `Messaging`, `Notifications`, and `Settings`):
   * 🔗 [https://www.figma.com/design/6Ml2UgiSTdDEt3Sjcc3pXL/Software-Quality-Group-project?node-id=20-4&t=PvpTJJUhgsq7jsRh-1](https://www.figma.com/design/6Ml2UgiSTdDEt3Sjcc3pXL/Software-Quality-Group-project?node-id=20-4&t=PvpTJJUhgsq7jsRh-1)
3. **Review the Complete 59-Page Technical Report & CCB Artifacts:**
   * Open `Project Report.pdf` to examine the full Change Request Form (`META-FB-2024-SEC-001`), comprehensive academic references (35 peer-reviewed and industry sources), and the Turnitin Originality Report (**3% overall similarity index**).

---

## 👥 Project Team & Author Details

| Name | Student ID | Section | Role & Module Contribution |
| :--- | :---: | :---: | :--- |
| **Shahadat Hossain** | `I26041279` | `6MB1` | **Lead SQA Architect & Technical Analyst** — Change Management Models, CCB Impact Analysis (`META-FB-2024-SEC-001`), ISO 9126 / McCall's / IEEE 610.12 Theoretical Mapping & System Architecture |
| **Md Arif Mahmud Oyion** | `Group 2` | `6MB1` | **UI/UX Prototype Lead & System Builder** — 8-Module Figma Interface Design, 3-Tier Client-Server Architecture Modeling & SQA Design Justification |
| **Keenjhar Lashari** | `Group 2` | `6MB1` | **Version Management Specialist** — SCM Repository Architecture, 5-Tier Git Branching Strategy & 7-Stage Version Lifecycle Modeling |
| **Koonj** | `Group 2` | `6MB1` | **Release Management & Recovery Specialist** — DigitalConnect Solutions Release Recovery Plan, 10-Stage Deployment Workflow & Rollback Governance |

---

<div align="center">
  <i>Developed for SDT4202 Software Quality (June 2026 Session) at INTI International University, Nilai, Malaysia under the Fully Funded International Student Mobility Scholarship Program.</i>
</div>