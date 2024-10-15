---
tags: kategoria
---
```dataview
table without id
	file.link as Przepis,
	kraj as Kraj,
	ocena as Ocena
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```