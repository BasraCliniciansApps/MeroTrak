# 💊 MeroTrack - Antimicrobial Stewardship & Meropenem Tracking System

**MeroTrack** is a lightweight, real-time Progressive Web Application (PWA) designed to bridge the communication gap between hospital inpatient pharmacies and the Microbiology Laboratory. It tracks **Meropenem** prescription requests, ensures compliance with culture sample submission protocols prior to antibiotic dispensing, and provides monthly analytics for Antimicrobial Stewardship Programs (ASP).

---

## 🌟 Key Features

- **Pharmacy Request Entry:** Streamlined form for inpatient pharmacists to record patient details, Statistical Number (MRN), treating physician, ward/department, and prescription date.
- **Smart Duplicate Detection:** Algorithms automatically detect duplicate entries within a 30-day window using normalized patient names or Statistical Numbers (MRNs) to prevent redundant culture orders.
- **Microbiology Lab Verification:** Secure confirmation or rejection of culture sample receipts protected by passcode access.
- **Time-Elapsed Delay Indicators:** Visual color-coded status badges alerting staff to pending samples (>24 hours orange warning, >48 hours critical red alert).
- **Physician Sample Refusal Tracking:** Dedicated option to log explicit physician decisions to dispense without a culture sample, maintaining administrative transparency.
- **Monthly Analytics & Dashboard (`stats.html`):**
  - KPI summary cards (Total Orders, Confirmed, Rejected, Pending, Doctor Refusals).
  - Interactive charts powered by **Chart.js** (Status Distribution, Prescribing Wards, Top Prescribing Physicians).
  - Professional Non-Compliance Analysis table evaluating physician sample submission rates.
- **Soft Delete & Audit Protection:** Prevents accidental or unauthorized data loss through soft-deletion backed by dedicated passcodes and Firestore rules.
- **Mobile-First & PWA Enabled:** Card-based UI optimized for mobile devices with single-tap home screen installation.

---

## 🛠️ Tech Stack & Dependencies

- **Frontend:** HTML5, CSS3, JavaScript (ES6 Modules), Bootstrap 5.3 (RTL)
- **Icons & Visuals:** Bootstrap Icons, Chart.js
- **Backend & Database:** Google Firebase Firestore (Realtime Cloud Database)
- **Hosting & Deployment:** GitHub Pages (PWA / Web App)

---

## 📁 Repository Structure

```text
├── index.html        # Main Application Interface (Pharmacy Order Entry & Lab Actions)
├── stats.html        # Monthly Analytics & Reporting Dashboard
├── manifest.json     # PWA Web App Manifest Configuration
├── icon.png          # Application Icon (512x512 PNG)
└── README.md         # Project Documentation
