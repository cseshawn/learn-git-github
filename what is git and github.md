# Git vs GitHub - Quick Guide

## What is Git?

**Git** is a **Version Control System (VCS)** that tracks changes in your code locally on your computer.

### Key Features:

- Tracks every modification in your project
- Allows you to go back to any previous version
- Works offline on your machine
- Creates different branches for features
- Free and open source

### Common Git Commands:

```bash
git init              # Start tracking a project
git add .             # Stage changes
git commit -m "msg"   # Save changes locally
git branch            # Create separate development lines
git merge             # Combine branches
git log               # View change history
```

---

## What is GitHub?

**GitHub** is a **cloud-based platform** that hosts Git repositories online and enables team collaboration.

### Key Features:

- Stores your Git repositories in the cloud
- Enables multiple developers to work together
- Provides Pull Requests for code review
- Offers Issue tracking and project management
- Hosts free public repositories
- Includes CI/CD with GitHub Actions

### Common GitHub Operations:

```bash
git push              # Upload local commits to GitHub
git pull              # Download changes from GitHub
git clone             # Copy a repository from GitHub
```

---

## Git vs GitHub - Quick Comparison

| **Git**                    | **GitHub**                        |
| -------------------------- | --------------------------------- |
| Installed on your computer | Website/Cloud service             |
| Works offline              | Requires internet                 |
| Manages version history    | Hosts repositories online         |
| Command-line tool          | Visual interface + Git commands   |
| Free software              | Free for public, paid for private |
| Individual use             | Team collaboration                |

---

## Practical Applications

### When to Use Git:

- Tracking personal projects
- Working offline
- Managing your own code versions
- Creating local backups

### When to Use GitHub:

- Sharing code with team
- Open source contributions
- Collaborating with developers
- Deploying applications
- Code review and quality control

---

## Workflow Example

```bash
# Local Work (Git)
git init
git add .
git commit -m "first commit"

# Push to Cloud (GitHub)
git remote add origin https://github.com/username/repo.git
git push -u origin main

# Team Collaboration
git pull origin main        # Get latest changes
git checkout -b new-feature # Create branch
git add .
git commit -m "new feature"
git push origin new-feature # Push to GitHub
# Create Pull Request on GitHub website
```

---

## Summary

- **Git** = Local version control tool on your computer
- **GitHub** = Cloud platform to host Git repositories and collaborate
- Together they enable powerful version control + team collaboration
