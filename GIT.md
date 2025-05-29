## Create a patch from the last commit
```bash
git format-patch -n HEAD^
```
## Apply a patch
```bash
git apply name-of-patch-file.patch
```
if it fails you might want to try
```bash
git apply --3way name-of-patch-file.patch
```
solve the conflicts and commit the changes
