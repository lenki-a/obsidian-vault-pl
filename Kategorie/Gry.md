---
tags: kategoria
---
```dataview
table without id
	file.link as Gra,
	ocena as Ocena,
	typ as Gatunek
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```