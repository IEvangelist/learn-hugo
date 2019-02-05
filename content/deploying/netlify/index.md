---
title: "Netlify"
---

## Configure Netlify

Login to <a href='https://app.netlify.com/account/sites' target='_blank'>Netlify</a> and click "__New site from Git__". Now, click the __<i class='fab fa-github'></i> GitHub__ button. At the bottom of the screen is a link that reads "Configure the Netlify app on GitHub". This will open a new window, where you're able to __Select repositories__ that enable Netlify to pull from.

The defaults are perfectly acceptable, as __Netlify__ sees your repository as a __Hugo__ site and configures this automatically. It knows to build the site using the `hugo` command and that the _public_ directory is where your rendered site resides.

![Netlify Continuous Deployment](/deploying/netlify/images/cd.png?classes=shadow,border)