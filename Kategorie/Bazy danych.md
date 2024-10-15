---
tags:
  - kategoria
---
```dataview
table without id
	file.link as Nazwa,
	url as WWW
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
sort file.name asc
```