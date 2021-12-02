# submodule-test
Test of git submodules

``` bash
# make it so that git status will include changes to submodules.
git config status.submodulesummary 1

# make it so that git diff will show a list of submodule commit messages
# instead of just the previous and current commit hashes.
git config diff.submodule log

```


# [githooks]

``` bash
mkdir ~/.githooks
git config --global core.hooksPath ~/.githooks

cat - <<"Q" > ~/.githooks/post-checkout
#! /bin/bash

echo "Check for submodules!"
Q
chmod +x ~/.githooks/post-checkout
```

## Aliases


``` bash
git config --global alias.cl 'clone --recursive'

```


[cheatsheet]:https://faun.pub/git-submodule-cheatsheet-29a3bfe443c3
