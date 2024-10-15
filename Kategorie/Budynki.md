---
tags: kategoria
---
```dataview
table without id
	file.link as Nazwa,
	styl as Styl,
	architekt as Architekt,
	lokalizacja as Lokalizacja
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
sort file.name asc
```