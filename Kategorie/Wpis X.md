---
tags: kategoria
---
```dataview
table without id
	file.link as Wpis,
	url as WWW,
	tags as Tagi
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```