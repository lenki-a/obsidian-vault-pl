---
tags: kategoria
---
```dataview
table without id
	file.name as Lokalizacja,
	lokalizacja as Koordynaty,
	kraj as Kraj,
	url as WWW
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```