# Instructions for Agentic AI Primer Lab
1.	Go to https://console.groq.com/keys , Create an API KEY 
2.	Go to https://openrouter.ai/, Create an API KEY
3.	Copy the keys & them safely, you may see it only once while creating.
# Student Workflow: Fork → Modify → Push
Step 1: Fork the Repository on GitHub
1.	Go to the repository: https://github.com/svhari/AAI_primer
2.	Click the "Fork" button (top right corner) &  Star it.
3.	This creates a copy under your GitHub account: https://github.com/your-username/AAI_primer
________________________________________
Step 2: Clone Your Fork Locally
bash
# Clone YOUR fork (not the original)
git clone https://github.com/your-username/AAI_primer.git
cd AAI_primer
________________________________________
Step 3: Complete Your Lab Work
bash
# Create a new branch for your lab work
git checkout -b lab-work

Make your changes
Edit files, add new files, etc.

# Check what's changed
git status
________________________________________
Step 4: Commit Your Changes
bash
# Stage all changes
git add .

# Commit with a message
git commit -m "Complete lab assignment"
________________________________________
Step 5: Push to Your Fork
bash
# Push to YOUR fork (not the original)
git push origin lab-work


# Common Scenarios and Solutions**
Scenario 1: Student modifies main branch directly
bash
# If they accidentally worked on main
git checkout main
git add .
git commit -m "My changes"
git push origin main  # Pushes to THEIR fork's main
Scenario 2: Student wants to switch branches
bash
# Switch to existing branch
git checkout existing-branch

# Create and switch to new branch
git checkout -b new-branch-name
Scenario 3: Student wants to undo last commit
bash
# Undo last commit but keep changes
git reset --soft HEAD~1

# Undo last commit and discard changes (careful!)
git reset --hard HEAD~1
Scenario 4: Student made changes on wrong branch
bash
# Save changes temporarily
git stash

# Switch to correct branch
git checkout correct-branch

# Apply saved changes
git stash pop

# Quick Reference Card for Students

Task	Command

Clone fork	git clone https://github.com/YOUR-USERNAME/AAI_primer.git

Add upstream	git remote add upstream https://github.com/svhari/AAI_primer.git

Create branch	git checkout -b branch-name

Check status	git status

Stage changes	git add .

Commit	git commit -m "message"

Push to YOUR fork	git push origin branch-name

Pull from original	git pull upstream main

Update your fork	git push origin main


