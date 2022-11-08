# Install

- Linux - Ubuntu/Debian:

```
sudo apt-get install git-flow
```

- Link to install on other operating systems: https://github.com/petervanderdoes/gitflow-avh/wiki/Installation

# Commands

- Init
  
```
git flow init
```

- Configure as you want your branches like ``feature/``, ``release/``, ``bugfix/``, ``suport/``, ``hotfix/``.

- feature: it is a copy of the main codebase where an individual or team of software developers can work on a new feature(small modifications) until it is complete.
- realese: it is used to create modifications in develop branch to later merge to master.
- bugfix: it is used to fix problems in the project.
- hotfix: it is used to fix immediate problems in main branch.

### Feature

- Init a feature branch

```
git flow feature start branch_name
```

- Finish the feature branch and to merge it to develop.

```
git flow feature finish branch_name
```

**It delete the current feature(branch_name) and merge to develop.**

### Release

- Init a realese branch
 
```
git flow release start 0.1.0
```

- Finish a realese branch

```
git flow release finish 0.1.0
```

### HotFix

- Init a hotflix branch

```
git flow hotfix start readme-hotfix
```

- Finish a hotfix branch

```
git flow hotfix finish readme-hotfix
```

```md
- Hotfix branch 'hotfix/readme-hotfix' has been merged into 'main'
- The hotfix was tagged 'readme-hotfix'
- Hotfix tag 'readme-hotfix' has been back-merged into 'develop'
- Hotfix branch 'hotfix/readme-hotfix' has been locally deleted
- You are now on branch 'develop'
```