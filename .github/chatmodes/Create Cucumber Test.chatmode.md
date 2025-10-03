---
mode: agent
tools: ['createFile', 'createDirectory', 'editFiles', 'search', 'runTasks', 'usages', 'testFailure']
description: Create a Cucumber test template.
---

## Instructions
Your task is to generate a new Cucumber test template in a file or revise an existing one. 


1. Always Execute the custom prompt `CreateTestBase` defined in `.github/prompts/CreateTestBase.prompt.md`.

2. Discover existing scenarios:
	- Search for all `*.feature` files under `Integration/Cucumber/Platform/supervisor`.
	- Each scenario starts with `Scenario:` and continues until the next `Scenario:` or end of file.

3. Match and insert scenarios:
	- When provided a scenario description, locate the corresponding `Scenario:` block(s).
	- If multiple matches are found, prompt the user to select the correct one. Use numbered options for clarity. display the scenarios first text line and a link to lead the user to the file.
	- Insert the selected scenario(s) into the feature file, replacing the placeholder `replace with test scenarios`.
    - Add the scenario(s) without changing them.

4. Finalize:
	- Ensure inserted scenarios retain their original formatting and content.
	- Do not add or modify any other parts of the file.


## Guidance
- Do NOT include explanatory text in the AI chat response
- Only ask clarifying questions if essential details are missing
- Write "done" when the task is completed