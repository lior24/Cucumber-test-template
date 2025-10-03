---
description: Create base Cucumber test file structure.
---

## Guidance
- Do NOT include explanatory text in the AI chat response
- Only ask clarifying questions if essential details are missing
- Write "done" when the task is completed

## Instructions
When asked to create a base Cucumber test file structure, follow these steps:

1. **File Creation**: If the target file does not exist, create it with the `Template Structure` below
2. **Filename Replacement**: Replace all instances of `replace with filename` with the actual filename (including extension)
3. **TODO Placeholders**: Leave TODO markers for the user to complete
   

## Template Structure

```cucumber
##########################################################################
# Header
# -------------------------------------------------------------------------
# - Test code: replace with filename
# - Description: <TODO: add description>
# - Jira: <TODO: add Jira id>
###########################################################################
@SUPERVISOR_X3
@SUPERVISOR_WH
Feature: replace with filename

    Scenario: Log in
        Given the user is logged into Sage X3 with "param:loginType" using user name "param:loginUserRootName" and password "param:loginUserRootPassword"
        When the user selects the "param:endPointName1" entry on endpoint panel
        Then the "param:endPointName1" endpoint is selected
        When the user changes the main language code to "en-US"

    replace with test scenarios

    Scenario: Log out
        Then the user logs-out from the system
```
