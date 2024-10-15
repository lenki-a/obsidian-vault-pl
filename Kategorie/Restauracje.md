---
tags: kategoria
---
```dataview
table without id
	file.link as Restauracja,
	lokalizacja as Gdzie,
	ocena as Ocena,
	cena as Cena
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```