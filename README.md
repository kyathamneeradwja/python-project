# Police Station Management System

This project implements a **Police Station Management System** using Python. It helps manage FIRs (First Information Reports) efficiently by allowing users to file, close, and view FIRs based on various criteria.

---

## Features

1. **File FIR:**
   - Collects complainant's name, phone number, address, case type (civil/crime), and a case description.
   - Automatically assigns a unique case ID starting from 1.
   - Prevents duplicate FIRs by checking if a similar case already exists.

2. **Close Case:**
   - Allows users to mark a case as solved by providing the case ID.
   - Automatically records the close date.

3. **View Pending Cases:**
   - Displays pending cases filtered by their type (civil/crime).

4. **View Solved Cases:**
   - Displays solved cases filtered by their type (civil/crime).

5. **Unique Case Management:**
   - Ensures no two FIRs have the same case ID.
   - Prevents registration of duplicate cases with identical details.

---

## How to Use

### Menu Options

1. **File FIR:**
   - Enter the complainant's details, case type, and description.
   - Ensure all fields are filled. Blank fields will prevent filing.
   - Duplicate cases will not be registered.

2. **Close Case:**
   - Enter the Case ID to mark a case as solved.
   - Only pending cases can be closed.

3. **View Pending Cases:**
   - Choose to filter by civil or crime cases.
   - Displays all matching pending cases.

4. **View Solved Cases:**
   - Choose to filter by civil or crime cases.
   - Displays all matching solved cases.

5. **Exit:**
   - Exits the program.

---

## Requirements

- Python 3.6+

---

## Sample Run

1. **Main Menu:**
   ```
   Police Station Management System
   1. File FIR
   2. Close Case
   3. View Pending Cases
   4. View Solved Cases
   5. Exit
   Enter your choice:
   ```

2. **File FIR:**
   ```
   Enter Complainant Name: John Doe
   Enter Complainant Phone Number: 1234567890
   Enter Complainant Address: 123 Main Street
   Enter Case Type (civil/crime): civil
   Enter Case Description: Land dispute
   FIR filed successfully: Case ID 1
   ```

3. **Close Case:**
   ```
   Enter Case ID to close: 1
   Case ID 1 closed successfully on 2023-12-27.
   ```

4. **View Pending Cases:**
   ```
   Enter Case Type to filter (civil/crime): civil
   Case ID: 2, Complainant Name: Jane Smith, Phone: 9876543210, Address: 456 Elm Street, Type: civil, Status: pending, Close Date: N/A, Description: Property dispute
   ```

---

## Code Overview

The system is implemented with two primary classes:

1. **FIR Class:**
   - Represents a single FIR with attributes like case ID, complainant details, case type, status, and close date.
   - Contains a method to mark a case as solved.

2. **PoliceStationManagement Class:**
   - Manages all FIRs.
   - Provides methods to file FIRs, close cases, and classify cases by status or type.

---

## Author
This project was created to demonstrate efficient case management for a police station. Let me know if you have suggestions for further improvements!

