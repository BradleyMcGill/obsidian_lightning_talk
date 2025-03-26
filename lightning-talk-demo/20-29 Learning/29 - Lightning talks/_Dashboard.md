Write here about what the sub directories are about



```dataview 
TABLE file.mtime AS Edited,
	file.folder AS Folder
WHERE date(now) - file.mtime <= dur(3 days)
	AND file.ctime < date(now) - dur(3 days) 
```

```dataview 
TABLE file.name
WHERE contains(file.tags, "TODO")
```

