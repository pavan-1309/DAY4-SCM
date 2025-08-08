# DAY4_Git_Branching
DevOps Project – Git Best Practices

Objective
This project demonstrates managing a DevOps project using **Git best practices**, including branch management, pull requests, tagging, and proper commit history.
"I have added images to the images/ folder. Please open the folder to view them."

---

Tools Used
- **Git** – Version control
- **GitHub** – Remote repository hosting
- **Docker** – Containerization

**Git Workflow Followed**

Repository Initialization
- Initialized a local Git repository:
  
  git init
  
- Added GitHub remote:
  
  git remote add origin git@github.com:pavan-1309/DAY4-SCM.git
  
- First commit and push:
 
  git add .
  git commit -m "Initial commit"
  git push -u origin main
  

---

Branching Strategy
We used a **two-branch workflow**:
- **`main`** – Stable production-ready code.
- **`dev`** – Development and testing branch.

**Commands Used:**

# Create and switch to dev branch
git checkout -b dev


---

Feature Implementation in `dev`
- Created a **Dockerfile** in the `dev` branch.
- Commit message used:
  
  Created Dockerfile
  
- Pushed the changes to the remote `dev` branch.

---

Pull Request & Merge
- Created a **Pull Request** (PR) from `dev` → `main`.
- Merged PR after review.
- This ensured the `main` branch always contains tested, stable code.

---

Syncing Local `main` with Remote
After merging PR:

git checkout main
git pull origin main

---

Version Tagging
- Created a **Git tag** for the release:

git tag -a V1.0 -m "Release Version 1.0"
git push origin V1.0


---
