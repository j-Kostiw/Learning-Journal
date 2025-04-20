[Uploading L5DE. 3.2 Version control.pdf…]()

Streaming service company improved data engineering with:


Git + GitHub for code management and reviews

CI/CD pipelines for automation

Outcome: Better collaboration, faster algorithm updates, and more reliable data products

🔹 Learning Objectives
Understand DevOps in data engineering: collaboration, automation, monitoring

Apply Git and CI/CD for reliable data product delivery

Perform code reviews on GitHub

🔹 Version Control Basics
Tracks code changes over time

Enables rollback to previous versions ("time machine")

Types:

Local

Centralised (e.g., SVN)

Distributed (e.g., Git)

🔹 What is Git?
Free, open-source, created by Linus Torvalds in 2005

Distributed, offline-capable, fast, excellent at merging

GitHub/GitLab = cloud-based Git repositories with collaboration tools

🔹 Git vs. Dropbox/OneDrive

Task	Git Term	Description
Load/sync repo	clone	Download repository
Save changes	commit	Snapshot of file changes
Upload changes	push	Send changes to remote repo
Download changes	pull	Get updates from repo
Create copy	fork	Make your own repo copy
Merge changes	pull request	Suggest changes to be added to base repo
🔹 Interfaces & Tools
Git CLI (command line) is standard but GUIs exist:

GitHub Desktop

RStudio, PyCharm, VSCode integration

GitHub vs GitLab:

GitHub: Owned by Microsoft, massive public user base

GitLab: More storage for private repos, built-in CI/CD

🔹 Git Concepts
Three States:

Modified: Changed but not yet tracked

Staged: Marked for next commit

Committed: Snapshot saved in Git database

Use git status, git diff, git add, git commit, git push

🔹 Working with Repositories
Steps:

Create repo (GitHub)

Clone to local

Make changes

Commit & push to GitHub

Re-download if needed

Tips:

Never store Git repos inside OneDrive or another Git repo

Use semantic versioning: Major.Minor.Patch

🔹 Branching & Merging
Create a branch: git checkout -b branchname

Switch: git checkout branchname

Merge: git merge

Branching allows:

Feature isolation

Easier testing and review

Collaborative development

🔹 Conflict Resolution
When two versions edit the same part of a file, Git flags a merge conflict

You must:

Edit the file manually

Remove conflict markers (<<<<<<<, =======)

Add and commit the resolved file

🔹 Pro Tips
Use .gitignore to avoid tracking temporary or sensitive files

Use branching for collaborative or larger projects

Write meaningful commit messages

Use https://learngitbranching.js.org/ to practice:
