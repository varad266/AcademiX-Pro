🎓 AcademiX-Pro

⚠️Closed-Source / Production Software Note: > AcademiX is a fully deployed, commercial enterprise application currently used in production by educational institutes. To protect proprietary business logic and client security, the source code is not publicly available. This repository serves as a technical showcase of the system's architecture, feature set, and the engineering challenges solved during its development.

AcademiX Pro is a comprehensive, multi-tenant desktop application designed to digitalize and streamline school administration. Built entirely in Python, it bypasses standard web-app limitations by offering deep OS integration, hardware compatibility (biometric scanners), and lightning-fast local execution with a robust PostgreSQL backend.

From handling admissions and automated fee calculations to generating pixel-perfect, government-compliant Transfer Certificates, AcademiX is built to handle the rigorous demands of modern educational institutes.

🛠️ Tech Stack & Architecture
Frontend GUI: Python, PySide6 (Qt framework) with responsive, DPI-aware vector scaling.

Database: PostgreSQL (Relational schema with strict data integrity and foreign-key constraints).

Document Engine: ReportLab (Vector-based PDF generation for flawless print scaling).

Hardware Integration: Custom listener daemons for Biometric/RFID scanners.

Packaging & Deployment: PyInstaller (Executable compilation) + Inno Setup (Custom deployment wizard with silent PostgreSQL background installation and update-awareness).

✨ Core Modules & Features
👨‍🎓 1. Student & Admissions Management
Complete Lifecycle Tracking: Manages student data from admission to graduation.

Compliance-Ready Certificates: Dynamically generates Bonafide, Leaving Certificates (LC), and Transfer Certificates (TC).

Tabular PDF Rendering: Bypasses simple HTML-to-PDF converters by using ReportLab to draw strict, mathematically aligned tabular grids that match state-board stationery formats exactly.

💰 2. Financial & Fee Management
Dynamic Fee Structures: Admins can define custom fee heads (Tuition, Bus, Uniform) per class/session.

Live Balance Calculation: Automatically computes total dues, paid amounts, and pending balances in real-time.

Overpayment Protection: Transaction logic explicitly prevents cashier errors and over-crediting.

Automated Receipt Generation: Generates official branded fee receipts with automated transaction ID generation and watermarks.

📊 3. Examination & Academic Module
Dynamic Grading System: Teachers input marks into a dynamically generated grid based on the class's specific syllabus.

Auto-Calculation: Automatically calculates total marks, percentages, and assigns grades (A1, B2, etc.) based on standard academic thresholds.

Report Card Generation: One-click generation of beautifully formatted, print-ready PDF Report Cards featuring automated pass/fail logic and grading scales.

Data Export: Seamless extraction of full-class result sheets to .csv for Excel analysis.

👥 4. Staff & HR Management
Role Allocation: Manages teacher-to-subject and class-teacher allocations.

Promotion & Salary Revision: Dedicated UI for handling staff promotions, tracking new designations, and effective salary dates.

Designation Directory: Centralized control over school departments (Admin, Teaching, Support, etc.).

🚀 Notable Technical Achievements
Zero-Friction Deployment Pipeline: Engineered a custom Inno Setup script that bundles the Python .exe, internal graphical assets (logos/icons), and the PostgreSQL Windows installer. It silently installs the database engine, configures the superuser, and creates the schemas in the background without user intervention.

Update-Aware Architecture: The installer detects existing PostgreSQL installations to prevent data corruption during software updates, allowing seamless rolling updates to the client.

Responsive Desktop UI: Moved away from fixed-pixel layouts to a highly responsive, pt-based DPI-aware UI utilizing QGridLayout and QStackedWidget for a fluid experience on any monitor size.

State Preservation: Implemented context managers to preserve user selections (Academic Session, Selected Classes) across tab switches and data refreshes, ensuring a premium UX.

📸 Application Previews
(Note: As the code is private, here are some previews of the user interface and generated documents.)

<img width="1918" height="1017" alt="image" src="https://github.com/user-attachments/assets/19b5b75e-6343-4af6-b7c2-d2ea6ccb74e6" />

<img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/be9b1183-5740-4f7e-82e1-b134d8bce01e" />


<img width="648" height="871" alt="image" src="https://github.com/user-attachments/assets/050a129f-98b5-415d-a9eb-2b107bdaf5d4" />

Developed by Varad Ambejogaiar Software Developer | Desktop & Application Architecture
