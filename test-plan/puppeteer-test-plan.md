# MakeMyTrip — Puppeteer Automation Test Plan

## 1. Objective

The objective of this project is to demonstrate web application test automation using Puppeteer while validating key MakeMyTrip travel-search workflows.

The automation approach focuses on browser automation, functional validation, reusable test components, regression coverage, and maintainable test design.

---

## 2. Automation Scope

The planned automation coverage includes:

* Homepage validation
* Flight search
* Source selection
* Destination selection
* Travel date selection
* Passenger selection
* Search results
* Flight filtering
* Flight sorting
* Flight details
* Navigation validation

---

## 3. Automation Framework

**Automation Tool:** Puppeteer

### Supporting Technologies

The automation environment may include:

* JavaScript
* Node.js
* Puppeteer
* Git
* GitHub
* GitHub Copilot

---

## 4. Automation Approach

The automation suite should follow maintainable practices including:

* Stable selectors
* Reusable functions
* Appropriate waits
* Assertions
* Independent test scenarios
* Test data separation
* Clear test naming
* Error handling
* Failure diagnostics

---

## 5. Page / Component Organization

Reusable page or component abstractions can be used to separate browser interaction logic from test scenarios.

Example conceptual structure:

```text id="7h4j3s"
pages/
├── home.page.js
├── flight-search.page.js
├── search-results.page.js
└── flight-details.page.js
```

This improves:

* Maintainability
* Reusability
* Readability
* Selector management
* Test maintenance

---

## 6. Flight Search Scenarios

### Source Selection

* Enter a valid departure location.
* Select the appropriate source suggestion.
* Validate the selected source.

### Destination Selection

* Enter a valid destination.
* Select the appropriate destination suggestion.
* Validate the selected destination.

### Travel Date

* Select a valid future travel date.
* Validate the selected date.
* Validate invalid or unavailable date conditions where applicable.

### Passenger Selection

* Select the required passenger count.
* Validate passenger information.

### Flight Search

* Execute a search using valid travel details.
* Validate that search results are displayed.

---

## 7. Search Result Scenarios

* Validate search result availability.
* Validate flight information.
* Apply available filters.
* Modify filters.
* Apply available sorting options.
* Change sorting options.
* Open flight details.

---

## 8. Positive Testing

Examples include:

* Valid source and destination
* Valid future travel date
* Valid passenger selection
* Valid search criteria
* Valid filter selection
* Valid sorting selection

---

## 9. Negative Testing

Examples include:

* Missing source
* Missing destination
* Missing travel date
* Invalid search combinations
* Invalid passenger values
* Unsupported selections
* Unexpected navigation states

---

## 10. Test Data

Test data may include:

* Departure locations
* Destination locations
* Travel dates
* Passenger counts
* Search criteria
* Filter combinations
* Sorting options

No confidential customer information should be used.

---

## 11. Browser Automation

Puppeteer primarily automates Chromium-based browser environments.

The automation suite should validate behavior consistently across the configured browser environment.

---

## 12. Assertions

Assertions should validate important application behavior, including:

* Page title
* URL/navigation state
* Element visibility
* Selected locations
* Selected travel date
* Search results
* Filter state
* Sorting behavior
* Flight details

---

## 13. Regression Strategy

The automated regression suite should prioritize:

1. Homepage loading
2. Source selection
3. Destination selection
4. Travel date
5. Passenger selection
6. Flight search
7. Search result validation
8. Filtering
9. Sorting
10. Flight details

---

## 14. GitHub Copilot Assistance

GitHub Copilot may assist with:

* Puppeteer script development
* Selector suggestions
* Test scenario implementation
* Assertion suggestions
* Error handling
* Refactoring
* Test data generation
* Documentation
* Debugging assistance

All generated suggestions must be reviewed, executed, and validated by the tester.

---

## 15. Failure Analysis

Automation failures should be analyzed to determine whether the cause is:

* Application behavior
* Selector failure
* Synchronization issue
* Test-data issue
* Environment issue
* Browser issue
* Automation implementation issue

Only verified application failures should be documented as defects.

---

## 16. Entry Criteria

Automation execution can begin when:

* The application is accessible.
* Node.js is available.
* Puppeteer is configured.
* Required test data is available.
* Automation scenarios are defined.

---

## 17. Exit Criteria

Automation execution may be considered complete when:

* Planned scenarios have been executed.
* Critical workflows have been validated.
* Failed tests have been analyzed.
* Valid defects have been documented.
* Regression scenarios have been completed.
* Test results have been reviewed.

---

## 18. Project Status

**Status:** Puppeteer automation portfolio project developed incrementally.

This repository documents the planned Puppeteer automation approach. Executable automation source files will be added when the corresponding implementation is available.

---

## 19. Disclaimer

This is an independent personal QA portfolio project created for learning, practice, and demonstration of Puppeteer automation and software testing skills.

It does not contain confidential information, proprietary data, or materials belonging to any previous employer or client.
