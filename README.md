cd ..   # repo root
git add .
git commit -m "Add Node app, Dockerfile and GitHub Actions workflow"
git branch -M main
# connect to remote repo you created on GitHub:
git remote add origin git@github.com:YOUR_GITHUB_USER/ci-cd-nodejs.git
git push -u origin main
