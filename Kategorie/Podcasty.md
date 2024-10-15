---
tags: kategoria
---
```dataview
table without id
	tytuł as Tytuł,
	autor as Autor,
	ocena as Ocena
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```