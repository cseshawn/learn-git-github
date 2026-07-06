# GitHub Fork — Simple Notes

## What is a Fork?

A **fork** is your own copy of someone else's GitHub repository.

### Example

Original repository:

```text
github.com/john/calculator
```

After clicking **Fork**, GitHub creates:

```text
github.com/shawn/calculator
```

Now there are two repositories:

```text
github.com/john/calculator     ← Original repository
github.com/shawn/calculator    ← Your fork
```

You can make changes in your fork without affecting the original repository.

---

## Why Fork?

- Contribute to open-source projects
- Fix bugs
- Add new features
- Experiment safely
- Learn from existing projects

---

## Fork Workflow

```text
github.com/john/calculator
            │
            ▼
          Fork
            │
            ▼
github.com/shawn/calculator
            │
            ▼
          Clone
            │
            ▼
      Make Changes
            │
            ▼
           Push
            │
            ▼
github.com/shawn/calculator
            │
            ▼
      Pull Request
            │
            ▼
github.com/john/calculator
```

---

## Clone Your Fork

```bash
git clone https://github.com/shawn/calculator.git
cd calculator
```

---

## Remote Repositories

Git usually uses two remotes:

```text
origin   = github.com/shawn/calculator
upstream = github.com/john/calculator
```

Example:

```bash
git remote -v
```

Output:

```text
origin   https://github.com/shawn/calculator.git
upstream https://github.com/john/calculator.git
```

### Meaning

| Remote   | Repository                              |
| -------- | --------------------------------------- |
| origin   | Your fork (`shawn/calculator`)          |
| upstream | Original repository (`john/calculator`) |

Memory Trick:

```text
origin   = My repository
upstream = Original repository
```

---

## Make Changes and Push

```bash
git add .
git commit -m "Added scientific calculator feature"
git push origin main
```

Changes are uploaded to:

```text
github.com/shawn/calculator
```

---

## What is a Pull Request?

A **Pull Request (PR)** is a request to merge your changes into the original repository.

```text
From:
github.com/shawn/calculator

To:
github.com/john/calculator
```

Example:

Original code:

```python
print("Calculator")
```

Your fork:

```python
print("Calculator")
print("Scientific Mode Added")
```

Create a Pull Request and ask John:

```text
Please merge my changes from
github.com/shawn/calculator

into

github.com/john/calculator
```

If John approves, your changes become part of the original repository.

---

## Quick Summary

```text
Fork  = Copy repository on GitHub
Clone = Download repository to your computer

origin   = github.com/shawn/calculator
upstream = github.com/john/calculator

Push → origin
Pull Request → upstream
```
