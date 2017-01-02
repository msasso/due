# due
due is du(1), enhanced.

## Rationale

`du` can be overly verbose. `due` folds smaller files and folders into their parends based on a given threshold. This is useful to understand which directories use big chunks of disk space or inodes.

## Syntax

```
due [-l limit] [-S space] [-F files] [path]
   -l limit   Display at most "limit" lines. By default this is $LINES - 4.
   -S space   Set the threshold to "space". You can use the usual suffixes (for instance 4GB, 1T, and so on...) By default this is 100MB.
   -F files   Set the threshold to "files". You can use standard suffixes (for instance 5k.) By default this is 10k.
   path       The path to evaulate. Current directory by default.
```
