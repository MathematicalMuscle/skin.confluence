This skin is a modification of [Confluence](https://github.com/xbmc/skin.confluence) to my specifications.  



### Git Workflow

(Based on [GitHub Standard Fork & Pull Request Workflow](https://gist.github.com/Chaser324/ce0505fbed06b947d962))


0. One time only steps:

  ```bash
  # Create a new branch
  git checkout -b krypton_mm2
  ```

1. Make commits to the `krypton_mm2` branch
2. When necessary, merge upstream changes:

  ```bash
  # If there were any new commits, rebase your development branch
  git checkout krypton_mm2
  git rebase krypton
  ```
