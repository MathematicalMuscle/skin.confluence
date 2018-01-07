This skin is a modification of [Confluence](https://github.com/xbmc/skin.confluence) to my specifications.  



### Installation via [`script.kodi_setter_upper`](https://github.com/MathematicalMuscle/script.kodi_setter_upper):

Modify the IP address and port and go to this URL in your browser:

[http://10.0.0.120:8080/jsonrpc?request={"jsonrpc":"2.0","id":1,"method":"Addons.ExecuteAddon","params":{"addonid":"script.kodi_setter_upper","params":{"ksu_class":"Addon","addonid":"skin.confluence_mm2","url":"https://github.com/MathematicalMuscle/skin.confluence_mm/archive/krypton_mm2.zip"}}}](http://10.0.0.120:8080/jsonrpc?request={"jsonrpc":"2.0","id":1,"method":"Addons.ExecuteAddon","params":{"addonid":"script.kodi_setter_upper","params":{"ksu_class":"Addon","addonid":"skin.confluence_mm2","url":"https://github.com/MathematicalMuscle/skin.confluence_mm/archive/krypton_mm2.zip"}}})



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
  git rebase krypton_mm
  ```
