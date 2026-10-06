# Lab-1: Develop with AI-Powered Code Suggestions Using GitHub Copilot and VS Code

## Objective

In this lab, you will use **GitHub Copilot with Visual Studio Code** to:

- Understand an existing codebase using AI-powered explanations.
- Work with Git branches using Copilot.
- Identify and fix a bug in the application.
- Add new application data and UI functionality.
- Implement an unregister/delete feature.
- Identify and fix a frontend refresh/state-update issue.
- Plan and implement backend tests using **FastAPI + pytest**.

---

## Prerequisites

Make sure the following are installed and available:

- Visual Studio Code
- Git
- Python 3.x
- GitHub account with access to GitHub Copilot
- GitHub Copilot extension enabled in VS Code

---

# Part 1: Clone and Run the Application

## Step 1: Clone the Repository

Open a terminal in VS Code and run:

```bash
git clone https://github.com/skills/getting-started-with-github-copilot.git
```

Navigate to the project folder:

```bash
cd getting-started-with-github-copilot
```

---

## Step 2: Create a Python Virtual Environment

```bash
python -m venv .venv
```

Activate the virtual environment in PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

---

## Step 3: Install Dependencies

```bash
python -m pip install -r requirements.txt
```

---

## Step 4: Run the Application

Start the FastAPI application using Uvicorn:

```bash
python -m uvicorn src.app:app --reload
```

Keep the terminal running.

Open the application in your browser and explore the existing functionality before starting the Copilot exercises.

---

# Part 2: GitHub Copilot Exercises

> **Tip:** For each exercise, first try the prompt in the requested Copilot mode. Review Copilot's response before accepting or applying any generated changes.

---

## Prompt 1: Explore the Project (Ask Mode)

Use **GitHub Copilot Chat – Ask Mode**.

**Prompt:**

> Please briefly explain the structure of this project.

### Goal

Understand:

- Project structure
- Important files and folders
- Application entry point
- How the application is started

---

## Prompt 2: Inline Chat in Terminal (Cntrl + i --> To Activate Copilot Chat)

Use **Inline Chat in the VS Code terminal**.

**Prompt:**

> Hey Copilot, how can I create and publish a new Git branch called "accelerate-with-copilot"?

### Goal

Use Copilot to generate the Git commands required to:

1. Create the branch.
2. Switch to the branch.
3. Publish the branch to the remote repository.

Review the commands before running them.

---

## Prompt 3: Analyze a Bug Using `#codebase` (Ask Mode)

Use **Copilot Chat** with the `#codebase` context.

**Prompt:**

> #codebase Students are able to register twice for an activity.  
> Where could this bug be coming from?

### Goal

Ask Copilot to:

- Inspect the relevant code.
- Identify where duplicate registration may be occurring.
- Explain the likely root cause.
- Identify the files/functions that may need to be changed.

**Important:** Understand Copilot's explanation before modifying the code.

---

## Prompt 4: Add New Activities (In the src/app.py file --> activate Inline Chat CNTRL + i)

Use Copilot to add the following activities to the application:

- **2 sports-related activities**
- **2 artistic activities**
- **2 intellectual activities**

**Prompt:**

> Add 2 more sports related activities, 2 more artistic activities, and 2 more intellectual activities.

### Goal

Verify that:

- The new activities are added successfully.
- They appear in the correct categories.
- The existing functionality continues to work.

---

## Prompt 5: Add Participants to Activity Cards (Agent Mode)

**Prompt:**

> Hey Copilot, can you please edit the activity cards to add a participants section.  
> It will show what participants that are already signed up for that activity as a bulleted list.  
> Remember to make it pretty!

### Goal

Modify the activity cards so that each card displays:

- A **Participants** section.
- The list of registered participants.
- A clean and visually appealing layout.

### Verify

Register a participant for an activity and confirm that the participant appears in the activity card.

---

## Prompt 6: Add an Unregister/Delete Feature (Agent Mode)

Use `#codebase` context.

**Prompt:**

> #codebase Please add a delete icon next to each participant and hide the bullet points.  
> When clicked, it will unregister that participant from the activity.

### Goal

Implement the ability to:

- Remove bullet points from the participant list.
- Display a delete/unregister icon beside each participant.
- Unregister the selected participant when the icon is clicked.

### Verify

1. Register at least one participant.
2. Click the delete icon.
3. Confirm that the participant is removed from the activity.

---

## Prompt 7: Investigate the Page Refresh Bug (Agent Mode)

**Prompt:**

> I've noticed there seems to be a bug.  
> When a participant is registered, the page must be refreshed to see the change on the activity.

### Goal

Use Copilot to:

- Analyze why the UI is not updating immediately.
- Identify the frontend state/update issue.
- Implement a fix so the participant list updates without manually refreshing the page.

### Verify

1. Register a participant.
2. Do **not** refresh the page.
3. Confirm that the new participant appears immediately.

---

# Part 3: Plan and Implement Backend Tests (Plan Mode)

Now use GitHub Copilot to introduce automated backend testing.

---

## Prompt 8: Plan the Backend Tests (Plan Mode)

**Prompt:**

> Let's plan for adding backend FastAPI tests in a separate tests directory.

### Goal

Ask Copilot to propose:

- A suitable `tests` directory structure.
- Which backend components should be tested.
- Test files that should be created.
- Any required testing dependencies.
- How the tests should be executed.

Review the plan before implementing it.

---

## Prompt 9: Use the AAA Testing Pattern (Plan Mode)

**Prompt:**

> Let's use the AAA (Arrange-Act-Assert) testing pattern to structure our tests

### Goal

Ensure each test follows:

### Arrange
Set up the test data, dependencies, and expected conditions.

### Act
Execute the API call or function being tested.

### Assert
Verify that the actual result matches the expected result.

### Example Structure

```python
def test_example():
    # Arrange
    ...

    # Act
    ...

    # Assert
    ...
```

Use this structure consistently across the backend tests.

---

## Prompt 10: Add pytest (Plan Mode)

**Prompt:**

> Make sure we use `pytest` and add it to `requirements.txt` file

**Implement the Changes**

> Click on "Start Implementation" to let GitHub Copilot generate the required changes by itself.


### Goal

Ensure that:

- `pytest` is added to `requirements.txt`.
- The testing environment can install pytest.
- The backend tests are written using pytest.
- The tests can be executed successfully.

Install updated dependencies if required:

```bash
python -m pip install -r requirements.txt
```

Run the tests using:

```bash
pytest
```

---

# Final Verification Checklist

Before completing the lab, verify that:

- [ ] The application runs successfully.
- [ ] A Git branch named `accelerate-with-copilot` was created.
- [ ] The duplicate registration bug was investigated and addressed.
- [ ] 2 sports activities were added.
- [ ] 2 artistic activities were added.
- [ ] 2 intellectual activities were added.
- [ ] Activity cards display registered participants.
- [ ] Participants can be unregistered using the delete icon.
- [ ] Participant changes appear without manually refreshing the page.
- [ ] A separate `tests` directory exists.
- [ ] Backend tests follow the AAA pattern.
- [ ] `pytest` is included in `requirements.txt`.
- [ ] Backend tests execute successfully with `pytest`.

---

## Lab Outcome

By completing this lab, you will practice using GitHub Copilot in **Ask Mode, terminal Inline Chat, and codebase-aware conversations** to understand, modify, debug, and test a real application.

The key objective is not only to generate code with Copilot, but to **review, validate, and understand the AI-generated suggestions before applying them**.
