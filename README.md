# Helpful-CMDs

## Recursively remove .DS_Store files from a directory
```
find . -name .DS_Store -exec rm {} \;
```

## Get the number of files in a directory
```
find /path/to/dir -type f | wc -l
```


## Get the number of files in a directory
```
find /path/to/dir -type d | wc -l
```

## Get the size of a directory
```
du -sh /path/to/dir
```

## Find all files in a directory over 100 megabytes, recursively
```
find . -xdev -type f -size +100M -exec ls -lh {} \;
```

## Find all hidden files in a directory, recursively
```
find . -name '.*'
```
