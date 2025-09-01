# Test Cases and Requirement Traceability Matrix (RTM)

## User Story: US1.2 - Search for a Round-Trip Flight

### Test Cases

| Test Case ID | Title | Test Steps | Expected Results | Priority | Test Type | Automation Status |
|--------------|-------|------------|------------------|----------|-----------|-------------------|
| TC1 | Validate 'From' field dropdown | Open the dropdown and check if it contains the cities: New York, London, Tokyo, Paris, Sydney, Mumbai, Delhi, Dubai, Singapore. | Dropdown should display the listed cities. | High | Positive | Automatable |
| TC2 | Validate 'To' field dropdown | Open the dropdown and check if it contains the cities: New York, London, Tokyo, Paris, Sydney, Mumbai, Delhi, Dubai, Singapore. | Dropdown should display the listed cities. | High | Positive | Automatable |
| TC3 | Validate 'From' field mandatory check | Leave the 'From' field blank and click the 'Search' button. | Error message "Please select a departure city." should be displayed. | High | Negative | Automatable |
| TC4 | Validate 'To' field mandatory check | Leave the 'To' field blank and click the 'Search' button. | Error message "Please select a destination city." should be displayed. | High | Negative | Automatable |
| TC5 | Validate 'From' and 'To' cannot be same | Select the same city in both 'From' and 'To' fields and click the 'Search' button. | Error message "Departure and destination cannot be the same." should be displayed. | High | Negative | Automatable |
| TC6 | Validate past dates in 'Departure Date' | Attempt to select a past date in the 'Departure Date' calendar picker. | Past dates should be disabled and not selectable. | High | Negative | Automatable |
| TC7 | Validate 'Departure Date' mandatory check | Leave the 'Departure Date' field blank and click the 'Search' button. | Error message "Please select a departure date." should be displayed. | High | Negative | Automatable |
| TC8 | Validate 'Return Date' mandatory check | Leave the 'Return Date' field blank and click the 'Search' button. | Error message "Please select a return date." should be displayed. | High | Negative | Automatable |
| TC9 | Validate 'Return Date' after Departure | Select a 'Return Date' that is before or the same as the 'Departure Date' and click the 'Search' button. | Error message "Return date must be after departure date." should be displayed. | High | Negative | Automatable |
| TC10 | Validate 'Passengers' field boundaries | Enter a value less than 1 or greater than 9 in the 'Passengers' field and click the 'Search' button. | Error message "Please enter between 1 and 9 passengers." should be displayed. | High | Negative | Automatable |

### Requirement Traceability Matrix (RTM)

| User Story ID | User Story Name | Acceptance Criteria | Test Case ID | Test Case Title | Priority | Execution Status | Defect ID(s) | Remarks / Gaps |
|---------------|-----------------|---------------------|--------------|-----------------|----------|------------------|---------------|----------------|
| US1.2 | Search for a Round-Trip Flight | AC1: From & To: Same rules as US1.1 (mandatory, not same, errors). | TC1 | Validate 'From' field dropdown | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC2 | Validate 'To' field dropdown | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC3 | Validate 'From' field mandatory check | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC4 | Validate 'To' field mandatory check | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC5 | Validate 'From' and 'To' cannot be same | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight | AC2: Departure Date: Same rules as US1.1 (mandatory, not in past). | TC6 | Validate past dates in 'Departure Date' | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC7 | Validate 'Departure Date' mandatory check | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight | AC3: Return Date: Visible if 'One Way' unchecked. Calendar/manual entry in dd-mm-yyyy. Mandatory. Error if blank → 'Please select a return date.' If ≤ departure date → 'Return date must be after departure date.' | TC8 | Validate 'Return Date' mandatory check | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC9 | Validate 'Return Date' after Departure | High | Not Executed | - | - |
| US1.2 | Search for a Round-Trip Flight |  | TC15 | Validate 'One Way' checkbox functionality | Medium | Not Executed | - | - |
