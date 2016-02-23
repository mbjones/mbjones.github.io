mbjones.github.io
=================

Matt Jones on GitHub

This site uses jekyll-scholar to generate the publications list, so will not 
properly build on GitHub pages.  Use `jekyll build` to build on the source branch to build the site locally, then commit the source branch, and publish the site to 
the master branch using:

```sh
#!/bin/bash                                                                                                                                                 
git branch -D master
git checkout -b master
git filter-branch --subdirectory-filter _site/ -f
git checkout source
git push --all origin
```
