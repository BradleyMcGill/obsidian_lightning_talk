Home dashboard for notes




Active:
```dataview 
TABLE file.name, file.mtime AS LastEdited  
FROM ""  
SORT file.mtime DESC  
LIMIT 10  
```

TODO:
```dataview
LIST file.name  
WHERE contains(file.tags, "TODO")  
```
