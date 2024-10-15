---
tags: kategoria
---
```dataview
table without id
	file.link as Nazwa,
	dokumentacja as Dokumentacja,
	tags as Tagi
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```