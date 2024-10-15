---
tags: kategoria
---
```dataview
table without id
	file.link as Cytat,
	autor as Autor,
	url as WWW
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```