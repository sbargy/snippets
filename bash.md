## Get Extensions
> Kind of a hack, but it was fast to figure it out...
To see all the extensions of files in a directory, get the last
4 characters of each line...

```
[~/Pictures/Family/iCloud Photos]
scott@bargamac$ ls -1 * | grep -o "....$" | sort -u
.JPG
.MOV
.PNG
.jpg
.mp4
.png
JPEG
list
```

## Trim first column
> get rid of the history number here

```
(contents of file x)
26484  git remote -v
26485  git checkout develop
26486  git merge --no-ff feature/restframework
26487  git branch -d feature/restframework
26488  git push origin develop
```

```
cat x | awk '{ print $2, $3, $4, $5, $6 }'
```

> yields

```
git remote -v
git checkout develop
git merge --no-ff feature/restframework
git branch -d feature/restframework
git push origin develop
```
