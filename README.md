This skin is a modification of [Confluence](https://github.com/xbmc/skin.confluence) to my specifications.  

### Git Workflow

(Based on [GitHub Standard Fork & Pull Request Workflow](https://gist.github.com/Chaser324/ce0505fbed06b947d962))

0. One time only steps:

  ```bash
  # Add 'upstream' repo to list of remotes
  git remote add upstream https://github.com/xbmc/skin.confluence.git

  # Verify the new remote named 'upstream'
  git remote -v

  # Fetch from upstream remote
  git fetch upstream

  # View all branches, including those from upstream
  git branch -va

  # Checkout your master branch and merge upstream
  git checkout master
  git merge upstream/master

  # Checkout the master branch - you want your new branch to come from master
  git checkout master

  # Create a new branch
  git checkout -b master_mm
  ```

1. To be continued...
