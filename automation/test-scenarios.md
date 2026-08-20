# MakeMyTrip — Puppeteer Automation Test Scenarios

## 1. Purpose

This document defines the planned automated test scenarios for the MakeMyTrip web application using Puppeteer.

The scenarios focus on critical travel-search workflows, functional validation, positive and negative testing, and regression coverage.

---

## 2. Automation Scenario Matrix

| Scenario ID  | Scenario                                      | Test Type  | Priority | Automation |
| ------------ | --------------------------------------------- | ---------- | -------- | ---------- |
| MMT-AUTO-001 | Verify MakeMyTrip homepage loads successfully | Smoke      | High     | Puppeteer  |
| MMT-AUTO-002 | Verify flight search interface is available   | Functional | High     | Puppeteer  |
| MMT-AUTO-003 | Select valid departure location               | Functional | High     | Puppeteer  |
| MMT-AUTO-004 | Select valid destination location             | Functional | High     | Puppeteer  |
| MMT-AUTO-005 | Select valid future travel date               | Functional | High     | Puppeteer  |
| MMT-AUTO-006 | Select passenger information                  | Functional | Medium   | Puppeteer  |
| MMT-AUTO-007 | Search flights using valid criteria           | End-to-End | Critical | Puppeteer  |
| MMT-AUTO-008 | Validate flight search results                | Functional | High     | Puppeteer  |
| MMT-AUTO-009 | Validate flight information                   | Functional | High     | Puppeteer  |
| MMT-AUTO-010 | Apply available flight filter                 | Functional | Medium   | Puppeteer  |
| MMT-AUTO-011 | Change flight filter                          | Functional | Medium   | Puppeteer  |
| MMT-AUTO-012 | Apply available sorting option                | Functional | Medium   | Puppeteer  |
| MMT-AUTO-013 | Change sorting option                         | Functional | Medium   | Puppeteer  |
| MMT-AUTO-014 | Open flight details                           | Functional | High     | Puppeteer  |
| MMT-AUTO-015 | Validate flight details                       | Functional | High     | Puppeteer  |
| MMT-AUTO-016 | Validate missing source                       | Negative   | High     | Puppeteer  |
| MMT-AUTO-017 | Validate missing destination                  | Negative   | High     | Puppeteer  |
| MMT-AUTO-018 | Validate missing travel date                  | Negative   | Medium   | Puppeteer  |
| MMT-AUTO-019 | Validate invalid search conditions            | Negative   | Medium   | Puppeteer  |
| MMT-AUTO-020 | Execute critical flight-search workflow       | End-to-End | Critical | Puppeteer  |

---

## 3. Homepage Scenarios

### MMT-AUTO-001 — Homepage Load

**Objective:** Verify that the MakeMyTrip homepage loads successfully.

**Expected Result:** The homepage loads without critical errors and the flight-search interface is available.

### MMT-AUTO-002 — Flight Search Interface

**Objective:** Verify that the flight-search controls are available.

**Expected Result:** The required search controls are displayed and available for interaction.

---

## 4. Location Scenarios

### MMT-AUTO-003 — Departure Location

**Objective:** Select a valid departure location.

**Expected Result:** The selected departure location is displayed correctly.

### MMT-AUTO-004 — Destination Location

**Objective:** Select a valid destination location.

**Expected Result:** The selected destination location is displayed correctly.

---

## 5. Date and Passenger Scenarios

### MMT-AUTO-005 — Travel Date

**Objective:** Select a valid future travel date.

**Expected Result:** The selected travel date is displayed correctly.

### MMT-AUTO-006 — Passenger Selection

**Objective:** Select passenger information.

**Expected Result:** The selected passenger count is reflected correctly in the search criteria.

---

## 6. Search Scenarios

### MMT-AUTO-007 — Flight Search

**Objective:** Search for flights using valid criteria.

**Flow:**

1. Open MakeMyTrip.
2. Open flight search.
3. Select departure location.
4. Select destination location.
5. Select travel date.
6. Select passenger information.
7. Submit the search.

**Expected Result:** Flight search results are displayed.

### MMT-AUTO-008 — Search Results

**Objective:** Validate that search results are displayed.

**Expected Result:** Available flight results are displayed according to the selected search criteria.

### MMT-AUTO-009 — Flight Information

**Objective:** Validate important flight information.

**Expected Result:** Relevant information such as airline, timing, route, and price is displayed where provided.

---

## 7. Filter Scenarios

### MMT-AUTO-010 — Apply Filter

**Objective:** Apply an available flight filter.

**Expected Result:** Search results are filtered according to the selected criteria.

### MMT-AUTO-011 — Change Filter

**Objective:** Modify an applied filter.

**Expected Result:** Search results update according to the changed criteria.

---

## 8. Sorting Scenarios

### MMT-AUTO-012 — Apply Sorting

**Objective:** Apply an available sorting option.

**Expected Result:** Search results are reordered according to the selected option.

### MMT-AUTO-013 — Change Sorting

**Objective:** Change the selected sorting option.

**Expected Result:** Results update according to the new sorting criteria.

---

## 9. Flight Details

### MMT-AUTO-014 — Open Flight Details

**Objective:** Open the details of a selected flight.

**Expected Result:** The selected flight details are displayed.

### MMT-AUTO-015 — Validate Flight Details

**Objective:** Validate information displayed for a selected flight.

**Expected Result:** Relevant flight details are displayed consistently with the selected search result.

---

## 10. Negative Scenarios

### MMT-AUTO-016 — Missing Source

**Objective:** Attempt to search without selecting a departure location.

**Expected Result:** The application should prevent an invalid search and provide appropriate validation.

### MMT-AUTO-017 — Missing Destination

**Objective:** Attempt to search without selecting a destination.

**Expected Result:** The application should prevent an invalid search and provide appropriate validation.

### MMT-AUTO-018 — Missing Travel Date

**Objective:** Attempt to search without selecting the required travel date.

**Expected Result:** Appropriate validation should be displayed.

### MMT-AUTO-019 — Invalid Search Conditions

**Objective:** Validate handling of invalid or unsupported search combinations.

**Expected Result:** The application should handle the condition appropriately.

---

## 11. End-to-End Scenario

### MMT-AUTO-020 — Critical Flight Search Workflow

**Objective:** Validate the primary flight-search workflow.

**Flow:**

1. Open MakeMyTrip.
2. Select flight search.
3. Enter departure location.
4. Enter destination location.
5. Select travel date.
6. Select passenger information.
7. Search for flights.
8. Validate search results.
9. Apply an available filter.
10. Apply an available sorting option.
11. Open a flight's details.
12. Validate the displayed information.

**Expected Result:** The complete workflow behaves according to the application's expected behavior.

---

## 12. Regression Automation

High-value regression scenarios include:

* Homepage loading
* Flight search
* Location selection
* Date selection
* Passenger selection
* Search results
* Filtering
* Sorting
* Flight details
* Critical search workflow

---

## 13. Automation Design Notes

The Puppeteer implementation should use:

* Stable selectors
* Reusable functions
* Appropriate synchronization
* Assertions
* Independent scenarios
* Test data separation
* Clear naming
* Failure diagnostics

---

## 14. GitHub Copilot Assistance

GitHub Copilot may assist with:

* Puppeteer test implementation
* Selector suggestions
* Assertion development
* Test data generation
* Refactoring
* Error handling
* Debugging
* Test documentation

AI-generated output should be reviewed and validated before use.

---

## 15. Project Status

These scenarios represent the planned Puppeteer automation coverage for the personal MakeMyTrip QA portfolio project.

Executable automation scripts will be added separately when the implementation is available.
