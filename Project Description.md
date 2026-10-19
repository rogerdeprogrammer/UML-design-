## Highheads Car Wash System

SYSTEM SOFTWARE DESIGN & PROJECT SPECIFICATION

## 1. Executive Summary

The Highheads Car Wash Management System is a comprehensive digital platform designed to automate and modernise car wash operations. The platform connects vehicle owners, wash station attendants, and facility managers through a unified real-time workflow. By replacing physical queues with structured online reservations, QR ticket scanning, automated bay assignment, and integrated payment processing, Highheads maximizes station throughput, cuts waiting times, and delivers full operational transparency.

## 2. Project Objectives

- Queue Elimination: Allow customers to pre-book specific time slots and select wash packages remotely.

- Real-Time Tracking: Provide live updates on vehicle wash status (Scheduled → In Queue → Washing → Drying → Completed).

- Dynamic Bay Routing: Assign incoming vehicles to available wash lanes automatically upon arrival scanning.

- Multi-Channel Payments: Support direct online checkout via Mobile Money, Credit/Debit cards, and cash logging.

- Business Intelligence: Equip management with clear metrics on daily revenue, peak hours, and staff productivity.

## 3. User Roles & System Personas

|   | Role Primary Responsibilities Core System Benefits Registers vehicles, books wash slots, Guaranteed wash times, no line waiting, Customer pays online, and tracks wash transparent package pricing, and digital receipts. progress. Scans customer QR tickets at entry Clear daily bay schedules, simple touch Attendant gate, updates wash stage status in interface, eliminated manual paperwork. real-time. Configures wash packages, sets Complete financial oversight, peak hour load Admin / Manager pricing, manages staff shifts, reviews balancing, and operational insights. revenue reports. |
| --- | --- |


## 4. System Architecture & Modules

| Customer Module | Attendant Station | Admin Dashboard |
| --- | --- | --- |
| User & Vehicle Profiles | QR & Code Ticket Scanner | Dynamic Package Rates |
| Interactive Slot Booking | One-Tap Stage Controls | Revenue & Sales Analytics |
| Package & Add-on Selection | Bay Status Toggle | Staff Shift Management |
| Payment Gateway Integration | Lane Assignment Display | Bay & Equipment Monitor |
| Live Status Progress Bar | Completed Wash Log | Customer CRM & Logs |

## 5. Non-Functional Requirements

- Performance: Sub-second verification of ticket QR codes and real-time state synchronization across devices.

- Usability: Touch-first, high-contrast user interface optimized for handheld devices and outdoor sunlight reading.

- Security: Encrypted payment tokenization, Role-Based Access Control (RBAC), and HTTPS secure transport.

- Scalability: Modular architecture capable of expanding from a single site to multi-branch operations.

## 6. Recommended Technology Stack

| Layer | Technology Choices | Function |
| --- | --- | --- |
|   | React.js / Tailwind CSS | Responsive web application for desktop and mobile |
| Frontend |   | devices. |
|   | Node.js (Express) or | High-performance RESTful API and WebSocket |
| Backend API | Python (FastAPI) | connection engine. |
|   | PostgreSQL / Redis | Relational storage for bookings/financials; Redis for |
| Database |   | queue state caching. |
|   | Stripe / Mobile Money API | Automated payment processing and instant |
| Integrations | / Twilio | SMS/WhatsApp ticket updates. |
