# **Test Cases for Real-Time Air Quality Monitoring Dashboard**

## **Test Case 1 - Validate Active Alerts Accuracy**

**Test Case ID:** TC_001

**Test Title:** Verify Critical and Warning Alerts Display Correctly.

**Test Description:**

Ensure that active alerts reflect real -time sensor data and preferred according to severity.

**Test Steps:**

1. Navigate to the **"Active Alerts"** section.
2. Verify the displayed alert messages.
3. Cross-check alerts with live sensor data:
    - **Critical Alert:** SNR-002
    - **Warning Alert:** SNR-001

**Test Data:**

- **Critical Alert:** *"High PM2.5 at Downtown (SNR-002)."*
- **Warning Alert:** *"Moderate AQI at Central Park (SNR-001)."*

**Expected Result:**

- Alerts match real-time sensor readings.
- Severity levels (Critical/Warning) are correctly prioritized.

**Post-Condition:** None

**Actual Result:** [To be filled after execution]

**Status:** [Pass/Fail]

### **Notes:**

- Alerts should update dynamically if sensor data changes.
- Verify timestamp accuracy for alert generation.