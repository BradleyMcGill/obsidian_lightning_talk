Write here about what the sub directories are about



```dataview 
TABLE file.mtime AS Edited,
	file.folder AS Folder
FROM "10-19 Projects"
```

```dataview 
TABLE file.name
FROM "10-19 Projects"
WHERE contains(file.tags, "TODO")
```

