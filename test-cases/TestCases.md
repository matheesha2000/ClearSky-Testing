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



## Test Case 2 - Verify AQI Legend Ranges

**Test Case ID:** TC_002

**Test Title:** Verify AQI Legend Ranges Match EPA/WHO Standards

**Test Description:**

AQI categories ensure that EPA/WHO use the correct numeric boundaries according to the guidelines.

**Test Steps:**

1. Navigate to the dashboard and locate the **"AQI Legend"** section.
2. Compare each displayed AQI range against official EPA/WHO standards:
   - Good
   - Moderate
   - Unhealthy for Sensitive Groups
   - Unhealthy

**Test Data:**

- **Good:** 0–50
- **Moderate:** 51–100
- **Unhealthy for Sensitive Groups:** 101–150
- **Unhealthy:** 151–200

**Expected Result:**

All AQI ranges in the legend **exactly match** the EPA/WHO standard ranges.

**Post-Condition:** None

**Actual Result:** [To be filled after execution]

**Status: [**Pass/Fail]

**Notes:**

- Critical for user safety and decision-making.
- Flag discrepancies immediately if ranges deviate from standards.