# Using Git Commands pushing other repo code to our repo
## Assuming you want to push the code from RepoA to RepoB:
### Clone RepoA locally:
- git clone <RepoA_URL>
- cd RepoA
### Add RepoB as a new remote:
- git remote add RepoB <RepoB_URL>

### Fetch code from RepoB:
- git fetch RepoB

### Checkout the branch you want to push:
- git checkout <branch_name>

### Push the code to RepoB:
- git push RepoB
  
## lms-team-1/praneeth to test/dev
- git clone -b praneeth https://github.com/digital-lync-2023/lms-team-1.git
- cd lms-team-1/
- git remote add murali https://github.com/muralialakuntla3/test.git
- git fetch murali
- git checkout dev
- git push murali

