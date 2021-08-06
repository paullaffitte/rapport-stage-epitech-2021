# rapport-stage-epitech-2021
End of study internship report - Promotion {EPITECH.} 2021

## Install dependencies

```bash
sudo apt update && sudo apt install -y \
  texlive \
  texlive-latex-extra \
  latexmk

tlmgr init-usertree

tlmgr install --verify-repo=none --usermode --no-persistent-downloads \
  biblatex \
  logreq
```

## Build and preview

- Install VS Code `LaTeX Workshop` extension.
- In a `.tex` file, use `Ctrl+Alt+B` to build and `Ctrl+Alt+V` to show the result.

## Troubleshooting

### tlmgr: Local TeX Live (20XX) is older than remote repository (20YY)

```bash
tlmgr repository add ftp://tug.org/historic/systems/texlive/20XX/tlnet-final
tlmgr repository list
tlmgr repository remove http://mirror.ctan.org/systems/texlive/tlnet
tlmgr option repository ftp://tug.org/historic/systems/texlive/20XX/tlnet-final
```

(source: https://askubuntu.com/questions/1265533/tlmgr-local-tex-live-2019-is-older-than-remote-repository-2020)
