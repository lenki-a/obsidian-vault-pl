---
tags: kategoria
---
```dataview
table without id
	file.link as Tytuł,
	ważność as Priorytet
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```