
# Xcode Project Setup

## 1. Setting Up a Brand New Project in Xcode
- Create a new Xcode project and save it in your preferred folder.

## 2. Organizing the Project
- Structure your project files as needed.
- Include a **Secrets** folder for storing sensitive data (e.g., API keys). Ensure this folder is secured and not exposed.

## 3. Add a README.md
- Create a `README.md` file for project documentation:
  
  ```bash
  touch README.md
  open README.md
  ```

## 4. Build and Run
- Build and run your project in Xcode to verify everything is working.

## 5. Add a .gitignore
- Create a `.gitignore` file to specify which files Git should ignore:
  
  ```bash
  touch .gitignore
  open .gitignore
  ```

## 6. Initialize Git and Create a GitHub Repository via Terminal

### Step 1: Initialize Git and Make Your First Commit

1. Initialize Git in your project:
   ```bash
   git init
   ```

2. Add your files and make the first commit:
   ```bash
   git add .
   git commit -m "Initial commit"
   ```

### Step 2: Create a GitHub Repository Using GitHub CLI

1. Navigate to your project directory (if you’re not already there):
   ```bash
   cd MyNewProject
   ```

2. Create a new repository on GitHub and set it as the remote:
   ```bash
   gh repo create MyNewProject --public --source=. --remote=origin
   ```

   - `--public`: Makes the repo public (use `--private` if you want a private repo).
   - `--source=.`: Uses the current directory as the source.
   - `--remote=origin`: Adds the GitHub repository as the remote.

### Step 3: Push Your Local Code to GitHub

Once the repository is created, push your local code to GitHub:

```bash
git push -u origin main
```

---

## SwiftLint Setup Guide

For detailed instructions on how to set up **SwiftLint** in Xcode, please refer to this guide:

[How to setup SwiftLint for Xcode.](https://github.com/devbyjonni/SwiftLintSetup)

---

## Setting Up Git Hooks for SwiftLint

To ensure code quality and consistency, SwiftLint can be used to lint your code before each commit. This guide explains how to set up a Git pre-commit (or pre-push) hook that runs SwiftLint, preventing commits if any lint violations are found.

[Learn how to set up Git hooks here.](https://github.com/devbyjonni/GitHooks)

---

### Version Check Commands

Use these commands to verify versions of common tools:

- Swift:
  ```bash
  swift --version
  ```

- Swift Package Manager:
  ```bash
  swift package --version
  ```

- Xcode:
  ```bash
  xcodebuild --version
  ```

- Xcode Command Line Tools:
  ```bash
  xcode-select --version
  ```
    ```bash
  xcode-select --install
  ```
  
- Homebrew:
  ```bash
  brew --version
  ```

- SwiftLint:
  ```bash
  swiftlint --version
  ```

- CocoaPods:
  ```bash
  pod --version
  ```
  
- Fastlane:
  ```bash
  fastlane --version
  ```
  
- Git:
  ```bash
  git --version
  ```

- Ruby:
  ```bash
  ruby --version
  ```
  
- Python:
  ```bash
  python --version
  ```

---
