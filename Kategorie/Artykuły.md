---
tags: kategoria
---
```dataview
table without id
	file.link as Nazwa,
	autor as Autor,
	tags as Tagi,
	ocena as Ocena
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
sort file.name asc
```

