# 🤖 Learning GitHub Actions – PR Greeting Workflow

This repository was created while **learning GitHub Actions**.  
The goal of this project is to understand how workflows work by automating a simple task:  
**posting a comment when a pull request is raised**.

---

## 📚 What I Was Learning

- Basics of GitHub Actions
- Workflow file structure (YAML)
- Event triggers in GitHub
- Job and step execution
- Using third-party GitHub Actions
- Handling permissions and tokens

---

## ⚙️ Workflow Details

- **Workflow Name:** PR-Greeting
- **Trigger Event:** `pull_request_target`
- **Runner:** ubuntu-latest
- **Action Used:** `thollander/actions-comment-pull-request@v1`
- **Comment Message:** `PR Raised`

---

## 🧠 How the Workflow Works

1. A pull request is created.
2. GitHub triggers the workflow.
3. The workflow runs on an Ubuntu runner.
4. A comment is automatically added to the pull request using the GitHub token.

---

## 🔐 Permissions

```yaml
permissions:
  pull-requests: write
