------------------------------
Kind of a hack, but it was fast to figure it out...
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

------------------------------

