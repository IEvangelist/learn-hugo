---
title: "Config"
weight: 3
---

## Configure Hugo

Add the following to the end of the `config.toml` file. For more details on the various configurations, please see <a href='https://gohugo.io/getting-started/configuration/' target='_blank'>configure hugo</a>. This will configure the __theme__ in hugo, enabling it to consume the previously added "hugo-theme-learn" theme.

```
# Change the default theme to be use when building the site with Hugo
theme = "hugo-theme-learn"

# For search functionality
[outputs]
home = [ "HTML", "RSS", "JSON"]
```