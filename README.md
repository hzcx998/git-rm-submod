# git-rm-submod
git remove submodule methond 

#### 1. remove test_mod

```bash

# step 1
vim .git/config

-[submodule "test_mod"]
-        active = true
-        url = https://github.com/yourname/test_mod

# step 2
rm -rf .git/modules/test_mod

# step 3
rm -rf test_mod

# step 4
git rm --cached test_mod
```


#### 2. remove hello/test_mod

```bash
vim .git/config
rm -rf .git/modules/hello/test_mod
rm -rf hello/test_mod
git rm --cached hello/test_mod
```
