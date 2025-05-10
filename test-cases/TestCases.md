# **Test Cases for Real-Time Air Quality Monitoring Dashboard**

## Test Case 1 - **Admin Login Button Validation**

**Test Case ID:** TC_001

**Test Title:** Verify Admin Login button redirects to the correct login page.

**Test Description:**

This test ensures the "Admin Login" button is functional and directs users to the correct admin authentication page.

**Test Steps:**

1. Navigate to the ClearSky dashboard .
2. Locate the "Admin Login" button .
3. Click the button.

**Test Data:**

- **User Role:** Unauthenticated user.
- **Expected Redirect URL:** **`https://clearsky.dizzpy.dev/admin/login.`**

**Expected Result:**

- The "Admin Login" button is visible and clickable.
- Clicking it redirects to the correct admin login page (**`/admin/login`**).
- The login page loads without errors.

**Post-Condition:**

- User lands on the admin login page.

**Actual Result:** [Fill in after execution].

**Status:** [Pass/Fail]

**Notes:**

- If the button is missing, verify permissions.
- Test on both mobile and desktop views if applicable.

## **Test Case 2 - Validate Active Alerts Accuracy**

**Test Case ID:** TC_002

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


