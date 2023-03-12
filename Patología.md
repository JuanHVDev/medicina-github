---
cssclass: btn
---

```button
name Agregar una nueva Patología
type note(<% tp.file.title%>, split) template
action tp_Patología
color purple
```


```dataview
TABLE author AS Autor, creado AS Creado, modificado AS Modificado, tags from "Patologías"

```
