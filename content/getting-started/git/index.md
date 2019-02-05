---
title: "Git - Source Control"
weight: 2
---

## Initialize Git

From the root directory of the newly created hugo site, invoke the following command. This will initialize the directory for git source control - enabling various source control specific features. For more details on this and other git commands please see <a href='https://git-scm.com/about' target='_blank'>git docs</a>.

```
git init
```

With the source control tracking in place, we need to add a submodule. We'll execute the `git submodule add` command with the desired theme URL and given path.

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

## Git Flow

Now, we'll add all of our code to staging.

```
git add -A
```

I often use `git status` to check the status of local changes. Let's commit the changes with a commit message.

```
git commit -m "Yay, I have working code!"
```

Now, let's push our latest source upstream.

```
git push upstream master
```

### Git Ignore

{{% notice tip %}}
This isn't required, but really eliminates all the noise from the various local builds.
{{% /notice %}}

We could add a `.gitignore` file so that we can specify a few things for __Git__ to ... well, ignore.

{{%attachments title=".gitignore file" style="grey"%}}