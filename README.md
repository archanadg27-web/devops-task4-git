\# 🚀 DevOps Internship – Task 4: Version-Controlled DevOps Project with Git



\## 📌 Objective

Manage a DevOps project using Git best practices including branching, pull requests, tagging, and documentation.



\## 🛠 Tools Used

\- Git

\- GitHub



\---



\## 📁 Project Structure



```

devops-task4-git/

├── README.md          # Project documentation

├── .gitignore         # Files to be ignored by Git

├── docs/

│   └── task4-notes.md # Task notes and learning

└── scripts/

&#x20;   └── setup.sh       # Sample setup script

```



\---



\## 🌿 Branching Strategy



| Branch | Purpose |

|--------|---------|

| `main` | Production-ready code |

| `dev` | Development integration branch |

| `feature/add-readme` | Feature branch for README addition |

| `feature/add-gitignore` | Feature branch for .gitignore |



\---



\## 🔄 Git Workflow Followed



\### 1. Initialize Repository

```bash

git init

git remote add origin https://github.com/YOUR\_USERNAME/devops-task4-git.git

```



\### 2. Create Branches

```bash

\# Create and switch to dev branch

git checkout -b dev



\# Create a feature branch from dev

git checkout -b feature/add-readme

```



\### 3. Make Changes and Commit

```bash

git add .

git commit -m "feat: add README.md with project documentation"

```



\### 4. Push and Create Pull Request

```bash

git push origin feature/add-readme

\# Then open a Pull Request on GitHub: feature/add-readme → dev

```



\### 5. Merge dev into main

```bash

\# After review, merge dev into main via Pull Request on GitHub

git checkout main

git merge dev

git push origin main

```



\### 6. Tag the Release

```bash

git tag -a v1.0 -m "Initial release - Task 4 complete"

git push origin v1.0

```



\---



\## 🏷️ Tags

\- `v1.0` – Initial release with complete Git workflow demonstration



\---



\## 📝 Interview Q\&A



\*\*1. What is Git?\*\*  

Git is a distributed version control system that tracks changes in source code, allowing multiple developers to collaborate efficiently.



\*\*2. What is the difference between merge and rebase?\*\*  

\- `git merge` combines two branches and creates a new merge commit, preserving history.  

\- `git rebase` moves or replays commits on top of another branch, creating a linear history.



\*\*3. What is a pull request?\*\*  

A pull request (PR) is a GitHub feature that lets you notify team members of changes in a branch, request code review, and merge changes into another branch.



\*\*4. How do you resolve merge conflicts?\*\*  

Open the conflicting file, look for `<<<<<<<`, `=======`, and `>>>>>>>` markers, manually edit to keep the correct code, then run `git add` and `git commit`.



\*\*5. What are Git tags?\*\*  

Tags are references to specific points in Git history, typically used to mark release versions (e.g., `v1.0`, `v2.0`).



\*\*6. What is Git workflow?\*\*  

A Git workflow is a set of branching and merging guidelines. Common ones include Git Flow, GitHub Flow, and Trunk-Based Development.



\*\*7. Explain git stash.\*\*  

`git stash` temporarily saves your uncommitted changes so you can switch branches or pull updates, and later restore them with `git stash pop`.



\*\*8. What is the use of .gitignore?\*\*  

`.gitignore` tells Git which files or directories to skip tracking — such as log files, secrets, build artifacts, and OS-specific files.



\---



\## ✅ Deliverables Checklist



\- \[x] Initialized Git repository

\- \[x] Pushed to GitHub

\- \[x] Created `main`, `dev`, and `feature` branches

\- \[x] Used pull requests to merge branches

\- \[x] Added `.gitignore`

\- \[x] Added proper `README.md`

\- \[x] Tagged release as `v1.0`

\- \[x] Documented all steps in Markdown



\---



\## 👤 Author

\*\*\[Your Name]\*\*  

DevOps Internship – ElevateLabs  

April 2026



