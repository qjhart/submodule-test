# submodule-test
Test of git submodules

# Git configuration settings

``` bash
# make it so that git status will include changes to submodules.
git config status.submodulesummary 1

# make it so that git diff will show a list of submodule commit messages
# instead of just the previous and current commit hashes.
git config diff.submodule log

git config submodule.recurse 1
```


You create a new submodule

``` bash
git submodule add https://github.com/qjhart/mod-part.git
git submodule add https://github.com/qjhart/mod-part.git part2
```


## [githooks]

Rather than relying on the users git configuration, we

[githooks]:https://git-scm.com/docs/githooks
[cheatsheet]:https://faun.pub/git-submodule-cheatsheet-29a3bfe443c3
