# Daily GitHub Workflow

This document defines the **standard workflow** I follow for every change in this repository.

---

## 0. Sync with main

```bash
git checkout main
git pull
````

---

## 1. Create a working branch

```bash
git checkout -b feature/<short-description>
```

**Rules**

* Never commit directly to `main`
* Branch name must describe the purpose of the change

---

## 2. Make changes

* Create / modify files
* Do not commit yet

---

## 3. Check current state

```bash
git status
```

Confirm:

* Only intended files are listed

---

## 4. Stage changes

```bash
git add <file-or-directory>
```

**Guideline**

* Stage only relevant changes
* Avoid `git add .` unless the change is trivial

---

## 5. Commit changes

```bash
git commit -m "Short, meaningful description of the change"
```

**Commit message rules**

* Describe *what* was changed
* Use present tense
* Keep it concise

---

## 6. Push branch to GitHub

```bash
git push origin feature/<short-description>
```

---

## 7. Open a Pull Request

**Pull Request Title**

* Same as commit message

**Pull Request Description**

```md
What:
- Summary of the change

Why:
- Reason for the change
```

---

## 8. Review diff and merge

* Review the diff carefully
* Confirm only intended changes are included
* Merge the Pull Request
* Delete the branch if no longer needed

---

## Core Principle

> GitHub is not just for storing code.
> It stores **intent, context, and history**.

Following this workflow ensures changes remain understandable and reversible.

