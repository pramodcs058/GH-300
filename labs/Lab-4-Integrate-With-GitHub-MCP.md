# 🧪 Lab - 4 : Integrating MCP with GitHub Copilot

## 🎯 Lab Objective

In this lab, you will learn how to enhance GitHub Copilot capabilities by integrating **Model Context Protocol (MCP)**. By the end of this lab, you will be able to:

* Configure an MCP server
* Use Copilot in Agent Mode
* Perform GitHub operations (issues, PRs) using AI
* Validate AI-generated code

---

## 📋 Prerequisites

Before starting, ensure you have:

* GitHub account
* Access to GitHub Codespaces
* GitHub Copilot enabled
* Basic understanding of GitHub repositories

---

## 🧩 Lab Overview

This lab consists of 4 major steps:

1. Environment Setup & MCP Introduction
2. MCP Server Integration
3. Using MCP with Copilot Agent Mode
4. Validating AI-generated Code

---

# 🚀 Step 1: Environment Setup & Introduction

## 📖 What is MCP?

Model Context Protocol (MCP) acts as a **universal connector for AI tools**, enabling GitHub Copilot to interact with external systems like GitHub.

---

## 🛠️ Task 1: Setup Development Environment

1. Clone the repo **https://github.com/skills/integrate-mcp-with-copilot/**
2. Open the this repository in **GitHub Codespaces**
3. Use default configuration to create the Codespace
4. Once loaded:

   * Verify Copilot Chat is available
   * Ensure Python extension is installed

---

## ▶️ Task 2: Run the Application

1. Navigate to **Run and Debug** panel
2. Click **Start Debugging**
3. Open the **Ports tab**
4. Launch the application in browser
5. Verify the application is running successfully

✅ Expected Outcome: Application loads successfully in browser

---

# 🔌 Step 2: Add GitHub MCP Server

## 🛠️ Task 3: Enable Agent Mode

1. Open Copilot Chat panel
2. Ensure **Agent Mode** is selected

---

## 🛠️ Task 4: Configure MCP Server

1. Navigate to `.vscode` folder

2. Create a new file:

   ```
   mcp.json
   ```

3. Add the following configuration:

```json
{
  "servers": {
    "github": {
      "type": "http",
      "url": "https://api.githubcopilot.com/mcp/"
    }
  }
}
```

---

## 🛠️ Task 5: Activate MCP Server

1. Click **Start** button inside `mcp.json`
2. Authenticate with GitHub when prompted
3. Open Copilot panel
4. Click the 🛠️ icon to view available tools

---

## 🛠️ Task 6: Commit Changes

1. Commit the `.vscode/mcp.json` file
2. Push changes to `main` branch

⚠️ Note: Direct push to main is only for lab simplicity

---

✅ Expected Outcome:

* MCP server connected
* Copilot shows additional capabilities

---

# 🤖 Step 3: Using MCP with Copilot (Agent Mode)

## 📖 Concept: Tool Calling

Copilot can:

* Discover tools
* Select appropriate tools
* Execute actions (e.g., create issue, PR)

---

## 🛠️ Task 7: Explore GitHub Projects

1. Open Copilot Chat (Agent Mode)
2. Use the following prompt:

```
Search for repositories similar to this project
```

3. Approve tool usage when prompted

---

## 🛠️ Task 8: Analyze a Project

Prompt:

```
Describe features of one selected project in detail
```

---

## 🛠️ Task 9: Compare Features

Prompt:

```
Compare these features with our project. Identify new ideas
```

---

## 🛠️ Task 10: Create Issues Using Copilot

Prompt:

```
Create GitHub issues for the identified improvements
```

1. Approve each action
2. Verify issues created in repository

---

## 🛠️ Task 11: Reset Context

1. Click **New Chat** in Copilot panel

---

✅ Expected Outcome:

* New issues created using Copilot
* Demonstrates MCP tool integration

---

# 🛠️ Step 4: Solve Issues Using MCP

## 🛠️ Task 12: Analyze Issues

Prompt:

```
How many open issues are there in my repository?
```

---

## 🛠️ Task 13: Prioritize Issues

Prompt:

```
Review all issues and suggest top 3 most important ones
```

---

## 🛠️ Task 14: Implement an Issue

Prompt:

```
#codebase Implement the top issue:
1. Create a new branch
2. Make required changes
3. Show changes before pushing
4. Create a pull request
```

1. Approve tool actions
2. Verify PR is created

---

✅ Expected Outcome:

* Code changes implemented
* Pull request created using Copilot

---

# 🔍 Step 5: Validate AI-Generated Code

## 🛠️ Task 15: Review Pull Request

1. Open the PR in GitHub
2. Review changes carefully
3. Merge PR if valid

---

## 🛠️ Task 16: Add Closing Comment

Prompt:

```
Add a closing comment to the issue with a summary and thank contributors
```

---

✅ Expected Outcome:

* PR reviewed and merged
* Issue updated with closing comment

---

# 🎉 Lab Completion

Congratulations! You have successfully:

* Integrated MCP with GitHub Copilot
* Used Agent Mode for real-world workflows
* Automated issue management and development tasks
* Validated AI-generated code

---

# 🧠 Key Takeaways

* MCP extends Copilot beyond code generation
* Agent Mode enables real automation
* Always validate AI-generated changes
* MCP + Copilot = End-to-End Developer Assistant

---

# ⚠️ Best Practices

* Always review tool actions before approval
* Avoid blind execution of AI suggestions
* Use MCP responsibly in production environments
* Combine MCP with instruction sets for better results

---

# 🚀 Bonus Challenges

* Add another MCP server (e.g., Slack, Figma)
* Automate full feature implementation using Copilot
* Integrate testing pipeline using GitHub Actions

---

Happy Coding! 💡
