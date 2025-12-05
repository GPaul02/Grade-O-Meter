# Quality Assurance Test Cases

| Test ID | Feature | Test Step | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC-01** | **Freshness Detection** | Upload `sample_data/sample_fresh_1.jpg` | System detects **Grade A (Premium)** with >90% confidence. | ✅ PASS |
| **TC-02** | **Defect Detection** | Upload `sample_data/sample_rotten_1.jpg` | System detects **Grade B (Low Quality)** with >90% confidence. | ✅ PASS |
| **TC-03** | **Geolocation** | Open app and allow location permissions | GPS Coordinates appear in the Sidebar. | ✅ PASS |
| **TC-04** | **Batch Logging** | Scan 3 images and click "Log to Batch" | "Total Scanned" count updates to 3. | ✅ PASS |
| **TC-05** | **Report Generation** | Click "Print Report" button | Browser opens Print/Save as PDF dialog. | ✅ PASS |
