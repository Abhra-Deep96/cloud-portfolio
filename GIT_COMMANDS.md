# 1. Check whether Git is installed
git --version

# 2. Check the Git username configured on the computer
git config --global user.name

# 3. Check the Git email configured on the computer
git config --global user.email

# 4. Check the current state of the repository
git status

# 5. Connect the local repository to the GitHub repository
git remote add origin https://github.com/Abhra-Deep96/cloud-portfolio.git

# 6. Verify the configured remote repository
git remote -v

# 7. Stage a specific changed file
git add README.md

# 8. Create a commit containing the staged changes
git commit -m "Document V1 S3 static website architecture"

# 9. Upload local commits to GitHub
git push

# During the initial setup we also used:
git push -u origin main
