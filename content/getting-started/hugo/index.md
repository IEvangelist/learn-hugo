---
title: "Hugo"
weight: 1
---

## What Is Hugo?

Hugo is a static site generator. 

> The world’s fastest framework for building websites. <cite><a href='https://gohugo.io/' target='_blank'>Hugo</a></cite>

You might be asking yourself, "what is a static site?". Who here has heard of <i class="fab fa-wordpress"></i> Wordpress - this is a dynamic site. Each request dynamically generates the HTML to be served to the client. As you can imagine there could be performance implications related to this. Static sites are pre-generated and served with no additional overhead as they are simply raw HTML files. This makes static sites load extremely fast!

> Hugo is one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again. <cite><a href='https://gohugo.io/' target='_blank'>Hugo</a></cite>

# Themes

There are nearly 1,000 pre-built themes. <a href='https://themes.gohugo.io/' target='_blank'>Hugo Themes</a>

## Hugo Commands

Let's start by finding the desired working directory for the hugo site. This directory will be the location in which you develop your site and also serve as your local git repository, more on that later. Execute the following command to create a new hugo website.

```
hugo new site learn-hugo
```

Change directory, navigating into the newly created site folder. Then, open __Visual Studio Code__ in with this folder as the command line argument.

```
cd learn-hugo && code .
```

## Adding Content

To add chapters, invoke the `hugo new` command with the `--kind chapter` switch - additionally specifying the folder and markdown file name. This command will add a "Getting Started" chapter.

```
hugo new --kind chapter getting-started/_index.md
```

To add sub-pages, invoke the `hugo new` with the top-level chapter, sub folder and markdown file.

```
hugo new getting-started/hugo/index.md
```

Add content to these markdown files to see how it renders. Test your site out locally with the following command, note that this also has "Live Reload" for convenient development.

```
hugo serve
```