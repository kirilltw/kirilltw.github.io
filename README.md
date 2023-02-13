# kirilltw.github.io

This repo stores the source code for my [website](https://kirilltw.github.io/). The main challenges I faced while creating the website were as follows:

- **Multiple git accounts and respective SSH keys on GitHub**

  These days, each GitHub account needs a unique SSH key. When I created my second account and tried to push some local commits, git rejected stating that my credentials were incorrect. After a brief research, I came across [this thread](https://gist.github.com/jexchan/2351996#multiple-ssh-keys-settings-for-different-github-account) that finally helped me resolve the issue.

- **Building my own Docker image with the required software**

  To avoid installing Ruby, Jekyll, and Bundler on my machine because of possible issues with version compatibility, I followed the excellent [tutorial](https://dev.to/billraymond/video-develop-jekyll-or-github-pages-using-docker-containers-2i04) by Bill Raymond and successfully built my Jekyll website in no time.

- **Changing Jekyll themes**

  Because I was new to Jekyll, it took me some time to figure out where the folder `_layouts` was located and how to switch to a new theme. [This thread](https://stackoverflow.com/questions/38891463/jekyll-default-installation-doesnt-have-layouts-directory) quickly brought me up to speed and allowed me to tackle the issue.

Ideally, the GitHub documentation should be updated to bridge these gaps and make the experience of building websites with [GitHub Pages](https://pages.github.com/) even more streamlined.