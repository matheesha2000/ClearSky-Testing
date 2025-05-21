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


## Test Case 3 - Verify AQI Legend Ranges

**Test Case ID:** TC_003

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

## Test Case 4 - Test Historical Trends Filtering

**Test Case ID: TC_004**

**Test Title: Verify Historical Trends Graph Updates with Sensor and Timeframe Filters**

**Test Description:**

Ensure the historical trends graph dynamically updates when users apply sensor and timeframe filters, as accurate data visualization is critical for trend analysis.

**Test Steps:**

1. Navigate to the **Historical Trends** section.
2. From the **sensor dropdown**, select **"SNR-001"**.
3. Change the **timeframe filter** to **"Last 24 Hours"**.
4. Verify the graph refreshes to display:
   - Data **only from SNR-001**.
   - Data points **within the last 24 hours**.

**Test Data:**

- **Sensor:** SNR-001
- **Timeframe:** Last 24 Hours

**Expected Result:**

- Graph updates **without errors** to reflect SNR-001’s data for the selected 24-hour period.
- No missing/blank data sections (unless no data exists for the timeframe).

**Post-Condition:**

- Graph persists with the applied filters until changed again.

**Actual Result:** [To be filled after execution]

**Status:** [Pass/Fail]

**Notes:**

- **Potential failure points:**
   - Delays (>3 seconds) in graph rendering.
   - Incorrect/mixed sensor data displayed.
   - Empty graph with valid data expected.
- Test edge cases.

## **Test Case 5 – Valid Admin Login**

**Test Case ID:** TC_005

**Test Title:** Verify that a registered admin can log in successfully with valid credentials.

**Test Description:**

This test ensures that the system provides access to a administrator user when a registered email and the correct password is recorded.

**Test Steps:**

1. Open the clearsky admin login page in a browser.
2.  Enter a recognized administrator email  and password
3. Click the "Login" button.

**Test Data:**

- Email: **`admin@clearsky.com`**
- Password: **`AdminPass123`**

**Expected Result:**

- The admin should be successfully authenticated.
- The system should redirect the admin to the dashboard page.
- A valid session token should be generated.

**Post-Condition:**

- Admin is logged in.
- Session remains active until logout or expiration.

**Actual Result:  [Fill in after execution]**

**Status:  [Pass/Fail]**

**Notes:**

- Session token was validated successfully.
- No unexpected delays or errors occurred during login.

## **Test Case 6 – Invalid Admin Login**

**Test Case ID:**  TC_006

**Test Title:**  Verify that the system rejects login attempts with invalid credentials.

**Test Description:**

This test ensures that unauthorized users cannot log in with incorrect email/password combinations.

**Test Steps:**

1. Navigate to the ClearSky admin login page.
2. Enter an invalid email  and password
3. Click the "Login" button.

**Test Data:**

- Email: **`wrong@clearsky.com`**
- Password: **`WrongPass`**

**Expected Result:**

- The system should display an error message.
- The user should remain on the login page.
- No session should be created.

**Post-Condition:**

- Login page remains open; no redirection occurs.

**Actual Result:  [Fill in after execution]**

**Status: [Pass/Fail]**

**Notes:**

- The error message did not specify whether the email or password was incorrect (good security practice).

## **Test Case 7 – Create Admin Successfully**

**Test Case ID:**  TC_007

**Test Title:**  Verify that a new admin account can be created with valid details.

**Test Description:**

This test confirms that the system allows the construction of a new administrator account when all the necessary fields are filled correctly.

**Test Steps:**

1. Go to the "Create Admin" page.
2. Fill in all mandatory fields (Name, Email, Password).
3. Click the **"**Create Account" button.

**Test Data:**

- Name: **`Alice Admin`**
- Email: **`alice@clearsky.com`**
- Password: **`NewAdmin123`**

**Expected Result:**

- A success message appears (e.g., "Admin account created successfully").
- The new admin  appears in the admin list.

**Post-Condition:**

- The new admin is visible in the system and can log in.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- The system correctly enforced email uniqueness (no duplicates allowed).

## **Test Case 8 – Duplicate Email Check**

**Test Case ID:** TC_008

**Test Title:** Ensure the system prevents duplicate email registrations.

**Test Description:**

This test verification that the system detects and the block tries to register a administrator with a pre -registered email.

**Test Steps:**

1. Navigate to the **"**Create Admin**"** page.
2. Enter an email that already exists
3. Submit the form.

**Test Data:**

- Email**:** **`admin@clearsky.com`**

**Expected Result:**

- The system should display an error (e.g., "Email already registered").
- No new admin account should be created.

**Post-Condition:**

- The form remains open with an error message.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- The email check was **case-insensitive.**

## **Test Case 9 – Verify Navigation Menu Functionality**

**Test Case ID:** TC_009

**Test Title:** Ensure navigation menu items work correctly and reflect proper active/inactive states.

**Test Description:**

This test checks whether clicking menu items redirects to the correct pages and whether active sections are visually highlighted.

**Test Steps:**

1. Log in as an admin.
2. Click each menu item (e.g., **Sensor Management, Profile Settings**).
3. Observe:
   - Page redirection.
   - Checkmark or highlight for active sections.
   - No checkmark for inactive sections.

**Test Data:**

- **Active (Checked) Items:**
   - Sensor Management
   - Admin Management
   - Profile Settings
- **Inactive (Unchecked) Items:**
   - Dashboard
   - Data Simulation
   - Alert Configuration
   - System Settings

**Expected Result:**

- Clicking a menu item redirects to the correct page.
- Active sections remain highlighted .
- Inactive sections show no checkmark.

**Post-Condition:**

- User lands on the selected page.
- Menu state updates accordingly.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- Test both checked and unchecked items for consistency.
- Ensure that the active state persists after page reload.

## Test Case 10 – Validate System Status Metrics Accuracy

**Test Case ID:** TC_010

**Test Title:** Verify real-time system metrics display accurate performance data.

**Test Description:**

This test ensures the dashboard correctly reflects live system health metrics (CPU load, memory, storage) within an acceptable tolerance range.

**Test Steps:**

1. Log in and navigate to the **System Status** dashboard.
2. Compare displayed values against actual server metrics.
   - **System Load:** 52% (Expected range: 47–57%)
   - **Memory Usage:** 60% (Expected range: 55–65%)
   - **Storage:** 40% (Expected range: 35–45%)
3. Simulate load spikes (e.g., run a CPU-intensive task) and refresh to verify updates.

**Test Data:**

- Metrics
- System Load: 52%
- Memory Usage: 60%
- Storage: 40%

**Expected Result:**

- Metrics match real server data within ±5% tolerance.
- Values update either in real-time (e.g., every 30 seconds) or upon manual refresh.

**Post-Condition:**

Dashboard reflects current system state without delays.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- Tested with server monitoring tools.
- Real-time updates worked as documented.

## **Test Case 11 – View Sensor List**

**Test Case ID:** TC_011

**Test Title:** Confirm the sensor list loads and displays correctly.

**Test Description:**

Validate that the Sensor Management page loads all preconfigured sensors with accurate details (ID, type, location).

**Test Steps:**

1. Log in as admin.
2. Navigate to **Sen**sor **M**anagemen**t**.
3. Verify the list contains seeded sensor data (e.g., 10 dummy sensors).

**Test Data:** Sensor data seeded

**Expected Result:**

- Sensors appear in a readable table format.
- Default sort: Newest sensors first (by creation date).

**Post-Condition:**

All sensors are visible; no data truncation.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- Pagination handled 50+ sensors smoothly.

## **Test Case 12 – Filter Sensors**

**Test Case ID:** TC_012

**Test Title:** Test filtering and sorting functionality.

**Test Description:**

Ensure users can narrow down sensors by type/location and sort by columns.

**Test Steps:**

1. Go to **Sensor Management**.
2. Apply filter: **Type = CO2**.
3. Sort by **"Location" (A-Z)**.

**Test Data:**

- Filter by: Type = CO2

**Expected Result:**

- Only CO2 sensors appear.
- Locations sorted alphabetically (e.g., "Lab 1" → "Warehouse").

**Post-Condition:**

Filters persist until cleared.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- UI dropdowns responded instantly.

## **Test Case 13 – Add New Gas Sensor with Valid Data**

**Test Case ID:** TC_013

**Test Title:** Successfully register a new gas sensor.

**Test Description:**

Verify the system accepts a new sensor when all mandatory fields are valid.

**Test Steps:**

1. Navigate to Add New Gas Sensor.
2. Fill in:
   - Name: "Warehouse CO2 Monitor"
   - Location**:** "Warehouse Zone 1"
   - Type**:** CO2
   - Threshold: 75
   - Start Date: 2025-04-25
3. Click Add New Sensor.

**Test Data:**

- Sensor Name: "Warehouse CO2 Monitor"
- Location: "Warehouse Zone 1"
- Sensor Type: "CO2"
- Threshold: "75"
- Start Date: "2025-04-25"

**Expected Result:**

- Success toast: *"Sensor added successfully!"*
- New sensor appears in the list with an auto-generated ID.

**Post-Condition:**

Total sensor count increments by 1.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- ID was unique and followed naming convention.

## **Test Case 14 – Attempt to Add Sensor with Missing Fields**

**Test Case ID:** TC_014

**Test Title:** Block submission if required fields are empty.

**Test Description:**

Ensure the system enforces validation and prevents incomplete submissions.

**Test Steps:**

1. Go to **Add New Gas Sensor**.
2. Leave **Sensor Name** blank.
3. Fill other fields:
   - **Location:** "Lab 3"
   - **Type:** Methane
   - **Threshold:** 50
4. Click **Add New Sensor**.

**Test Data:**

- Sensor Name: (Blank)
- Location: "Lab 3"
- Sensor Type: "Methane"
- Threshold: "50"
- Start Date: "2025-04-25"

**Expected Result:**

- Error message: *"Sensor Name is required."*
- Form remains open; no network request sent.

**Post-Condition:**

Sensor count unchanged.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- Repeat for **Location** and Threshold (all passed).

## **Test Case 15 – Configure and Start a Quick Simulation**

**Test Case ID:** TC_015

**Test Title:** Validate Quick Simulation with Random Data

**Test Description:** Ensure the system generates and displays simulated sensor data within configured thresholds.

**Test Case Steps:**

1. Navigate to the "Data Simulation" page.
2. Select "Test Union" as the sensor.
3. Set **Pattern Type** to "Random."
4. Configure:
   - Update Frequency: 5 minutes
   - Min Value: 350
   - Max Value: 2000
   - Thresholds: 1400, 1800
5. Click **Quick Start**.
6. Observe the "Line Data" section for live updates.

**Test Data:**

- Sensor: Test Union
- Min/Max: 350–2000
- Thresholds: 1400 (warning), 1800 (critical)

**Expected Result:**

- Data appears in "Line Data" within 5 minutes.
- Values stay between 350–2000.
- Threshold alerts trigger if data crosses 1400 or 1800.

**Post Condition:** Simulation logs appear in "Simulation History."

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:** Verify alerts  and data persistence.

## **Test Case 16 – Verify Simulation History Logging**

**Test Case ID:** TC_016

**Test Title:** Validate Historical Data Accuracy

**Test Description:** Confirm completed simulations are logged with correct parameters.

**Test Case Steps:**

1. Run a quick simulation (as in TC001).
2. Go to the "Simulation History" table.
3. Locate the latest entry for "Test Union."
4. Verify the logged details:
   - Sensor name
   - Pattern type ("Random")
   - Duration (e.g., "00:00:22")
   - Min/Max values (350/2000)
5. Click **View Data** to inspect details.

**Test Data:** Use the most recent "Test Union" entry.

**Expected Result:**

- History entry matches configured settings.
- "View Data" shows correct min/max/pattern.

**Post Condition:** No data corruption or missing entries.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:** Check timestamp accuracy and data integrity.

## **Test Case 17 – Update Default Threshold Value & Verify Persistence**

**Test Case ID:** TC_017

**Test Title:** Ensure the system saves and applies the new default threshold for sensors.

**Test Description:** This validates core configuration functionality affecting all future sensors.

**Test Steps:**

1. Navigate to **Global Alert Settings**.
2. Change **Default Threshold Value (ppm)** from **`100`** to **`120`**.
3. Click **Save Settings**.
4. Refresh the page and verify the value remains **`120`**.

**Test Data:**

- Field: Default Threshold Value
- Input: **`120`** (valid positive integer)

**Expected Result:** The value **`120`** is retained after saving and refreshing.

**Post Condition:** New sensors will use **`120 ppm`** as the default threshold.

**Actual Result:** [Fill in after execution]

**Status: [Pass/Fail]**

**Notes:**

- Critical for system-wide consistency.
- Test edge cases (e.g., negative values, decimals) separately.

## **Test Case 18 – Trigger Critical Alert via Threshold Breach**

**Test Title:** Validate critical alerts are triggered when data exceeds 150% of the threshold.

**Test Description:** Confirms the system detects and escalates critical alerts as configured.

**Test Steps:**

1. Set **Default Threshold Value** to **`100`** ppm.
2. Ensure **Critical Alert Threshold (%)** is **`150`**.
3. Simulate sensor data reaching **`151`** ppm.
4. Check **Active Alerts** for a critical alert.

**Test Data:**

- Sensor Threshold: **`100`** ppm
- Simulated Data: **`151`** ppm (150% + 1).

**Expected Result:** A critical alert appears in **Active Alerts**.

**Post Condition:** Alert is logged; notifications fire if enabled.

**Actual Result:** [Fill in after execution]

**Status:**  **[Pass/Fail]**

**Notes:**

- Tests both threshold calculation and alert visibility.
- Integrates with notification settings (email/SMS) if enabled.

## **Test Case 19 – View Admins**

**Test Case ID:** TC_019

**Test Title:** Display Admin List**

**Test Description:**

This test confirms that the admin management page correctly loads and displays the list of administrators.

**Test Steps:**

1. Navigate to Admin Management.

**Test Data:**

- **Precondition:** Existing admin accounts in the system.

**Expected Result:**

- A table listing all admins should be displayed, along with available actions (edit, delete, etc.).

**Post-Condition:**

- The admin list remains accessible for management.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- The table supports pagination, allowing smooth navigation through multiple entries.

## **Test Case 20 – Delete Admin Account**

**Test Case ID:** TC_020

**Test Title:** Delete Admin Account

**Test Description:**

This test ensures that an administrator can successfully delete another admin account while preventing accidental self-deletion (a critical security measure).

**Test Steps:**

1. Navigate to the Admin Management page.
2. Locate the target admin account and click the Delete button.
3. Confirm the deletion in the pop-up dialog.

**Test Data:**

- Admin ID: A pre-existing admin account.

**Expected Result:**

- The selected admin account should be permanently removed from the system.

**Post-Condition:**

- The deleted admin no longer appears in the admin list and loses all access.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- The system correctly blocked attempts to delete the *currently logged-in* admin (self-deletion), ensuring account security.

## **Test Case 21 – Update System Preferences**

**Test Case ID:** TC_021

**Test Title:** Update System Preferences

**Test Description:**

This test verifies that global system settings (e.g., timezone, units) can be modified and persist across sessions.

**Test Steps:**

1. Go to **System Settings**.
2. Update the **Timezone** field to *UTC+5:30* 
3. Click **Save** to apply changes.

**Test Data:**

- Timezone: UTC+5:30.

**Expected Result:**

- The new timezone should be saved and reflected across the system immediately.

**Post-Condition:**

- All time-based data (logs, alerts) now align with the updated timezone.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- Changes remained intact even after refreshing the page, confirming proper backend storage.

## **Test Case 22 – Invalid System Setting Input**

**Test Case ID:** TC_022

**Test Title:** Invalid System Setting Input

**Test Description:**

This test assumes that the system rejects invalid or fruitless input with clear error messages.

**Test Steps:**

1. Navigate to **System Settings**.
2. In the Unit field, enter ”abc123”.
3. Attempt to submit the form.

**Test Data:**

- Unit Field Input: “abc123”

**Expected Result:**

- The system should display an error message and prevent saving.

**Post-Condition:**

- The original system setting remains unchanged.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- The frontend validation was robust, catching the error before any API call was made.

## **Test Case 23 – Update Admin Profile Info**

**Test Case ID:** TC_023

**Test Title:** Edit Admin Profile

**Test Description:**

This test confirms that administrators can update their personal profile information (e.g., name) with immediate effect.

**Test Steps:**

1. Open Profile Settings from the user dropdown.
2. Change the *Name* field to *"John Admin"*.
3. Click **Save**.

**Test Data:**

- New Name: John Admin

**Expected Result:**

- The updated name should appear in the profile header and across the system.

**Post-Condition:**

- The admin’s profile reflects the new name in all relevant sections.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- No cache issues were observed; the new name loaded consistently.

## **Test Case 24 – Invalid Data**

**Test Case ID:** TC_024

**Test Title:** Invalid Input in Profile

**Test Description:**

This test ensures the system blocks profile updates containing invalid characters (e.g., symbols) in the name field.

**Test Steps:**

1. Go to Profile Settings.
2. Enter *"@dm!n"*  into the *Name* field.
3. Click Save.

**Test Data:**

- **Name Input:** "@dm!n"

**Expected Result:**

- The system should reject the input with a validation error.

**Post-Condition:**

- The profile name remains unchanged.

**Actual Result:** [Fill in after execution]

**Status:** [Pass/Fail]

**Notes:**

- The regex-based validation worked perfectly, allowing only alphanumeric characters and spaces.


