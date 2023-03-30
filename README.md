# Helpful-CMDs

## Remove .DS_Store files from a directory, recursively
```
find . -name .DS_Store -exec rm {} \;
```

## Get the number of files in a directory
```
find /path/to/dir -type f | wc -l
```

## Get the number of files in current directory
```
find . -type f | wc -l
```

## Get the number of directories in a directory
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

## List all files in a directory, recursively, and output to a text file. 
```
ls -l1R /path/to/dir > filelisting.txt
```

## Find and replace a text string across all files in a directory, recursively
```
find . -type f -exec sed -i 's/old-string/new-string/g' {} \;
```

## Transfer files from one directory to another
```
rsync -rav /path/to/source /path/to/target
```

## Transfer files from one directory to another (sudo) (cd into target directory)
```
sudo rsync -rav /path/to/source* .
```

## Transfer files from one directory to another (sudo)
```

sudo rsync -rav /path/to/source* /path/to/target
