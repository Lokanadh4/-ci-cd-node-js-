cd ..   # repo root
git add .
git commit -m "Add Node app, Dockerfile and GitHub Actions workflow"
git branch -M main
# connect to remote repo you created on GitHub:
git remote add origin git@github.com:YOUR_GITHUB_USER/ci-cd-nodejs.git
git push -u origin main
# Create a README file
@"
# CI/CD Node.js Project

This project uses GitHub Actions to automatically build and deploy a Node.js app to Docker Hub.
"@ | Out-File -Encoding utf8 README.md

# Add all files
git add .
git commit -m "Initial CI/CD setup"
git branch -M main

# Connect your GitHub repository (replace USERNAME)
git remote add origin https://github.com/<YOUR_USERNAME>/ci-cd-nodejs.git

# Push to GitHub
git push -u origin main
