Follow Steps below:

1. Run "npm install" in root to install all node module dependencies.

2. To deploy on GH Pages, use these commands:

git branch gh-pages
git checkout gh-pages && git merge main --no-edit
npm run build
git add dist -f && git commit -m "Deployment commit"
git subtree push --prefix dist origin gh-pages

3. Return to your main branch via "git checkout main"