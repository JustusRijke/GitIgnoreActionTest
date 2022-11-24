[![GitIgnore](../../actions/workflows/GitIgnore.yml/badge.svg)](../../actions/workflows/GitIgnore.yml)

# GitIgnore action

## Overview
This repo contains a GitHub action that checks if a repo contains ignored files.

The GitIgnore action should fail, because the repo contains `ignoreme`, which is declared in `.gitignore`.

## Removing ignored files that were added
```
git rm -r --cached .
git add .
git commit -am "Remove ignored files"
```
