# 🌫️ Real-Time Air Quality Monitoring Dashboard

This is a web-based dashboard designed to monitor real-time air quality across various regions of Colombo. The system collects data from IoT-based air quality sensors and visualizes it in an intuitive interface for users and administrators. It features alert systems, user authentication, and data filtering capabilities.

---

## 📌 Project Overview

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** PHP (Laravel)  
- **Database:** MySQL  
- **Project Type:** University Coursework  
- **Team:** Matheesha and team  
- **Features:**
  - Real-time AQI data from sensors
  - Admin and user roles
  - Alert systems for critical air quality
  - Search and filter AQI by location
  - Secure login/logout mechanism

---

## ✅ Testing Summary

This project includes both **manual** and **automated** testing to ensure system reliability and usability.

### 📄 Test Plan

- **Tested By:** QA Team (University Group)
- **Start Date:** May 1, 2025  
- **End Date:** May 9, 2025  
- **Test Methodology:** Manual testing using Google Chrome, Firefox, and Safari browsers on desktop and mobile.

#### 🧪 Testing Tools
- **Browsers:** Chrome, Firefox, Safari  
- **Database:** MySQL Workbench  
- **Testing Platform:** localhost  
- **Bug Tracking:** GitHub Issues (private repo)

---

## 🧪 Manual Test Cases

| Test Case ID | Description | Expected Result | Status |
|--------------|-------------|------------------|--------|
| TC01 | User Login | Redirect to dashboard on success | ✅ Pass |
| TC02 | Sensor Data Display | Data from all sensors displayed | ✅ Pass |
| TC03 | Alert Generation | Alerts trigger if AQI > 150 | ✅ Pass |
| TC04 | Admin Access | Admin can manage sensors | ✅ Pass |
| TC05 | User Registration | Unique email check, success redirect | ✅ Pass |
| TC06 | Filter by Location | Filters AQI data by region | ✅ Pass |
| TC07 | Logout Functionality | User session ends, redirect to login | ✅ Pass |
| TC08 | Sensor Status Indicator | Displays “Active”/“Inactive” correctly | ✅ Pass |
| TC09 | Performance – Load Time | Dashboard loads < 2 sec | ✅ Pass |
| TC10 | SQL Injection Protection | Blocks injection attempts | ✅ Pass |

---

## 📄 Test Deliverables

- ✅ Test Plan Document  
- ✅ Manual Test Case Report  
- ✅ Bug Report Summary  
- ✅ Screenshots of Test Runs  
- ✅ README File (this)

---

## 🛡️ Security & Performance

- Login form is secured against basic SQL injection.
- Session management uses Laravel Auth for role-based access.
- Dashboard tested under simulated high-load for acceptable latency.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/air-quality-dashboard.git
