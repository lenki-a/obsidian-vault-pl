---
tags: kategoria
---
```dataview
table without id
	file.link as Firma,
	kraj as Kraj,
	specjalizacja as Specjalizacja,
	url as WWW
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.link asc
```