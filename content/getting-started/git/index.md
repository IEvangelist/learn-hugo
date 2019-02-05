---
title: "Git - Source Control"
weight: 2
---

## Initialize

Initialize Git

```
git init
```

Add submodule

```
git submodule add https://github.com/matcornic/hugo-theme-learn themes/hugo-theme-learn
```

## Remote Repository

Open https://github.com/new to create a new remote repository. Name it accordingly. Do __not__ change any other defaults. Click "__Create Repository__".

![New GitHub Repo](/getting-started/git/images/new-repo.png?classes=shadow,border)

## Configure Remote

From the __Git__ command line, if you were execute `git remote -v` it will tell you what remote branches are configured. The list should be empty right now, but let's change that.

```
git remote add upstream https://github.com/IEvangelist/learn-hugo.git
```

```
λ git remote -v
upstream        https://github.com/IEvangelist/learn-hugo.git (fetch)
upstream        https://github.com/IEvangelist/learn-hugo.git (push)
```