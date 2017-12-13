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

  # Checkout your krypton branch and merge upstream
  git checkout -b krypton origin/krypton
  git merge upstream/krypton

  # Checkout the krypton branch - you want your new branch to come from krypton
  git checkout krypton

  # Create a new branch
  git checkout -b krypton_mm
  ```

1. Make commits to the `krypton_mm` branch
2. When necessary, merge upstream changes:

  ```bash
  # Fetch upstream master and merge with your repo's master branch
  git fetch upstream
  git checkout krypton
  git merge upstream/krypton

  # If there were any new commits, rebase your development branch
  git checkout krypton_mm
  git rebase krypton
  ```
