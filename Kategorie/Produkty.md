---
tags: kategoria
---
```dataview
table without id
	file.link as Produkt,
	producent as Producent,
	url as WWW,
	cena as Cena
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```