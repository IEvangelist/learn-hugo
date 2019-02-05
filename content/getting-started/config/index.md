---
title: "Config"
weight: 3
---

## Configure Hugo

Add the following to the end of the `config.toml` file. For more details on the various configurations, please see <a href='https://gohugo.io/getting-started/configuration/' target='_blank'>configure hugo</a>. This will configure the __theme__ in hugo, enabling it to consume the previously added "hugo-theme-learn" theme.

```toml
# Change the default theme to be use when building the site with Hugo
theme = "hugo-theme-learn"

# For search functionality
[outputs]
home = [ "HTML", "RSS", "JSON"]
```

## Additional / Optional Parameters

There are additional paramaters that are optional. For example you can render a __More__ menu navigation items, like displayed on this tutorial.

```toml
[[menu.shortcuts]]
name = "<i class='fab fa-github'></i> Github Repository"
identifier = "learn-hugo"
url = "https://github.com/IEvangelist/learn-hugo"
weight = 1

[[menu.shortcuts]]
name = "<i class='fab fa-twitter'></i> Follow @davidpine7"
identifier = "twitter"
url = "https://twitter.com/davidpine7"
weight = 2
```

For more details please see <a href='https://learn.netlify.com/en/basics/configuration/' target='_blank'>these theme specific configurations.</a>