# Helpful-CMDs

## Recursively remove .DS_Store files from a directory
```
find . -name .DS_Store -exec rm {} \;
```

## Get the number of files in a directory
```
find /path/to/dir -type f | wc -l
```
