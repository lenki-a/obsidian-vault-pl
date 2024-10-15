---
tags: kategoria
---
```dataview
table without id
	file.link as Strona,
	url as WWW,
	opis as Opis
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```