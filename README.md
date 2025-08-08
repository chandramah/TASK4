# Task 4 - Version Controlled DevOps Project 
 

## Usage 
Instructions on how to clone and run the project. 

## Objective
Manage a DevOps project using Git best practices — including branching, pull requests, conflict resolution, tags, and documentation.

---

## Branching Workflow
- **main** → Stable production-ready branch  
- **dev** → Integration/testing branch  
- **feature/** → Individual features or fixes

---

## Steps Completed

1. **Repo Setup**
   - Initialized local Git repo
   - Added `.gitignore`, `README.md`, `sample.txt`
   - Linked to GitHub repository

2. **Branching**
   - Created `dev` branch from `main`
   - Created `feature/add-usage-section` from `dev`

3. **Development**
   - Added "Usage" section to `README.md` in feature branch
   - Committed and pushed to GitHub

4. **Pull Requests**
   - Merged `feature/add-usage-section` → `dev`
   - Resolved conflict when merging `dev` → `main`

5. **Tagging**
   - Created annotated tag `v1.0` for initial stable release

---

## Commands Used
```bash
git init
git add .
git commit -m "chore: initial commit"
git branch -M main
git remote add origin <repo_url>
git push -u origin main

git checkout -b dev
git push -u origin dev

git checkout -b feature/add-usage-section
# make changes
git add .
git commit -m "feat: add Usage section to README"
git push -u origin feature/add-usage-section

# Merge via Pull Requests on GitHub

git checkout main
git pull origin main
git tag -a v1.0 -m "Task 4 - initial stable release"
git push origin v1.0


