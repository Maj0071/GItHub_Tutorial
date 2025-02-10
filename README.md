# GItHub_Tutorial
A tutorial on how to use GitHub commands

# clone repository
git clone <github-link>
cd into new directory

# Adding new read.me file can be any file
# Add changes to github
echo "Adding a demo update" >> README2.md
git add README2.md
git commit -m "Updated README with demo text"
git push

# pull other people's code from branch
git pull

# Create a new branch
git branch feature-demo

# Switch to the new branch
git checkout feature-demo

# Make changes on this branch
echo "This is a feature branch" >> feature.txt
git add feature.txt
git commit -m "Add feature file"

# Push the branch to GitHub
git push -u origin feature-demo

# switch between branches
git checkout main
git checkout feature-demo

# Merge branches back to main
git checkout main
git merge feature-demo
git push


# additional features uncommon

# makes a visual of your commit history in the terminal
git log --oneline --graph --all

# Temorarily saves uncommited changes
# Save uncommitted changes
git stash

# Switch branches
git checkout main

# Restore the changes later
git stash pop

# Apply a specific commit from one branch to another.
# Find the commit hash you want to apply
git log --oneline

# Apply that commit to your current branch
git cherry-pick <commit-hash>

# Show who made changes to each line of a file.
git blame README.md
