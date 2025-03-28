---
cssclasses: []
---
Write here about what the sub directories are about

RECENT:
```dataview 
TABLE file.mtime AS Edited,  
      file.folder AS Folder  
WHERE startswith(file.path, regexreplace(this.file.path, "/[^/]+$", ""))  
```

TODO:
```dataview 
LIST file.name  
WHERE contains(file.tags, "TODO")  
AND startswith(file.path, regexreplace(this.file.path, "/[^/]+$", ""))
```

