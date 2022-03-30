## TIL 22-03-30
---
1. Hexo
   - hexo init dir-name
   - cd dir-name
   - npm install
   **check node version if hexo has some errors when try posting**
   - git remote add origin repoURL
   - hexo post title
     - cd source to check posts
     - add comments through vi
   - hexo server
   - edit _config.yml file to change configuration
     - check #Deployment area
       deploy:
       	 type: git
	 repo: repoURL
	 branch: main
   - hexo clean && hexo deploy

2. .gitignore

3. branch
   - git branch
   - git branch -r
   - git branch newBranchName
   - git checkout newBranchName

   - git push origin branchName
   - git merge branchName
   - git branch -D branchName

4. git flow strategy(models for work)
   - git flow
   - github flow
---
